## Interfacing with Datasets

```
from azureml.core.dataset import Dataset

url_paths = [
            'http://yann.lecun.com/exdb/mnist/train-images-idx3-ubyte.gz',
            'http://yann.lecun.com/exdb/mnist/train-labels-idx1-ubyte.gz',
            'http://yann.lecun.com/exdb/mnist/t10k-images-idx3-ubyte.gz',
            'http://yann.lecun.com/exdb/mnist/t10k-labels-idx1-ubyte.gz'
            ]

dataset = Dataset.File.from_files(path=url_paths)
df = dataset.to_pandas_dataframe()
```
## Installing and Using the SDK with a Makefile

One of our main goals in using the Azure ML SDK is to add automation to our Python projects. One way we can do that is to use the SDK is to create an installation step with a `Makefile` and incorporate the Azure ML SDK with your Continuous Integration workflow.

A Makefile can include a command to install and upgrade packages in a `requirements.txt` file. Here's an example in Azure Cloud Shell:

```
(.azure-ml-sdk) udacity@Azure:~/azure-ml-sdk$ cat Makefile
install:
        pip install --upgrade pip &&\
                pip install --upgrade -r requirements.txt
```
The `requirements.txt` file will look like this:

```
(.azure-ml-sdk) udacity@Azure:~/azure-ml-sdk$ cat requirements.txt
ipython
azureml-sdk
```
And then, to install, you can simply run `make install` in the shell.

## Data Preparation

```
ws = Workspace.from_config() 
blob_store = Datastore(ws, "workspaceblobstore")
compute_target = ws.compute_targets["STANDARD_NC6"]
experiment = Experiment(ws, 'MyExperiment') 

input_data = Dataset.File.from_files(
    DataPath(datastore, '20newsgroups/20news.pkl'))
```
## Training Configuration

```
output_data = PipelineData("output_data", datastore=blob_store)

input_named = input_data.as_named_input('input')

steps = [ PythonScriptStep(
    script_name="train.py",
    arguments=["--input", input_named.as_download(),
        "--output", output_data],
    inputs=[input_data],
    outputs=[output_data],
    compute_target=compute_target,
    source_directory="myfolder"
) ]

pipeline = Pipeline(workspace=ws, steps=steps)
```

## Training Validation

```
pipeline_run = experiment.submit(pipeline)
pipeline_run.wait_for_completion()
```

## Listing Past Experiments

```
from azureml.core.experiment import Experiment

# First, we pass in the workspace object `ws` to the `list` method
# and it returns a Python list of `Experiment` objects.  
list_experiments = Experiment.list(ws)

# If we print the contents of the variable,
# we can see the list of all the experiments
# that have been run in that workspace.
print(list_experiments)
[Experiment(Name: dataset_profile,
 Workspace: Azure-ML-Workspace), Experiment(Name: binary-classification,
 Workspace: Azure-ML-Workspace), Experiment(Name: regression,
 Workspace: Azure-ML-Workspace), Experiment(Name: sfautoml]
```

##  Submitting New Experiments

```
from azureml.core.experiment import Experiment

experiment = Experiment(ws, "automl_test_experiment")
run = experiment.submit(config=automl_config, show_output=True)
```
