# Internet Privacy

In this hands-on assignment, you will learn a little bit about Internet
privacy, and some of the privacy risks associated with Internet traffic. We
will also learn a little bit about encryption and the ways to protect
ourselves from eavesdropping of traffic.

## Overview 

Internet traffic is sent in units of *packets*, chunks of information that
carry both the data itself, as well as various metadata about the traffic
(i.e., where it is coming from, where it is going to, how big it is, etc.).

All of that information can vcarry various privacy risks, including
information about what websites you are browsing, and (in the case of smart
devices) even more sensitive information such as when you might be home, awake
or asleep, and so forth. There are various ways to protect privacy, including
encrypting your traffic. Most web traffic is now encrypted, and even Internet
protocols like DNS are becoming encrypted.  Yet, simply encrypting traffic is
often not sufficient to protect privacy, because the metadata about the
traffic can also reveal sensitive information about activity.

## Activity

In this activity, we will use a tool called "Wireshark" to inspect network
traffic. We will first use Wireshark to inspect a traffic trace that we have
provided you.  We will then capture a "live" traffic trace of some web
browsing activity and explore what is visible in that trace.

### Part 1: Basic Wireshark Exploration

Let's first use Wireshark to explore a basic packet capture that we have
provided for you.

1. Open Wireshark.
2. Use Wireshark to open the provided packet capture file `nestcam.pcap`.
3. Answer the following questions about the trace:
    - How many bytes were sent in the trace?
    - To whom was the device communicating with, and when?
    - Can you tell, based on the activity patterns, when the device was more
      active? (Hint: Look at traffic volumes.)

### Part 2: Live Wireshark Packet Capture

We will now use Wireshark to perform a live packet capture of a Web download.
Because Wireshark will capture anything on your network interface, we'll also
need to use some display can capture filters to make sure we capture and show
only the traffic we are interested in looking at.

1. Open Wireshark again.
2. Find the option that allows you to capture traffic from the network
   interface that is sending and receiving traffic.
3. Set a capture filter, of the IP address of the website we will visit, as
   well as port 53 (which is DNS traffic).
4. Start the capture.

What can you learn about the web browsing activity from this capture?
    - What websites do you see?
    - Can you learn about other activities (e.g., when someone was browsing a
      site, how long they spent on the site, etc.)?

## Going Further

Repeat the above steps with encrypted DNS enabled.

Can you see the DNS traffic anymore? What types of privacy benefits might this
provide to you, as an Internet user and consumer.


