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

### Part 1: Exploring Internet routes.

1. Open a terminal program on your computer. If you are using a Mac (as in the
   instructional lab), this is as simple as typing "command-space" and then
   typing in terminal and hitting enter. There are more sophisticated terminal
   programs, but the one that ships with your machine will suffice.
2. Type `telnet route-views.routeviews.org`, which will bring you to a
   terminal prompt for a router. At the login prompt, type `rviews`.
3. Explore the outputs of the following commands:
    - `show ip bgp neighbor`
    - `show ip bgp`
4. 
   
### Part 2: How the DNS Resolves a Query 

## Home Thought Question


