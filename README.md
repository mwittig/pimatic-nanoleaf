# pimatic-nanoleaf
Simple Nanoleaf plugin for <a href="https://pimatic.org">Pimatic</a> using <a href="https://github.com/darrent/nanoleaf-aurora-api">nanoleaf-aurora-client</a>

## Status of implementation

This version supports the following
* Turn on and off aurora light

## Plugin Configuration

Plugin section:
```
    {
      "plugin": "nanoleaf",
      "active": true
    },
```
    
 Device section:
``` 
    {
      "IP": "<IP>",
      "Token": "uZ4UKQ05jkFCn6jllYjOo8srMUGuIXgB",
      "id": "Nanoleaf",
      "name": "Nanoleaf",
      "class": "LightAurora",
      "Interval": 3000
    }
 ```
  
## How to get API Token
1. Press the Power Key on your Hub for 5-7 sec. until the yellow light is blinking.
2. Do a post request to the following link (using Postman or something similar):
http://192.168.178.48:16021/api/beta/new 
3. You should find the Token in the body section.

## To do
- Add a dimmer 
- Add a colorpicker
- Add a effectpicker 
