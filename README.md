# webapp
Uniface 10 Responsive Web Framework/Starter Application

### Overview
A Uniface 10.3 responsive web/mobile application starter project created by David Akerman. 

#### Background
It evolved from the WebStart Uniface 9.7 project, and aims to provide a framework for DSP development addressing common
requirements such as Login, Navigation, Modality, Alerts etc.

#### Dependencies
Various UI resources are used. The can be loaded from an external Content Delivery Network (CDN) or downloaded separately:
- bootstrap 4
- jquery
- font-awesome

### Notes
The menu is driven by cfg\menu.json. If desired, it can be swapped with code using navsvc to build a JSON structure.
The resulting structure is used to dynamically create menu HTML in JavaScript.

### Installation and Configuration
Not currently documented in full!

Notes: 
- Some template configuration files can be found in the cfg folder
  - nav.json drives the menu
  - urouter.asn uses non-default Uniface installation locations so may need to be modified. 
  - add a #file to your Uniface common\adm\urouter.asn to include your project's asn\urouter.asn after modification
  - web.xml should be copied to your tomcat conf\CATALINE\localhost folder, and the location changes as needed
  - You may also need to modify web.xml to change Tomcat ports and locations.
  - Tomcat & URouter services will need to be restarted
