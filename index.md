---

layout: ribbon

style: |

    #Cover h2 {
        margin:30px 0 0;
        color:#FFF;
        text-align:center;
        font-size:70px;
        }
    #Cover p {
        margin:10px 0 0;
        text-align:center;
        color:#FFF;
        font-style:italic;
        font-size:20px;
        }
        #Cover p a {
            color:#FFF;
            }
    #Picture h2 {
        color:#FFF;
        }
    #SeeMore h2 {
        font-size:100px
        }
    #SeeMore img {
        width:0.72em;
        height:0.72em;
        }
---

# IoT Workshop
 
 IoT solutions on Azure
 
 Excersises


![](pictures/cover.jpg)


## I:🌸 Create IoT Hub

1. Go to Azure Portal
1. Create IoT Hub
    - preferable S1 tier
    - 1 unit
    - 4 partitions
1. Create device
    - IoT Devices -> New 
    - with symetric key
1. Go to your device and open connection strings, we will need it later
    - IoT Devices -> your device -> Primary Connection String

## I:🌸 VS Code for IoT Hub

1. In VS Code call *Command Palette* and call *Azure: Sign in*
1. In Explorer at the bottom go to *Azure IoT Hub*
    - select *More actions...*
    - *Select IoT Hub*
1. Select Devices
    - select your device
    - *Start monitoring build-in endpoints*
    - observe messages in Output window

## I:🌸 VS Code Simulate device

1. Select Devices
    - select your device
    - *Send D2C Messages*
    - set your text and send
1. While sending look into Output windows

## II:🥀 Arduino create project

1. Create new project 
    - Shift + Ctrl + P => Command Palette
    - Azure IoT Device Workbench: Create Project  
    - choose project name
    - close all instances of VS Code
    - open again ale wait about minute

## II:🥀 Arduino fun

1. Go to [documentation](https://microsoft.github.io/azure-iot-developer-kit/docs/apis/hts221/) and choose what you want to code
    - LED [blog](https://www.programistkaikot.pl/2020/01/mxchip-zabawy-dioda.html)
    - Buttons [blog](https://www.programistkaikot.pl/2020/01/mxchip-obsuga-przyciskow-uzytkownika.html)
    - Oled [blog](https://www.programistkaikot.pl/2020/01/mxchip-oled-display.html)
    - Humidity & Temperatur [blog](https://www.programistkaikot.pl/2020/02/mxchip-czujnik-wilgotnosci-powietrza.html)
    - Audio 

## III:💮 IoT DevKit

1. Update firmware
    - [Firmware link](https://bit.ly/2riKrLw){:target="_blank"}; [Firmware updating instruction](https://bit.ly/34Pug60){:target="_blank"}
    - Drag and Drop downloaded packege in Windows Explorer
1. Set WIFI connection - Access Point mode
    - => **Hold B, press Reset** - still holding B just press and release Reset still holding B, **release B**
1. Connect to you DevKit access point
1. Configure WIFI at 192.168.0.1        
1. See sensors reading => Press B

## IV:🌹 Getting started 

1. [Upload getting started program](https://aka.ms/devkit/prod/getstarted/latest){:target="_blank"}  [Solution link](https://docs.microsoft.com/en-us/samples/azure-samples/mxchip-iot-devkit-get-started/sample/){:target="_blank"}
1. Configure getting started
	- => **Hold B, press Reset** - still holding B just press and release Reset still holding B,
    - => **release B**
1. Connect to you DevKit access point
1. Configure at 192.168.0.1
    - set WIFI
    - set connection string from recent demo        
	- restart device

## IV:🌹 Getting started - Cold Path

21. Go to Azure portal
	- go to Message routing
	- *Add*
    - on Add Route page *Add endpoint*, storage
    - fill name, choose frequency, choose JSON and *pick container*
    - create or choose storage account and container
22. Check storage
    - body is encripted with Base64

## V:🌺 Hot Path
   - create Azure Function App
   - add new function custom template, in-portal
   - set trigger on IoT Hub, output on CosmosDB
   - add return in function body (return input)
   - in IoT Hub add message routing telemetry to build in events

## VI:🌵 IoT Central
1. Create your own IoT Central application on [Solution page](https://aka.ms/iotcentral){:target="_blank"}
1. Upload [MXChipa current release](https://aka.ms/iotcentral-docs-MXChip-releases){:target="_blank"}
1. Add new device 
    - Devices > + > Real
    - set Device Name

## VI:🌵 IoT Central - configure device
1. Open your device configuration
    - Devices > your device 
    - *Connect* in right upper corner - leave it open
1. Configure device
    - restart device
    - **press A and B** right after restart at the same time
    - connect to access point 
    - open 192.168.0.1 and set all needed informations from point 2 and device display
    - reboot device


