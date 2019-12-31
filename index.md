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


## I: IoT DevKit

1. Update firmware
    - [Firmware link](https://bit.ly/2riKrLw){:target="_blank"}
    - [Firmware updating instruction](https://bit.ly/34Pug60){:target="_blank"}
    - Open in Windows Explorer and drop package that you just downloaded
2. Set WIFI connection 
    - => **Hold B, press Reset** - still holding B just press and release Reset still holding B,
    - => **release B**
3. Connect to you DevKit access point
4. Configure WIFI at 192.168.0.1        
3. See sensors reading => Press B

## II: Create IoT Hub
1. Go to Azure Portal
2. Create IoT Hub
    - preferable S1 tier
    - 1 unit
    - 4 partitions
3. Create device
    - IoT Devices -> New 
    - with symetric key
4. Go to your device and open connection strings, we will need it later
    - IoT Devices -> your device -> Primary Connection String

## III: Getting started
1. [Upload getting started program](https://aka.ms/devkit/prod/getstarted/latest){:target="_blank"}
2. Configure getting started
	- => **Hold B, press Reset** - still holding B just press and release Reset still holding B,
    - => **release B**
	- set connection string from recent demo
	- restart device
3. Observe the magic
	- => VS Code – IoT Hub extension
	- => check Azure Blob storage data

4. [Solution link](https://docs.microsoft.com/en-us/samples/azure-samples/mxchip-iot-devkit-get-started/sample/)

## 3. IoT Central

[Strona rozwiązania](https://aka.ms/iotcentral){:target="_blank"}

[Obrazy oprogramowania dla MXChipa](https://aka.ms/iotcentral-docs-MXChip-releases){:target="_blank"}

1. Update settings: – Fan – Voltage 
2. Call commands: - Echo - Countdown


<!-- 
## Plain Text on Your Slides

Lorem ipsum dolor sit amet, consectetur [adipisicing](#all-kind-of-lists) elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, *quis nostrud* exercitation ullamco laboris **nisi ut aliquip** ex ea commodo consequat. Duis aute irure <i>dolor</i> in reprehenderit in voluptate velit esse cillum <b>dolore</b> eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in `<culpa>` qui officia deserunt mollit anim id est laborum.
 
{:.note}
Shower ['ʃəuə] noun. A person or thing that shows. 

## All Kind of Lists

1. Simple lists are marked with bullets
2. Ordered lists begin with a number
3. You can even nest lists one inside another
    - Or mix their types
    - But do not go too far
    - Otherwise audience will be bored
4. Look, seven rows exactly!

## Serious Citations

<figure markdown="1">

> Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia.

<figcaption>Marcus Tullius Cicero</figcaption>
</figure>

## Code Samples

    <!DOCTYPE html>
    <html lang="en">
    <mark><head></mark> <mark class="comment">< !--Comment-- ></mark>
        <title>Shower</title>
        <meta charset="<mark class="important">UTF-8</mark>">
        <link rel="stylesheet" href="screen.css">
    <mark></head></mark>

## Even Tables

|  Locavore      | Umami       | Helvetica | Vegan     |
+----------------|-------------|-----------|-----------+
|* Fingerstache *| Kale        | Chips     | Keytar    |
|* Sriracha     *| Gluten-free | Ennui     | Keffiyeh  |
|* Thundercats  *| Jean        | Shorts    | Biodiesel |
|* Terry        *| Richardson  | Swag      | Blog      |

It’s good to have information organized.

## Pictures
{:.cover #Picture}

![](pictures/picture.jpg)

## **You can even shout this way**

## Inner Navigation

1. Lets you reveal list items one by one
2. …To keep some key points
3. …In secret from audience
4. …But it will work only once
5. …Nobody wants to see the same joke twice

## ![](http://shwr.me/pictures/logo.svg) [See more on GitHub](https://github.com/shower/shower/)
{:.shout #SeeMore} -->
