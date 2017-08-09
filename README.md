Research to bypass all adblockers like AdBlock Plus, uBlock, uMatrix, AdGuard and others.

Project Goal
========

List all mechanism to show how to defeat adblockers.


RoughTed 
========

Affected pages:
* Adf.ly
* ExtraTorrent
* Openloud
* Ouo.io
* .... (thousand others)


How it works?
========

The malicious code present in these rogue ads will load various scripts in the browser's background, which redirect the user through tens of URLs where various checks are performed.

The detection include checks for browser type, operating system, language settings, and geolocation information and a advance detection if th user argent info was faked.

These scripts range from using the now standard HTML5 canvas-based fingerprinting technique to a newer trick of checking for a list of installed fonts — which are different based on OS.


Protection?
========


Router (doesn't work 100%)

For a router to do this, it would have to be more than a router. To truly filter ads, you have to sit at the application level, layer 7. Routers sit at layer 3 and 4. To a router, ads and legit website traffic can come from the same IP address, making it impossible to differentiate between the two.


Regex detection (works 100%):


&tid=6[0-9]{5}&(status|red)=[0-9]{1,2}&(info|ref|subid|abt|v)



Top RoughTed domains
========

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
* baltimoresun.com
* boston.com
* calgaryherald.com
* calgarysun.com
* capitalgazette.com
* carrollcountytimes.com
* celebslam.com
* celebuzz.com
* chicagotribune.com
* chowhound.com
* citypaper.com
* computershopper.com
* courant.com
* csgoutpost.com
* ctnow.com
* cycleworld.com
* dailypress.com
* deathandtaxesmag.com
* delmartimes.net
* download.cnet.com
* edmontonjournal.com
* edmontonsun.com
* edmunds.com
* everydayhealth.com
* extremetech.com
* fieldandstream.com
* financialpost.com
* gamepedia.com
* gamerevolution.com
* geek.com
* gofugyourself.com
* growthspotter.com
* hearthhead.com
* hockeysfuture.com
* hoylosangeles.com
* ibtimes.com
* idigitaltimes.com
* infinitiev.com
* lajollalight.com
* leaderpost.com
* lifewire.com
* lolking.net
* mamaslatinas.com
* mcall.com
* metacritic.com
* metrolyrics.com
* mmo-champion.com
* montrealgazette.com
* nasdaq.com
* nationalpost.com
* orlandosentinel.com
* ottawacitizen.com
* ottawasun.com
* pcmag.com
* popphoto.com
* popsci.com
* ranchosantafereview.com
* ranker.com
* realclearpolitics.com
* redeyechicago.com
* sandiegouniontribune.com
* saveur.com
* sherd.com
* southflorida.com
* spin.com
* sporcle.com
* stereogum.com
* sun-sentinel.com
* tf2outpost.com
* thebalance.com
* thefrisky.com
* theprovince.com
* thespruce.com
* thestarphoenix.com
* thesuperficial.com
* thoughtco.com
* timeanddate.com
* tmn.today
* torontosun.com
* twincities.com
* vancouversun.com
* vibe.com
* wikia.com
* windsorstar.com
* winnipegsun.com
* wowhead.com
* wrestlezone.com
* zam.com
* 101greatgoals.com
* 4chan.org
* allthetests.com
* biology-online.org
* destructoid.com
* eurweb.com
* fullmatchesandshows.com
* grammarist.com
* jerusalemonline.com
* lucianne.com
* phonesreview.co.uk
* thefreethoughtproject.com
* veteranstoday.com
* walla.co.il
* yad2.co.il


Research:
* https://blog.malwarebytes.com/cybercrime/2017/05/roughted-the-anti-ad-blocker-malvertiser/
* https://github.com/gorhill/uBO-Extra/wiki/Sites-on-which-uBO-Extra-is-useful#instart-logic
