# Internet Routing: The Border Gateway Protocol

## Overview

In this assignment, we will learn about how Internet traffic travels between
Internet endpoints, or IP addresses.  There 

## Background

Internet traffic travels along paths between endpoints via intermediate
waypoints called routers. Each router looks at the destination IP address of a
piece of Internet traffic (called a "packet") and determines where to send
that packet next by looking at information it stores locally, in a structure
called a routing table.

This routing information is stored and passed between routers using technology
called a routing protocol. Routers on the Internet use a couple of different routing
protocols to exchange this information. Today, we will focus on the protocol
that independently operated networks (e.g., the University of Chicago, Google)
use to exchange information, called the Border Gateway Protocol (BGP).

Below we will explore some real-life Internet routing tables and learn more
about how this information is stored and updated.

## Activity

### Part 1: Exploring Internet routes with traceroute.

We will use a program called `traceroute` to see the router-by-router path
to an Internet destiantion. 
  
1. Open a terminal program on your computer. If you are using a Mac (as in the
   instructional lab), this is as simple as typing "command-space" and then
   typing in terminal and hitting enter. There are more sophisticated terminal
   programs, but the one that ships with your machine will suffice.
2. Type `tracroute google.com` and observe the output.
   - How many "hops" are there between your local network and the destination?
   - What is the round-trip latency to each hop?
   - What else do you observe?
3. Can you tell anything about the networks that your local network
   connects to? What "upstream Internet service provider" does the path use to
   reach the destination?
4. Repeat the above for other domains, such as `amazon.com` or `facebook.com`
   Also try an academic domain ending in `.edu` such as `stanford.edu`.
   - Are the upstream providers the same?
   - Do you always see responses? When or why might you not see a response?
   
   
### Part 2: Exploring the Internet routing tables.

5. Type `telnet route-views.routeviews.org`, which will bring you to a
   terminal prompt for a router. At the login prompt, type `rviews`.
6. Explore the outputs of the following commands:
    - `show ip bgp summary`
    - `show ip bgp neighbor`
   What do these commands show us?
7. Now look up a route for `google.com`. You can do so using the `show ip bgp`
   command, by typing `show ip bgp <IP address>` where you enter the IP
   address of `google.com`. (Remember how to get an IP address from the last
   lesson.) 
   - What information do you see?
   - Can you compare the information you see in the routing table from the
     information you see in the traceroute?
 
## Home Thought Question

Internet routes are continually changing.  If you want to see it in action,
type an Internet address or "prefix" into the interface at
[BGPlay](https://bgplay.massimocandela.com/).
