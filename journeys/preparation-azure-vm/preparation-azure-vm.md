# Using an Ubuntu VM for IoT Edge #

You are going to create an Ubuntu VM on Azure and install the IoT Edge Runtime. This VM will serve as a simulated Edge device.

## Steps ##
| # | Step   |
|-|-|
|1.| Login into Azure Portal
|2.| Create an Ubuntu VM with pre-installed IoT Edge [:blue_book: hints for this challenge](vm_hints.md) OR
|3.| In case you would like to install the IoT Edge Runtime all by yourself please create a vanilla Ubuntu VM (16.04 or 19.04) and use *[this guide](https://docs.microsoft.com/en-us/azure/iot-edge/how-to-install-iot-edge-linux)*
|4.| Edit *config.yaml* to configure IoT Edge security daemon. Refer to *[this guide](https://docs.microsoft.com/en-us/azure/iot-edge/how-to-install-iot-edge-linux#configure-the-security-daemon)* for details on various ways to configure it. For the sake of simplicity we'll use *[manual provisioning](https://docs.microsoft.com/en-us/azure/iot-edge/how-to-install-iot-edge-linux#option-1-manual-provisioning)*. Feel free to experiment with Device Provisioning Sevice.
|5.| After you've edited *config.yaml* and restarted the daemon run ``` iotedge check ``` to verify that IoT Edge is up and running. You can run ``` iotedge list ``` to see the list of running modules. Since we haven't deployed any modules yet, edgeAgent should be the only one.