# Creating Azure IoT Services #

You are going to create an IoT Hub, Azure Container Registry and optionally a Device Provisioning Service (DPS). 

## Steps ##
| # | Step   |
|-|-|
|1.| Login into Azure Portal
|2.| Create an IoT Hub using [this guide](https://docs.microsoft.com/en-us/azure/iot-dps/tutorial-set-up-cloud#create-an-iot-hub)
|3.| Create Azure Container Registry using *[this guide](https://docs.microsoft.com/en-us/azure/container-registry/container-registry-get-started-portal#create-a-container-registry)*
|4.| If DPS is not used, please refer to *[this guide](https://docs.microsoft.com/en-us/azure/iot-edge/how-to-register-device#register-in-the-azure-portal)* to provision your IoT Edge device directly with the IoT Hub. Don't forget to grab the primary connection string for your device. Otherwise proceed with step *5*
|5.| Optional: create a Device Provisioning Service as described in *[this guide](https://docs.microsoft.com/en-us/azure/iot-dps/tutorial-set-up-cloud#create-a-device-provisioning-service-instance-and-get-the-id-scope)*
|6.| Optional: link your IoT Hub to the Device Provisioning Service you've created using *[this guide](https://docs.microsoft.com/en-us/azure/iot-dps/tutorial-set-up-cloud#link-the-device-provisioning-service-to-an-iot-hub)*
|7.| Optional: review supported attestation mechanisms *[here](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security)* 
|8.| Optional: for simplicity we'll use *individual enrollments* with symmetric key. Please refer to *[this guide](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-symmetric-key-attestation)* for details on how to create an enrollment for your IoT Edge Device (*Hint: don't forget to specify that it is an IoT Edge device*)