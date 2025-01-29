---
date: 2025-01-29 01:18:59 +0000
title: "Plex"
tags:
  - plex
  - media
  - film
  - tv
---

{{< figure src="https://blog.tomasino.org/images/plex.png" caption="Plex Media Library" >}}

[Plex](https://www.plex.tv/) is a home media platform which lets you catalog and
manage your media. That is, your TV and movies, music, and some other stuff.
It's pretty smart. It knows about show seasons, airdates, organizes everything
for you into your own personal Netflix-style environment. You can then watch
that stuff on your computer, or with their apps available on smart TVs and game
systems, on your TV.

There's also a mobile app for Apple and Android devices. You can stream to your
phone. And if you're not home, you can stream it on your laptop while you're at
a comfy hotel.

Oh, and if you have friends on the platform, you can open up your media library
to them, so they can also stream your shows and films, or listen to your music.
And since they use their own account it will track their progress for them, and
not bother you and yours.

You get where this is going? It's pretty awesome. There's some other software
that does this too, notably Jellyfin, an open-source project that's very
similar. But Plex is the current king, and it has some really killer features
I won't get into in this post.

What I wanted to document a little bit here, on my non-technical blog, is the
rather ridiculous setup I have for acquiring media. Lets just say right away
that everything else I describe below is to acquire digital copies of things
I own in physical format already. Got it? Cool. Just pretend with me and we'll
move along.

Lets pretend that I wanted to find a digital backup copy of Batman (1989) to go
along with my VHS tape. It'll be easier to watch it streaming to my phone that
way. There's a lot of ways to acquire that online, the most popular being
torrent sites. I could search around for a torrent site, search for the movie,
and hope the version I get looks like it's good quality and it's a decent file
size. But that's a lot of work! What if it's not on the first torrent site? What
if it is, but only in a low quality? Or the filesize is too big. Or it's in
French? This stuff happens all the time, and it's annoying. Finding stuff is
hard. I've just been talking about films, but imagine TV shows. How do you know
when a new episode comes out? Finally, there's other ways besides torrents to
find things and they have their own challenges.

So what do I do? I use **Prowlarr**, an index manager. It's entire purpose is to
search stuff for me according to rules I set up. I tell it the quality I want
(DVD is good enough for me. I don't need Bluray). I tell it the language I want
(original, no dubs). I tell it a list of a bunch of torrent sites it can look
at, and other places too. It gets to be very smart for me so when I tell it to
find something it can do it automatically. Cool, right?

It's a start. That's fine for searching, but how do I know what to search for?
For TV shows I have another program called **Sonarr** and for films one called
**Radarr**. They're trackers. I tell them I want to watch the Golden Girls, and
they tell Prowlarr all about the episodes to go search for. Or I tell Radarr
that I want to see the newest Godzilla film (which I will totally own already!)
and it watches for when it is released on video or streaming so it can tell
Prowlarr to begin the search.

So that's it, right? Well, no. Now we're tracking and we're searching, but we're
not *ahem* acquiring just yet. I need some downloaders for that. I won't bore
you with the names, but yes, a torrent program is involved, as is another
technology that I'm not even going to try to explain here except to say it's
more than a decade older than the world wide web. There's a lot of tech stuff
that goes into this part of the puzzle, and it's pretty boring. Just trust me,
they take the info Prowlarr finds and actually uses that to download things.

And then we're done! Nah... See, Sonarr and Radarr then can tell the downloader
information to rename the file and sort it right into my Plex library. Pretty
names, folder structures, etc. Everything is nice and organized, and Plex is
automatically updated. Huzzah!

So we're---hold your horses! I said earlier I like original language things.
That means I'm going to need subtitles. And that means I need something to go
search and fetch those for me. This is yet another program called **Bazarr**.
It's configured with the language I want and it integrates with Radarr and
Sonarr to automatically queue up things that they download. Subtitles also get
shoved into Plex, and we're finally good to go.

Except, how do I tell these tools what I want to add later on? There's a few
tricks here. Sonarr and Radarr can be set up so that anything I add to my
"Watchlist" in Plex will get added to their queue. I also use a website called
[Trakt](https://trakt.tv) to track my watching habits and rate things. It's like
letterboxed does for movies, but it works for both movies and TV shows. I tell
Sonarr and Radarr that anything in my Trakt "To watch list" should get queued up
too.

So there we have it. I can just tell my media library what I want and it'll show
up automatically for me. Nice, right?

But!!! What if you're my friend and you want something to be in my collection
that you can see? Well, I have one last tool called **Overseer** that integrates
with ... well everything above. It's a discovery tool, and you can log into my
copy of it via your Plex login, if you have access to my Plex. Then it does some
cool magic. It looks at your Plex watch history on my server and offers
a discovery service. It'll recommend things based on your history. If you want
something you can click it to request it. That can be set up to send me the
request to approve, or just auto-approve. From there it's just like I had added
it myself. Into the queue and onto Plex.

It's a pretty silly level of setup, and everything beyond "install plex" is not
for the non-technical person. It's a fun set of toys to me, and I get a kick out
of the notifications I get--HOLD YOUR HORSES!! Notifications!

Right, so all those tools are working quietly in the background of my computer,
but how do I know what's going on? They all integrate with a number of
notification systems, from email to whatsapp to my choice, **Pushbullet**.
I have Pushbullet set up on my computer and phone, and whenever one of these
systems does a thing, it lets me know with a push notification everywhere.

Right, so I get a kick out of those notifications. They make me feel all fancy.


<!--  vim: set shiftwidth=4 tabstop=4 expandtab: -->
