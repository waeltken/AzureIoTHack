# Let's run the application

In the folder 'raspberrypi_app' you will find the application we want to run on our Pi, so it sends us the temperature data we wish to collect. This is a node.js application and you need to set up your Pi so the application can be run there.

## Prepare your Pi
1. Connect to your Pi, if you are not already connected to it via SSH, remote desktop or by attaching desktop, mouse and keyboard. If you are connected to it via the last two options, please open a terminal.


## Configure the application



## Run the application

1. Now you are going to need the Azure IoT Hub connection string.
    ```bash
    echo $connection
    ```
    If this does not print your connection string you are potentially using another terminal. You can just store it again.
    ```bash
    connection=$(az iot hub device-identity connection-string show --device-id myPi --hub-name $prefix'iotpihub' --output tsv)
    ```
1. Now we give the connection string and run the application:
    ```bash
    ```