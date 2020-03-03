# [OMSP-INFO-05] Web Browser
## Description
Numerous models of vehicles begin to bring built-in web browsers implemented by manufacturer with which users can surf the Internet freely. In general, these browsers are usually based on Chromium, and allow the user to connect as if they were in front of a computer.

However, some manufacturers have limited browsers for obvious cybersecurity purposes, for example, preventing local IP addresses from being visited, so that internal vehicle resources cannot be accessed like connected assets (cameras, microphones, etc).

![OMSP](/images/webbrowser.JPG)

Example: Tesla Webbrowser (Chromium)

## How to Test
In this control, the characteristics commented above should be reviewed, in order to validate that the user cannot take advantage of the freedom of these browsers to manipulate the vehicle configuration, extract information or deny the service.

**Browser settings**
* Browser settings should not be accessible by requesting links like `about:config` or `chrome://components/`

**Local resources resolution**
* Network aliases and IP access should be disabled to prevent access to local resources.

**Plugins**
* Installation of plugins should be disabled. If any plugin is needed, it must be preinstalled by the manufacturer or developer.

**Updates**
* Browser version should be the latest one in order to prevent from any 0-day or vulnerability found in the browser.

## Tools


## References
