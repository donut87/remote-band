# Problem
As many many people we as a band faced issues with the Corona pandemic. Since this is a hobby project for all of us and we did not even had a gig yet, the problem is much smaller for us than for professional or semi professional bands. But still, we faced the situation, that we could no longer meet in our rehearsal room and make music together, which we usually quite enjoy. Also we were on track on getting our first songs together for playing small gigs on stage in 2020.

We are a band of 5 people with 3 of us working in IT, so we pretty earlier set out to find a solution to our problem.

## Disclaimer

We briefly discussed, meeting anyway, as we were pretty sure, no one would be prosecuting us. Everyone was kind of relieved, that no one really wanted to opt for this path. This proved to be the first "Corona character test" for all of us, I guess.
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
#### Mid March
After having a look over various possible solutions (and grabbing our gear from our rehearsal room) we opted for JamKazam. JamKazam has a central server, that the people behind JamKazam fully own. Which was fine for us, as we got the idea, that this was not easy and better left to people who know their stuff.
Features:
- Configure Audio input with gear latency measurement
- Text chat
- Audio chat
  - nice for communication between songs
- Video Chat
  - Seeing each other is nice!
- Set volume and balance for each participating musician
  - really handy to have distribute instruments to left and right
  - adjust volume of everybody to your needs (tune out singer 😉)
- Insert audio track file
  - This would be the key killer feature, but we didn't know that at first

It seemed to offer all we needed and was easy enough to use. If only that was the whole truth.

To test JamKazam the 3 IT guys registered, and tried to start a session. Keep in mind, this was the beginning of the restrictions and it seemed musicians from all over the world were trying to find solutions and lots of them tried to start a session with the very same tool. With some frustration we gave up and met again a week later to try again. This time it kind worked for us 3. Latency was around 40 to 60ms. We could work with that!

Our drummer did not even get to register through the Client software, as no connection to the server could be established. We figured, through various screen sharing session via Skype and even VNC, that his router was configured very strictly. Not necessarily a bad thing, but he lost his admin password. So we had to start without him.

#### April
Being short of a drummer, we were glad about the audio track, as all our songs are well written down using GuitarPro. Exporting the drum tracks as wav file was easy and so rehearsal could start.

If it wasn't for latency again 🙈. This time from our singer. His situation at that point was a WiFi bridge and a rather shitty ISP. So latency was between 300 and 1200ms. We kind of tuned him out...

It was not much, but we still had some hope, that this would all be over soon.
#### May
It was not over soon...

