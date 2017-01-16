Between Christmas and New Year's I decided to take some time off of work, spend some time with my friends and family, and relax at home. It was...great!

I didn't really have much of a plan. <a href="http://twitter.com/kezforprez">Amanda</a> and I took a trip to Long Island over the Christmas weekend, which was pretty packed with family visits and food eating, and then back in Brooklyn, we decided to just play it by ear.

At one point I realized I had a number of projects on my list that I thought I could tackle while on break and one of them was to start getting my "data" in order. It's a monumental project, and one that I will be writing about quite a bit over the course of 2017.

The data, is very much, out of order. It's everywhere. It's on my phone, it's on my old phone, it's on my laptop, and the laptop before that, and the three other laptops before that. It's backed up in places I no longer know about, it's on broken hard drives, thumb drives, SD cards, DVDs, CDs, Zip Disks, cloud accounts, Dropboxes, Google Drives, and oh yeah, there's a bunch of notebooks--that's data too.

I don't think I'm unique. In fact, I think most people are just like me--data basically everywhere, without any kind of a plan, or maybe better put, any kind of a realistic plan.

So, one of my "big projects for 2017" is to at least approach the problem with some kind of a plan and see where it takes me.

The first step in my plan (and this plan will evolve in real time) is to gather all the data in one place, and get it to be all "live." What I mean by that is, to power it up, put it on a computer somewhere so that I can easily access it, and start to deal with it.

To do this, I figured the easiest way to start would be to build a little home server, attach a big drive array and start pumping in all the data I can find. So, over the holiday break I decided to build a small home server out of an old Mac Mini I had lying around. It went pretty well, until it broke.

I tweeted my progress, which you can <a href="https://twitter.com/i/moments/814119107905908738">read about here</a>, but what is missing is the why part, which I will try and explain in this post. And then of course, the part where it all broke down and sent me basically back to square one--that part has yet to be explained as well. So here goes.

https://twitter.com/micahwalter/status/813971245834321920
<h3>Mac Mini</h3>
The computer I chose for this project was an old Mac Mini that had been sitting on my bookshelf, powered off, for a few years. It was a pretty nice machine in its day. Small form factor, HDMI display port. I think it was an early 2010 model, which I bought in the "server" configuration, which means it has twin 500Gig hard drives and 8 gigs of RAM. In fact, I bought this computer about 7 years ago to do basically the same thing I am trying to do with it now--build and run a home server.

Home servers have come a long way since I bought the Mac Mini. You can basically buy an off the shelf solution, complete with massive amounts of redundant storage and a built in operating system for a pretty nominal amount of money. But, I already had the Mini, and macOS was going to be part of the overall plan (more on that in another post next week) so I decided to see if I could resurrect the Mini and get it up and running without much expense.

It didn't take long to get the Mini working again. I used the <a href="https://support.apple.com/en-us/HT201314">Internet Recovery</a> feature to get a fresh install going, and then quickly upgraded it to macOS Sierra. This all seemed to work just fine, no glitches, no gotchas. I purchased the $20 <a href="http://www.apple.com/macos/server/">Sierra Server</a> app from the App Store and got that up and running pretty fast as well. Basically, within one evening, I had a fresh installed, working server waiting for me to tell it what to do.

I found a nice spot for it on top of a bookshelf in the living room, and wired up the <a href="http://www.drobo.com/">Drobo</a> S I had lying around. The Drobo S is a drive array I've had for about the same amount of time. It's got tons and tons of files on it, and usually is just lying dormant on the floor somewhere until I need something form it or want to copy some files to it for cold storage. I figured it would be the perfect storage solution as it always seems to work just fine, has plenty of room to spare and already has a large chunk of "the data." I plugged it in and it worked right away.

https://twitter.com/micahwalter/status/814109716196507648

I spent the rest of the time tweaking the server to make it do a few basic things.
<h3>I wanted it to:</h3>
<ol>
 	<li>Be a file server on the local network</li>
 	<li>Provide internal DNS so it would be easy to find on the local network</li>
 	<li>Be always backing itself up somewhere to the cloud</li>
 	<li>Maybe do some other fancy things some other day.</li>
</ol>
By the end of the day I had 1, 2 and 3 working just fine.

For 1 and 2, I just configured the Sierra Server options. It's pretty easy to do, and the hardest thing was understanding how the internal DNS should be set up so you can get to the local network as well as the external "Internet" without having to think about it.

https://twitter.com/micahwalter/status/814486454441246720

For 3, I chose to use Backblaze, which is a pretty easy to configure, backup everything, unlimited space, cloud backup solution. You just install it, and over time it backs up everything for a small amount of money. I use this on my laptop as well and it works great. I've used Crashplan and others in the past, but this is what I'm using now.

Everything was going perfectly smoothly. I found one issue which was that the Mac Mini and Sierra have a hard time when not attached to a monitor. That said, it works just fine, except for trying to do any screen sharing. So, I found this little device that plugs into the HDMI port and makes it think its plugged into a monitor all the time. This seemed to do the trick and screen sharing worked perfectly form that point on.

https://twitter.com/micahwalter/status/814589445701771264

Once it was basically all set up, I started work on the files. The first big project there was to set up an Apple Photos instance and start pumping in photos from the archives. I'll of course get into that plan in a future post, but it's just the very first step in a long line of steps to build what I am calling my "Penultimate Photo Archive."

I got Photos set up and started importing everything from 2003. The files were set to all live on the Drobo (One big Apple Photos Archive stored on the Drobo volume).

https://twitter.com/micahwalter/status/814614296382636032

It sat there and chugged along for a few days, and then all the sudden on the last day of the vacation it just stopped working. The computer switched off, and I haven't been able to get it working since. It will power up, but after a minute or so of going through the boot sequence, it just shuts itself off. From everything I've read online it looks like a drive failure. I'm sure it's repairable, but ugh... what a bummer!
<h3>Back to the drawing board!</h3>
Honestly, I'm not entirely sure what to do now. I suppose I could try and fix the server, reinstall macOS and basically start over. I could buy another Mac Mini, one that's under warranty and start from there, or I could go down the rabbit hole of trying to use something else, like an off the shelf NAS. Also, I could just plug my Drobo directly into the Airport Extreme so I could at least have access to the files, but I don't really want to do that. Gonna have to think the next steps through a bit before I make my next move. Till then... happy for any thoughts, feedback or ideas. ;)

Here's the Twitter version, which I created as a Twitter Moment, since that's a thing you can do now.

https://twitter.com/i/moments/814119107905908738