---
layout: post
title: Cheap Rotary Home Phone Using AWS SIP Trunking
---

A few months ago, I pulled a red Western Electric rotary phone from the shed behind my house and immediately decided that I had to set it up as a home phone for my housemates and me. It being 2024, I also knew that plugging it into the wall and signing up for POTS (Plain Old Telephone Service) with the local telephone office was not an option, so I began to scheme. My scheming took me for quite a loop before I realized that there is an easy solution that doesn't even require my engineering degree.

I initially assumed that I could commandeer the phone's microphone and speaker with some custom electronics and then hook it into the internet, designing a zany high-voltage circuit to control the ringer. My first task: figure out how it all works.

I found it surprisingly difficult to find a source on the internet describing how a telephone works. There are pleny of articles along the lines of, "...converts your voice into electrical energy...the wheel makes pulses as it spins..." But how do two wires carry two directions of communication plus ringing and dialing information? How does the telephone office detect if the phone is off the hook? What are the voltages and currents involved in ringing and talking? How does your voice end up at the other person's microphone and not your own? Finally, I found [this old website](https://www.epanorama.net/circuits/teleinterface.html), last updated in 2001, that clearly explained it all, and I was a little intimidated. Telephones use crazy 19th century analog wizardry to solve all of these problems with just inductors and capacitors.

Fortunately, during this search I also found that there exist cheap consumer devices called analog telephone adaptors (ATAs) which easily turn old phones like mine into VoIP phones. In cases like this, the best engineering decision is to do no engineering and just use the solution that somebody else perfected—especially when it just costs $20 on eBay. Not all ATAs would work with my phone's mechanical ringer and rotary pulse dialing. I chose a Grandstream ht801 after reading online that it supports pulse dialing and offers a high-power ringer output. Plug the phone into one end and ethernet in the other and POOF! your nonfunctional telephone is magically transformed into a nonfunctional VoIP telephone.

I actually created a problem by installing the adapter where the old telephone wiring originally entered the house. Now all the old phone jacks in the house were fully functional, which allowed me to justify hoarding old telephones and installing them all over the place. Since starting this blog post, I fixed up a 1930s Western Electric Model 202 and installed it in my room.

In order for the 

