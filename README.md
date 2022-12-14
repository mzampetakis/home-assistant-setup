# Home Assistant Setup

The purpose of this repository is to expose the setup process and the functionality offered by the home assistant setup I am using and improving over time.

## Setup

The barebone of my smart home setup is based on a [Raspberry pi 4 model B (8GB)](https://www.raspberrypi.comproducts/raspberry-pi-4-model-b/) with access to the local home network. Raspberry pi runs a [Home Assistant Operating System](https://www.home-assistant.io/installation/raspberrypi)

Home Assistant (HA) Operating System is a minimal Operating System optimized to power Home Assistant. It comes with Supervisor to manage Home Assistant Core and Add-ons.

Basic setup of the OS is pretty straight forward and after a few [onboarding steps](https://www.home-assistant.io/getting-started/onboarding) HA will be up and running.

## Devices & Sensors

As soon as the HA OS is up and running some devices, such as the weather forecast, might be already present. From the Settings-> Devices & Services HA might have already some proposed devices to integrate.

A list of devices I have added can be found at the [Devices & Sensors](/devices-and-sensors) page.

## Custom scripts

In order to perform any custom operation within the HA various scripts can be integrated.In my case I have integrated a baric router management through a custom binary interface I have developed.Mor info about custom scripts integrations within the HA can be found at the [Custom Scripts](/custom-scripts) page.

## Automation

The automation part of the HA is the most interesting one. Using the automation functionality we are able to make things a bit "smart". It's the part where more than one devices and sensors can cooperate effectively to make our lives easier. The way that automations can be setup alongside some examples can be found at the [Automation](/automations) page.

## Configuration files

At the [configuration-files](/configuration-files) page, a list of the available configuration files I use can be found for reference.

## Add ons

HA OS supports various addons that allow the user to extend the functionality around Home Assistant by installing additional applications.

At the [addons](/addons) page there is a list  of the add ons that I have used in the past (or currently using) and find pretty useful
