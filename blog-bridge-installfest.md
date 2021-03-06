###date###

<a id="bridge-installfest">A BSD-focused Tor Bridge Installfest</a> by gman999

This disturbing picture of the [Tor bridge operating system monoculture](https://torbsd.github.io/oostats/bridges-os-count.txt) should frighten everyone.

No exaggeration intended, but when only one operating system kernel is responsible for the vast majority of censored traffic entering the Tor network, alarm bells should sound.

__TDP__ is looking to attack this problem on the local level with hands-on Tor installfests on the BSDs.

One could get online commitments from all over to wear a blue shirt on the first Tuesday of the month, to stop using salt on kale or to run a Tor bridge on a BSD variant, but those calls generally evaporate on the internet. It's time to start doing physical sessions to gather the hardware, do the Tor configuration and ultimately start changing the bridge operating system count.

__TDP__ is organizing a Tor bridge installfest in New York City in the fall.
 
The meeting will be introduced with a quick overview of Tor and the role of bridges, with a glance at the current [statistics](https://torbsd.github.io/oostats.html).

To make the event fruitful, users need to do some prepatory work coming into the installfest.

* Get your small and quiet thin client, an [APU2 from PCengines.ch](http://pcengines.ch/apu2.htm) or maybe a [BeagleBone Black](https://beagleboard.org/black) to move beyond the x86/Intel monoculture.

* Install your preferred BSD on the hardware, but keep it lean and small. For FreeBSD users [/etc/src.conf](https://man.freebsd.org/src.conf/) can be your friend. Minimize startup daemons and build this as a single-purpose system.

* In some parts of world bandwidth is underutilized. For those with FIOS or regular cable connections in a place like New York City, it's likely that your connection is quiet, even if the providers are being deceptive about the true bandwidth of residential connections. Decide how much bandwidth to dedicate to the bridge. Setting _RelayBandwidthRate_ in the torrc to 5000 or 10000 KB will probably go unnoticed by you, but could be lifeline to users blocked from the Tor network.

* If the bridge will be behind a firewall or NAT, figure out how to forward a TCP port to it. The bridge should have a static [RFC1918](https://tools.ietf.org/html/rfc1918) IP address, like 192.168.1.20.

The NYC event will be followed up by a planned IRC sessions for those wanting more feedback and discussion once the bridge is up and running.

Take this model of a *BSD Tor bridge installfest and replicate in your own locale or as a birds-of-a-feather session at an upcoming BSD conference.

In the coming weeks, we'll blog a suggested approach to the installfest, with all the all the details covered to ensure a successful event.

Consider this installfest open-sourced and ready to hack and replicate.

Let us know how it goes.
