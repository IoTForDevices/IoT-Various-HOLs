# Image Classification at the Edge with Custom Vision
The original description of this tutorial can be [found here](https://docs.microsoft.com/en-us/azure/iot-edge/tutorial-deploy-custom-vision). This HOL guide is available to have all prerequisites in place in one single location. Before being able to run the Custom Vision tutorial, you must have the right tools installed on your development machine and you must have an Azure IoT Edge device running Linux available. The latter can also be hosted in an Azure VM.
## Development Machine
This tutorial teaches the development steps for Visual Studio Code, so this needs to be installed on your development machine. Additionally, you need to install
- [Git](https://git-scm.com/), to pull module template packages later in this tutorial.
- [C# for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp) (powered by OmniSharp) extension
- [.NET Core 2.2 SDK](https://www.microsoft.com/net/download)
## Azure IoT Edge Device on Linux
The Azure IoT Edge runtime is what turns a device into an IoT Edge device. You will now create an Azure Virtual Machine that will contain the Azure IoT Edge runtime. To do so, take a look at [this document](https://docs.microsoft.com/en-us/azure/iot-edge/how-to-install-iot-edge-ubuntuvm).

NOTE: You don't have to create a new IoT Hub if you still have one from a previous HOL. You can simply re-use that IoT Hub for this HOL. Just make sure to pass the right credentials. Also, as the document states, it is probably the easiest to provide a user name - password combination for the VM and make sure to have the SSH port enabled to be able to remotely connect to your VM.

Once the Azure IoT Edge VM is deployed, you need to add it to your IoT Hub. You can do so by following the steps in [this document](https://docs.microsoft.com/en-us/azure/iot-edge/how-to-register-device-portal#create-a-device) (steps 1 - 5).

Now you have everything ready to start the actual HOL, so this is a good moment to continue with the [remaining prerequisites](https://docs.microsoft.com/en-us/azure/iot-edge/tutorial-deploy-custom-vision#prerequisites).

Having all tools installed, now move on to [this location in the original HOL document](https://docs.microsoft.com/en-us/azure/iot-edge/tutorial-deploy-custom-vision#build-an-image-classifier-with-custom-vision). From there simply follow all steps.