To solve at least the WiFi bridge problem, we bought a [long CAT-6 network cable](https://smile.amazon.de/dp/B00EOTHDWQ/). This had to go through the garden into the main house. He lives in a the renovated garage, so they even dug up the ground and buried the cable. So latency was better. Still not perfect, but better most of the times.
We were still lacking a drummer, but we could not do anything about that.

#### June
Not much rehearsing going on. We had more important things to do. Hard to believe, but getting married was more important for on of our guitarists (groom) and the bassist (best man).

#### July through September/October
Since we live and rehearse in Berlin, we got to see each other again over the summer on our rehearsal room. We once again had a drummer!

#### November
Covid struck again. The anticipated 2nd wave was there and we were once again at home. One major thing improved compared to spring:
Our drummer did reset his router and was able to register.

Unfortunately, connecting his e-drum set to a computer proved to be a challenge. So we were back with JamKazam, no drummer and a slightly lacking vocalist. But even that improved, as he switched ISPs.

Unfortunately, JamKazam got worse with every update and updates came weekly.

Some of us had to reconfigure the audio setup each week and the chat microfon of our guitarist and bassist was not usable anymore.

Nevertheless we carried on, using discord in parallel for chatting.

Lesson learned: Mute your discord mic, or your band colleagues will hear your "unplugged" sound next to your real sound, with some latency.

#### December

##### Drummer finally joins, JamKazam gets worse
JamKazam still did not get much better, but our drummer geared up and was able to join us in our weekly sessions. We had live drums. Oh the glory and joy. Ask his neighbours. Turns out, even an e-drum can make too much noise.

Now that we finally felt, we had a more or less stable solution at hand, an announcement from JamKazam came in. Beginning in 2021 they will start charging money for using JamKazam. We looked at the plans they offered. Between the 4 plans free, silver ($4.99/month and person), gold ($9.99/month and person) and platinum ($19.99/month and person) the gold option would have been the one to continue the way we rehearsed through the year.

As I said, we are 3 people working in IT and two of us are software developers. So paying for software is fine. As long as it is worth it. Since not all of us got through the pandemic without losing jobs/income we even would be able to distribute the 50$ among the others. Paying for a service is really not the problem. Paying 50$ for a service that got worse every time on the other hand, was not in our interest.

##### The Search for another tool
So it was time to revisit the list of alternatives. If only we had saved that list somewhere. So back to zero and search the internet once again.

Online search was faster this time, because we had a better idea of what we were looking for and the tool of our choosing was [Jamulus](https://jamulus.io/).

Features and perks:
- Configure Audio input
  - more basic than JamKazam, but still good enough
- Set volume and balance for each participating musician
- Overall Latency measurement
  - ping to server
  - overall latency
- Multiple open servers available
- Text chat
- Configure buffer size
  - So you can decide what is more important quality or speed.
- FOSS (GPL 2.0)
  - [Repo](https://github.com/corrados/jamulus)

Audio chat is a missing feature, but since we had to work around that before, it wasn't a big issue. Also uploading a wav file and playing it to everyone does not work, but our drummer has joined the online party so, this was also not a big issue.

##### Testing on a public server
Public servers are public. So anyone can join. For a quick test this was fine, as there are empty servers out there, if you are lucky. Along the way some people joined, but we quickly muted them and as soon as they got, that we were not trying to jam with strangers on the internet, we could try this out.

Unfortunately the connection of our bassist was so bad, Jamulus seemed to be unusable. The issue was already visible with JamKazam, but got worse with Jamulus. Best guess: Jamulus server did more compression because of slow internet connection.

##### Private server and a faster connection
Switching ISPs did the trick again. Ping and bandwith improved massively for our bassist and we had our last rehearsal with JamKazam on 29th of December. After that we had to have a new solution.

So we decided against one of us hosting this at home, configuring port forwarding, sharing his current IP address with the band, and everybody connecting after copying the address in the to Jamulus client. It should be easy to use 😉. Only other solution was to rent a server. Since renting real hardware in some data center is expensive (we were kind of on a 50$/€ budget), we decided to try out a vServer, which are very cheap compared to bare metal servers. Having a budget of 50€ meant we could choose from a variety of providers and basically all plans. To not jeopardize the mission by being cheap, we opted for a 4 core vServer with 8GB RAM from 1&1/ionos for 16€/month. Turns out, these are some Intel Xeon Gold 5120 CPUs working there and it is of course a vmware machine.

##### Installing Jamulus
Installing Jamulus is actually pretty easy, if you are familiar with linux and/or docker. You can install this directly to the system or just start up a [docker container](https://hub.docker.com/r/grundic/jamulus). Since starting up a docker container is fairly easy, I tested this. It also comes with a nice [docker-compose](https://github.com/grundic/jamulus-docker) file. The result was a little bit astonishing. Connecting to my server was easy enough after configuring the 1&1 firewall to open port 22124 and there it said overall latency 60ms with 25ms on my behalf (network plus hardware latency). Not bad!
Reading through the documentation of how to run your own server and the [Linux how-to page](https://jamulus.io/wiki/Installation-for-Linux), I decided to opt for a low-latency-kernel. Result: 50ms! Down 10ms.

##### First real band rehearsal with Jamulus and private server
Although the Jamulus wiki clearly states "Close every application, that deals with sound or internet!", we met at discord and Jamulus and started playing. Worked like a charm.

The vServer is vastly oversized. I had htop open the whole time and the load average did not even make it over 0.5 and not even 600MB RAM were used. So we might scale down to half the size, which will reduce costs by half.

### Lessons learned

1. Jamming, rehearsing event teaching instruments is possible.
2. Good internet connection is a must have
3. Quality gear makes your life easier
4. Do not give up!
5. It is still much more fun in person
