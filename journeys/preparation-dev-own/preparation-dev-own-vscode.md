# Setting Up VS Code for IoT Edge Development #

You are going to install the required VS Code extensions and optionally connect to a Linux VM via SSH for remote development.
*Please keep in mind, if you want to work in a reote VM you will need to install all prerequisites in that VM after you've connected to it*

## Steps ##
| # | Step   |
|-|-|
|1.| Optional: install the "Remote Development" extension bundle if you'd like to develop inside a remote VM
|2.| Optional: to connect to your VM via the Remote SSH extension (part of Remote Development extension) check out [:blue_book: hints for this challenge](preparation-dev-own-vs-hints.md#Configure-Remote-SSH-extension-to-acces-the-remote-VM).
|3.| Open VS Code and navigate to the Extensions blade [:blue_book: hints for this challenge](preparation-dev-own-vs-hints.md)
|4.| Search for "Azure IoT Edge"
|5.| Install the extension
|6.| Depending on your prefererred programming language/technology you will need to install other pieces, like e.g. .NET Core, NodeJS etc. *[Here is how you can install the latest .NET Core Version on Linux](https://dotnet.microsoft.com/download/linux-package-manager/ubuntu16-04/sdk-current)*
|7.| Create an IoT Edge Solution, when asked for a container registry please point to your Azure Container Registry [:blue_book: hints for this challenge](preparation-dev-own-vs-hints.md#Create-a-new-IoT-Edge-Solution)
|8.| Set credentials for your Azure Container Regisry in the *.env* file
|9.| Explore *deployment.template.json* to understand the deployment manifest structure
|10.| Now build container images for your modules and push them into your container registry (*Hint: use the IoT Edge Extension to "Build and Push IoT Edge Solution"*) 
|11.| Create a deployment using target condition ```deviceId='<YOUR_DEVICE_ID>'``` (*Hint: use the IoT Edge Extension to create a "Deployment at Scale" and provide your deployment manifest*)

In case you would like to have more information about debugging options and various tools available for IoT Edge development, please refer to *[this documentation](https://docs.microsoft.com/en-us/azure/iot-edge/development-environment)*