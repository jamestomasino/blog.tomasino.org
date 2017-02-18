---
layout: "post"
title: "Apples"
date: "2008-04-09"
author: "tomasino"
tags:
  - "Computers"
slug: "apples"
---

Last night I went shopping at the [Perimeter Mall][] just north of
Atlanta. I've been up in the area a few times, but I hadn't been inside
the mall yet. Last night, a friend and I had too much food at
[Cheeseburger in Paradise][] before walking off our fattness around the
swanky stores.

Most of the stores weren't very inviting; either selling kids clothes or
personal electrolysis kits. We had a little fun in the [EB Games][], but
as our game systems are mostly modded, we weren't really planning on
buying anything.

Then we came to the [Apple Store][]. It was a glorious, pearly haven of
electronic goodness, bountiful in innovation and style. Behind the
counter, the [Apple Geniuses][] were hard at work training and
explaining all the latest Mac concepts to the shoppers. Stepping inside,
we could feel the excitement. Customers swarmed around iPod touches,
MacBooks, new iMacs, and of course, the new MacBook Air.

![MacBook Air][]

It was our first time seeing the device in person. The commercials had
been a big hit, showing how thing and elegant the design was, but I
wasn't impressed. To me, thin meant fragile, stripped-down, even
backwards. Then we touched it.

I knew I was wrong right away. As I lifted the unit, I was as impressed
by how sturdy and solid it felt as I was by how little it weighed. Gone
were the days where the screen wobbles as you walk the laptop around.
The hinges held tightly as I closed and reopened it, noticing another
nice surprise. Apple had also removed the annoying push-button to open
the laptop. On my 12" PowerBook at home, that very switch has recently
being giving me problems. On the Air, you just lift from the recessed
notch and it's done.

With the outside examined, I wanted to put it to the real test. As I
moved my hand to the touchpad, I paused. It had been enlargened to a big
comfortable size. I could barely keep my excitement in. I'd been dying
to try this out for a while. Opening safari, I went to the first webpage
I could think of, this blog, and pinched my fingers together. Instantly,
the text size shrunk. I spread my fingers out and the text grew.
Multi-touch touch-pads may be the coolest thing since the hotdog was
invented.

Plopping my thick fingers onto the keyboard, I was in for another
surprise. The new keyboard design was fantastic! Rather than the shoddy
loose keyboard faceplate of the old PowerBook models, the Air had a
solid metal faceplate with large, unencumbered buttons rising up. No
tapered sides or miniature footprint here; this keyboard was solid, easy
to use, and comfortable.

I loved the keyboard so much, I wanted one right then and there. I
couldn't afford the 1799\$ pricetag of the Air, though, so I went the
easy route. I picked up the Apple Wireless Keyboard for use on my PC at
home.

![Apple Wireless Keyboard][]

Without going into too many details, let me just say it's amazing. The
smallest footprint you can imagine, with the feel of a full-size
keyboard. As I type this blog entry out on a big, clunky, monster of an
HP keyboard, my fingers feel dirty. They crave the AWK even now.

Setup had a cost, though. While I'm certain that integrating with a Mac
would have been simple, doing so with a PC had a few problems.

First, setting up the bluetooth connection was really problematic. I
purchased the [Kensington Bluetooth USB Adapter 2.0][] from Best Buy on
the way home. I followed the installation instructions, set up the
Bluetooth device, and turned on the Keyboard. My Bluetooth configuration
picked up the keyboard right away and knew exactly what it was, but when
I went to handshake and share pass-key to connect, the problem was
apparent. The screen told me to type in the PIN number on my keyboard
and press Enter, but there was no PIN number on the screen. After some
searching online, I found more information on [this forum][].

In the end, the solutions they presented helped lead me to my own
solution, even if they didn't work as stated. I downloaded an old
version of the Wildcomm Drivers (v. 1.4.2.10), as they suggested at one
point in the forum. The order in which I installed things was important.
After a few errors, I uninstalled everything and did the following. I
installed the old Wildcomm Drivers. Then when it asked me to plug in my
Bluetooth device, I plugged in the USB adapter. It popped up asking for
a driver. At that point, I had Windows search the driver CD for the
correct driver. When it finished installing, the Wildcomm install also
finished. After a reboot, I turned on the Keyboard and told Windows to
supply the PIN itself. Voila!

If that wasn't crazy enough, I had a new problem. The
<acronym title="Function">FN</acronym> button wouldn't work. That made
it very difficult to perform a CTRL-ALT-Delete. After a few more forums,
I found the solution via the utility, [AutoHotKey][]. I started with
[someone's][] prefabricated "Apple Wireless Keyboard" [script][], and
edited it to make the eject button into a delete button, which was my
preference. Now not only can I CTRL-ALT-Delete, but the keyboards media
keys work with [Winamp][] too!

All in all, I'd say the keyboard is downright fantastic. If you don't
mind messing with firmware and drivers a bit, or installing and
scripting some fancy hot-keys, this keyboard might be a good fit for you
too.

  [Perimeter Mall]: //www.perimetermall.com/
  [Cheeseburger in Paradise]: //www.cheeseburgerinparadise.com/
  [EB Games]: //www.ebgames.com/
  [Apple Store]: //www.apple.com
  [Apple Geniuses]: //www.apple.com/retail/geniusbar/
  [MacBook Air]: //blog.tomasino.org/images/apple-macbook-air.jpg
  [Apple Wireless Keyboard]: //blog.tomasino.org/images/apple-wireless-keyboard.jpg
  [Kensington Bluetooth USB Adapter 2.0]: //us.kensington.com/html/9403.html
  [this forum]: //www.neowin.net/forum/lofiversion/index.php/t285546.html
  [AutoHotKey]: //www.autohotkey.com/
  [someone's]: //www.autohotkey.com/forum/topic6367.html
  [script]: //brrp.mine.nu/fnkey/files/AppleWirelessKeyboard.zip
  [Winamp]: //www.winamp.com
