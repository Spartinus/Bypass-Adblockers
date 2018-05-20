## Research to bypass all adblockers like AdBlock Plus, uBlock, uMatrix, AdGuard and others.

[![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/fold_left.svg?style=social&label=Follow%20%40CHEF-KOCH)](https://twitter.com/FZeven)
[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/CHEF-KOCH)
[![Discord](https://discordapp.com/api/guilds/204394292519632897/widget.png)](https://discord.me/NVinside)

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

These scripts range from using the now standard HTML5 canvas-based fingerprinting technique to a newer trick of checking for a list of installed fonts — which are different based on your installed OS.


Detection
========

Based on the research papers. 

* Alexa top-10K list and are able to detect anti-adblockers on 30.5% websites. From manually checking one third (1000) of these detected websites.

* The ﬁlter lists are maintained by a group of volunteers through informal crowdsourced feedback from users. As expected, adding new rules or removing redundant rules in the ﬁlter lists is a laborious manual process and is prone to errors that often result in site breakage.

* In sum, adblockers currently are simply not effective against anti-adblocking. For example, prior work showed that adblockers remove less than 20% of the adblock detection warning messages shown by anti-adblockers.

* Some solutions (e.g., BlockAdblock) utilize eval to wrap their anti-adblocking logic represented as a string
most websites choose to outsource anti-adblocking to dedicated third-party anti-adblocking service providers such as PageFair.

*  Analytics and ads scripts by Google are the most popular source of anti-adblocking scripts. Several other online advertising services such as Taboola and Outbrain using anti-adblockers.

* Some scripts use the “pixel” technique, which loads a small, unobtrusive piece of image (i.e., pixel) and then drops a browser cookie for future inter-domain ad re-targeting.

* Adblockers are currently struggling to keep up with anti-adblockers due to the challenges in manually analyzing the anti-adblocking Javscript. There is simply no guarantee. 

* I anticipate escalation of the technological battle between adblockers and anti-adblockers — at least in the short term. From the perspective of security and privacy conscious users, it is crucial that adblockers are able to keep up with antiadblockers. Moreover, the increasing popularity of adblocking has already led to various reform efforts within the online advertising industry to improve ads (e.g., Coalition for Better Ads, Acceptable Ads Committee) and even alternate monetization models (e.g., Google Contributor, Brave Payments). However, to keep up the pressure on publishers and advertisers in the long term, I believe it is crucial that adblockers keep pace with anti-adblockers in the rapidly escalating technological arms race.



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
* https://palant.de/2017/04/19/is-undetectable-ad-blocking-possible
* https://sites.google.com/view/antiadb-proj/
* https://blog.malwarebytes.com/cybercrime/2017/05/roughted-the-anti-ad-blocker-malvertiser/
* https://github.com/gorhill/uBO-Extra/wiki/Sites-on-which-uBO-Extra-is-useful#instart-logic *[ref](https://github.com/sindresorhus/devtools-detect)
* [EasyList: Ad-serving domain removed due to DMCA takedown request](https://news.ycombinator.com/item?id=14978228)
