---
layout: page
title: "Philips TV"
description: "Instructions on how to add Philips TVs to Home Assistant."
date: 2016-11-01 13:00
sidebar: true
comments: false
sharing: true
footer: true
logo: philips.png
ha_category: Media Player
ha_iot_class: "Local Polling"
ha_release: 0.32
---


The `philips_js` platform allows you to control Philips TVs which expose the [jointSPACE](http://jointspace.sourceforge.net/) API. Instructions on how to activate the API and if your model is supported can be found [here](http://jointspace.sourceforge.net/download.html).

To add your TV to your installation, add the following to your `configuration.yaml` file:

```yaml
# Example configuration.yaml entry
media_player:
- name: NAME
  platform: philips_js
  host: 192.168.1.99
```

Configuration variables:

- **name** (*Optional*): The name you would like to give to the Philips TV.
- **host** (*Required*): IP address of TV.