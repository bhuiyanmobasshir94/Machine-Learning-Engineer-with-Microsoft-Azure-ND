## Codes

One of our main goals in using the Azure ML SDK is to add automation to our Python projects. One way we can do that is to use the SDK is to create an installation step with a `Makefile` and incorporate the Azure ML SDK with your Continuous Integration workflow.

A Makefile can include a command to install and upgrade packages in a requirements.txt file. Here's an example in Azure Cloud Shell:

```
install:
        pip install --upgrade pip &&\
                pip install --upgrade -r requirements.txt
```

And then, to install, you can simply run `make install` in the shell.