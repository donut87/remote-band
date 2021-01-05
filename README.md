# Problem
As many many people we as a band faced issues with the Corona pandemic. Since this is a hobby project for all of us and we did not even had a gig yet, the problem is much smaller for us than for professional or semi professional bands. But still, we faced the situation, that we could no longer meet in our rehearsal room and make music together, which we usually quite enjoy. Also we were on track on getting our first songs together for playing small gigs on stage in 2020.

We are a band of 5 people with 3 of us working in IT, so we pretty earlier set out to find a solution to our problem.

# Solution

### What we wanted
An easy to use solution for all of us (vocals, guitar, guitar, drums, bass) to make music together online.

The solution had to be easy to use, because (as said earlier) we are 3 out of 5 working in IT and driving around giving IT support and installing everything was out of the question. Everybody had to be able to do the setup with minimal to no help.
### First ideas
 - Skype
 - discord
 - ...

All of these platforms match the easy-to-use criteria, but are not good for playing together and there is a simple reason: latency.

#### Latency
Playing together means, that everybody has to listen to everybody else. Even the drummer! So if the signal needs 300ms to travel from dummer to everybody else, everybody reacts to that and it then needs another 300ms to travel back to the drummer, rehearsing is not going to work.
So, latency is a key factor in music.
But the major platforms for online communication use 'high' latency for a reason. This way, background noises, feedback, echo and stuff like that can be filtered much easier and synchronizing all participants gets possible. Also ~300ms is fine for meetings and 1:1 talks. Just not for music.

There had to be another way. We couldn't probably be the first ones looking into this.

### Possible Softwares
We weren't. There are plenty of softwares, that promise you online distributed rehearsal, instrument teaching, recording and jamming. A few that pop up early in any online search are Ninjam (complex), JamKazam (closed source), Bandlab (commercial), eJamming (register first on website), Jamulus (FOSS, but seemed very basic)

So our Journey began :-)
#### April
After having a look over various possible solutions (and grabbing our gear from our rehearsal room) we opted for JamKazam. JamKazam has a central server, that the people behind JamKazam fully own. Which was fine for us, as we got the idea, that this was not easy and better left to people who know their stuff.
Features:
- Configure Audio input with gear latency measurement
- Audio chat
  - nice for communication between songs
- Set volume and balance for each participating musician
  - really handy to have distribute instruments to left and right
  - adjust volume of everybody to your needs (tune out singer 😉)
- Insert audio track file
  - This would be the key killer feature, but we didn't know that at first

It seemed to offer all we needed and was easy enough to use. If only that was the whole truth.

Our drummer did not even get to register through the Client software, as no connection to the server could be established. We figured, through various screen sharing session via Skype and even VNC, that his router was configured very strictly. Not necessarily a bad thing, but he lost his admin password. So we had to start without him.

Being short of a drummer, we were glad about the audio track, as all our songs are well written down using GuitarPro. Exporting the drum tracks as wav file was easy and so rehearsal could start.

If it wasn't for latency again 🙈. This time from our singer. His situation at that point was a WiFi bridge and a rather shitty ISP. So latency was between 300 and 1200ms. We kind of tuned him out...

It was not much, but we still hoped, that this would all be over soon.
#### May
It was not over soon...

To solve at least the WiFi bridge problem, we bought a [long CAT-6 network cable](https://smile.amazon.de/dp/B00EOTHDWQ/). This had to go through the garden into the main house. He lives in a the renovated garage, so they even dug up the ground and buried the cable. So latency was better. Still not perfect, but better most of the times.
We were still lacking a drummer, but we could not do anything about that.

#### June through September/October
- Back in rehearsal room

#### November
- Back with JamKazam
- it now sucks
  - Microfone from one of us, no longer works (robo/darth vader sounds)
  - loses settings from week to week (one gets really skilled in setting this up)

#### December
- JamKazam still sucks
- but now a monetization is announced
  - we are not happy
- fiddling with Jamulus and the public servers
  - but public servers are... yeah... public...
  - Solution: Host server at home (raspi or other dedicated pc)
  - Problem: Default routers from ISP are shitty
  - Next idea: Let's rent a vServer
    - works!
    - latency: 35ms default Ubuntu 20.04
    - low latency kernel: 25ms
