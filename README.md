Research to bypass all adblockers like AdBlock Plus, uBlock, uMatrix, AdGuard and others.


RoughTed 
========

Affected pages:
Adf.ly
ExtraTorrent
Openloud
Ouo.io
.... (thousend others)


How it works?
========

The malicious code present in these rogue ads will load various scripts in the browser's background, which redirect the user through tens of URLs where various checks are performed.

The detection include checks for browser type, operating system, language settings, and geolocation information and a advance detection if th user argent info was faked.

These scripts range from using the now standard HTML5 canvas-based fingerprinting technique to a newer trick of checking for a list of installed fonts — which are different based on OS.




Research:
https://blog.malwarebytes.com/cybercrime/2017/05/roughted-the-anti-ad-blocker-malvertiser/
