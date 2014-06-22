Capture the Flag
================

Capture the Flag is a sample application demonstrating the use of Nokia X
services on Nokia X software platform: HERE Maps, Nokia Notifications and Nokia
In-App Payment. The application also implements the corresponding Google APIs
and utilises them when the same APK file is installed on a Google services
enabled phone. The detection of services is done run-time. OpenIAB is used to
implement the in-app payment feature.

The app itself is based on the traditional outdoor game where two teams each
have their own flags, which the opposing team then tries to capture. The flags
in the game are randomly placed on the map within a fixed distance of the
player creating the game. The team who manages to get to the flag of the
opposing team first wins.

![Main menu](https://raw.github.com/nokia-developer/capture-the-flag/master/doc/screenshots/ctf_screenshot_1_small.png)&nbsp;
![Offline game ongoing](https://raw.github.com/nokia-developer/capture-the-flag/master/doc/screenshots/ctf_screenshot_2_small.png)

This demo application is hosted in GitHub
(https://github.com/nokia-developer/capture-the-flag) where you can find the
source code and documentation of the latest release.

Visit the project wiki for documentation:
https://github.com/nokia-developer/capture-the-flag/wiki

Offline documentation is provided with this project in `doc` folder.


How to set up and build the project
-------------------------------------------------------------------------------

**Dependencies**

The example is dependent on the following libraries, which are provided with
the project:

* *AndroidAsync* is a low level network protocol library. The project is
  hosted in GitHub: https://github.com/koush/AndroidAsync
* *HERE API library* (`com.here.android.sdk.jar`)
* *Nokia Notifications helper library* (`push.jar`)
* *OpenIAB* provides cross-platform in-app payment functionality and
  encapsulates both Nokia In-App Payment API and Google In-App Billing API.
  The project is hosted in GitHub: https://github.com/onepf/OpenIAB

In order to build the project you will also need Google Play services library.
The library can be installed via Android SDK Manager (*Extras* -> *Google Play
services*).

**API keys and IDs**




Game server
-------------------------------------------------------------------------------

To play the online version of the game, a server is needed. The server software
is provided with the project, see
[`/server`](https://github.com/nokia-developer/capture-the-flag/tree/master/server).
The software is implemented utilising node.js and socket.io library. To test
the server, you can use free server services such as
[Heroku](https://www.heroku.com/) or [Cloud9](https://c9.io/). For more
information see the
[README](https://github.com/nokia-developer/capture-the-flag/blob/master/server/README.md)
for the server software and the
[project wiki](https://github.com/nokia-developer/capture-the-flag/wiki).


License
-------------------------------------------------------------------------------

See the license text file provided with the project. The license is also
available online at
https://github.com/nokia-developer/capture-the-flag/blob/master/License.txt


Related documentation
-------------------------------------------------------------------------------

* [Nokia X Developer's Library](http://developer.nokia.com/resources/library/nokia-x)
    * [Nokia In-App Payment](http://developer.nokia.com/resources/library/nokia-x/nokia-in-app-payment.html)
    * [Nokia Notifications](http://developer.nokia.com/resources/library/nokia-x/nokia-notifications.html)
    * [HERE Maps](http://developer.nokia.com/resources/library/nokia-x/here-maps.html)


Version history
-------------------------------------------------------------------------------

* Version 2.0: One APK solution update - Maps/location, notifications and in-app
  payment services selected run-time based on which services are available on
  the phone (either Nokia X or Google services).
* Version 1.0: The initial release.
