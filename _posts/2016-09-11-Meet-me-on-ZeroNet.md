---
layout: post
title: "Meet Me on ZeroNet"
date: 2016-09-11
excerpt: "Revolution starts from Zero. Welcome to ZeroNet"
tags: [ZeroNet, torrent, play, bitcoin, bittorrent, internet]
feature: /assets/img/zeronet/feature.PNG
comments: true
---


## Hola ZeroNet

So, a new discovery. You can get bored of watching cute cat and dog videos. No kidding. And cat gif's just don't cut it anymore.  So you head back to torrent sites. And you see that blazing screen, that warning; the government is going to get you, or your favourite website has been taken down, never to come up again maybe? Sigh. So you work around the URL, look for alternative torrent sites, use a proxy? Oh, so you have exhausted all free trials on VPN services? The effort alone can drive you back to cat/ dog videos and articles like "blah blah, YOU WON'T BELIEVE WHAT HAPPENED NEXT!!!"

Enter ZeroNet. 

>>Open, free and uncensorable websites,
using Bitcoin cryptography and BitTorrent network

Boo yah. Try taking this one down. B)
Summing it up in three simple lines--

>>Uncensored:
It's nowhere because it's everywhere!

ZeroNet is decentralised, peer to peer web hosting. It doesn't follow the conventional client server model. With ZeroNet, you're the server, and you're the client. When you visit a website on ZeroNet, the web pages get loaded on to your system and you start hosting them as well. Quite similar to how torrent seeding works. The site remains live as long as it has at least one peer hosting it. And since there is no single server hosting it, it is impossible for anyone to take down. Imagine a scenario, where hundreds of people are dragged to court for downloading HTML and CSS files.
Not happening. And did I mention? You can also use ZeroNet with *Tor* and go completely anonymous.

>>No hosting costs:
Sites are served by visitors.

You heard that right. It's people like you and me who keep ZeroNet alive. You can have your website for free on ZeroNet in just a few clicks and also have your database. *Really? Let's get back to this later, shall we?*

>>Always accessible:
No single point of failure.

As long as there is even a single peer hosting a site, the site is accessible to anyone in the world. You can even view your visited sites ***offline***.  You don't even need Jio data packs now. :P

Then let's get to it. Head over to [ZeroNet](http://zeronet.io/) and download the *ZeroBundle*. It's as easy as they mention. Extract the contents of the zip anywhere on your drive and run *zeronet.cmd* (if you're on Windows, i.e.)
*Most of the links following this can only be viewed after installing ZeroNet*
And that's all. You can now start browsing zeronet in your regular browser.

![helloZero](http://nish-d.github.io/assets/img/zeronet/helloZero.PNG)

Use [ZeroSearch](http://127.0.0.1:43110/zerosearch.bit/) as a search engine, [ZeroMail](http://127.0.0.1:43110/Mail.ZeroNetwork.bit/) for all mailing purposes, and [ZeroId](http://127.0.0.1:43110/zeroid.bit/) to create a standard id to be used everywhere on ZeroNet. 

## Clone a Site

Now coming to the interesting part. Like any website you come across? Clone it, modify it and host it as your own.

![clone](http://nish-d.github.io/assets/img/zeronet/clone.PNG)

1) This creates a new folder in `..\ZeroBundle\ZeroNet\data`
for e.g. `ZeroBundle\ZeroNet\data\1MTpPDTJAB6YmNSeGKjfxrosD738tjnQVf`.  
Add your own changes if you wish to in the html/css files here.

![clone_2](http://nish-d.github.io/assets/img/zeronet/clone_2.PNG)

2) **1MTpPDTJAB6YmNSeGKjfxrosD738tjnQVf** is your website address. After you're done signing the `content.json` (content.json is used to convey to your peers the number and kind of files that are being used by your website) and publishing the site, it can be accessible to everyone on http://127.0.0.1:43110/1MTpPDTJAB6YmNSeGKjfxrosD738tjnQVf/

## Create your Site from Scratch

Unfortunately, Zeronet cannot run scripting languages, so you cannot use PHP or Ruby here. Only Html, CSS, Javascript and CoffeeScript. (Yes, you read that right. CoffeeScript of all. Sigh.) So if you have a WordPress blog that you would like to have on Zeronet, you'd better migrate to any static website generator like Jekyll, Hugo or Hyde. However, it is possible to have dynamic websites using ZeroNet's API, [ZeroFrame](https://zeronet.readthedocs.io/en/latest/site_development/zeroframe_api_reference/).

1) Navigate to `ZeroBundle\ZeroNet` folder in your command prompt and run the following.


    zeronet.py siteCreate

This will generate a private key for your website that should never be shared with anyone. This key is instrumental for publishing and/or making modifications to your site. All your peers have all the content to your website but cannot modify it without the private key. 

If you're not a python developer, chances are you may be missing some of the packages required by `zeronet.py` to run. Simply,

    pip install *missing_package*
    
If your command prompt does not recognise pip,
navigate to `Python[verno]\Scripts` and make sure you have pip. Run `pip install` from here. If you do not have pip, download and execute `get-pip.py'.

2) After running `siteCreate` you should see something like this:

![siteCreate](http://nish-d.github.io/assets/img/zeronet/siteCreate.PNG)

3)Now you can insert your index.html files, CSS and javascript files at your site address directory. To view your website in debug mode, shut down ZeroNet and start it again. 

    zeronet.py --debug
    
4) You can find your site in the list of visited websites on the left side of HelloZero. But this is only visible to you; it needs to be signed and published before the whole world can see it. So go ahead and repeat the same steps as before, 
provide a site title, description, sign and publish. This time, you will be asked to enter your private key, the one that was generated while creating the website. And voila!

5)You may not have any peers yet, so you can leave your site URL in the comments below or post them on ZeroTalk or ZeroMe.
It is possible to register your own .bit domain on ZeroNet with [Namecoin](https://www.namecoin.org/). This requires bitcoins which can be obtained for free, but more on those some other day.

While on ZeroNet do not forget to visit [my mirror site](http://127.0.0.1:43110/18hjYbktA2g8zb21u9JRkaJCudaRRR6oqT/). It's still not perfectly tailored for ZeroNet yet, but please do visit me. :D

**Last but not the least, the primary attraction, the best thing about ZeroNet are torrent sites that will never in their entire lifetime go down. Check out [Play](http://127.0.0.1:43110/1PLAYgDQboKojowD3kwdb3CtWmWaokXvfp)**

![play](http://nish-d.github.io/assets/img/zeronet/play.PNG)




