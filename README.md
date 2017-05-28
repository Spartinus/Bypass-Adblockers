# Research to bypass all adblockers like AdBlock Plus, uBlock, uMatrix, AdGuard and others.

Project Goal
========

List all mechanism to show how to defeat ad-blockers.


RoughTed 
========

Affected pages:
* Adf.ly
* ExtraTorrent
* Openloud
* Ouo.io
* .... (thousend others)


How it works?
========

The malicious code present in these rogue ads will load various scripts in the browser's background, which redirect the user through tens of URLs where various checks are performed.

The detection include checks for browser type, operating system, language settings, and geolocation information and a advance detection if th user argent info was faked.

These scripts range from using the now standard HTML5 canvas-based fingerprinting technique to a newer trick of checking for a list of installed fonts — which are different based on OS.


Protection?
========


Router (doesn't work 100%)

For a router to do this, it would have to be more than a router. To truly filter ads, you have to sit at the application level, layer 7. Routers sit at layer 3 and 4. To a router, ads and legit website traffic can come from the same IP address, making it impossible to differentiate between the two.


Regex:


&tid=6[0-9]{5}&(status|red)=[0-9]{1,2}&(info|ref|subid|abt|v)



Top RoughTed domains
* histock.info
* charmstroy.info
* greatwork.info
* yoursinfo.info
* leversions.info
* modescrips.info
* beershavartb.com
* budgement.info
* octagonize.com
* contentpap.info


Research:
https://blog.malwarebytes.com/cybercrime/2017/05/roughted-the-anti-ad-blocker-malvertiser/
