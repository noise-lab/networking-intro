# The Domain Name System

## Overview

In this assignment, we will learn more about the Internet's Domain Name System
(DNS), the protocol and system that maps Internet names (e.g. www.cs.uchicago.edu) to
IP addresses (e.g. 128.135.24.72).

You will look "under the hood" at the Domain Name System using a tool called
``dig'', which allows us to issue domain name queries directly and see what
the responses are, as well as what information is contained within the
response. As we look at those responses, we will also come to understand how
devices connected to the Internet, such as your phone and laptop, make use of
this information, as well as how the DNS is used to build efficient
distributed systems on the Internet.

## Background

The Internet's DNS is much like a phone book, which maps names to phone
numbers. Similarly, the DNS maps names to IP addresses. Almost every
connection your device initiates to an Internet destination originates with a
DNS query. Thus, when you load a web page (as we did in the last assignment),
a single web page may involve tens to hundreds of DNS lookups.

When your web browser uses the DNS to look up names, it receives responses to
each of them in the form of an IP address. For large distributed services
(e.g., Google, Netflix, Amazon, Facebook), that IP address may differ for
different clients. For example, the person next to you may receive a different
IP address than you do. Certainly, as we will see below, if you issue a DNS
query from a different location, you're almost certain to receive a different
IP address.

Below we will explore some of these phenomena.

## Activity

1. Open a terminal program on your computer. If you are using a Mac (as in the
   instructional lab), this is as simple as typing "command-space" and then
   typing in terminal and hitting enter. There are more sophisticated terminal
   programs, but the one that ships with your machine will suffice.
2. Type `dig uchicago.edu` and look at the output.
   * There is a line with an IP address. What is the IP address?
   * The `A` letter next to the IP address indicates that this is an "address"
     record, in other words an IP address. There are other record types. 
   * What does the number on the same line next to the A mean?
3. Type `dig MX uchicago.edu`; how does the record differ? What do you
   think this record type is used for?
4. Now type `dig NS uchicago.edu`. These records are called
   "authoritative name servers" for the domain, in other words the servers
   that are responsible for resolving any domain name in the `uchicago.edu`
   domain. How do you think your browser would find these servers? 
5. Type `dig +trace uchicago.edu`. This "trace" provides the complete set of
   DNS lookups that your browser would issue to resolve the domain name
   `uchicago.edu` to an IP address. How many lookups are performed? How long
   does each one take? Imagine that when loading a web page, you'd need to
   load hundreds of objects. How could this process be sped up?

Below are some more questions we can explore in class together that build on
these initial experiments.

## Questions

Now repeat these steps above with `amazon.com` or another domain name of
your choice.  How do the results differ?

## Home Thought Question

If you have Virtual Private Network (VPN) software, you know that part of what
that software does is make your computer look like you are coming from a
different location (in a future class, we will explore how that works). 

As mentioned above, DNS responses can differ depending on your location.
Perform the following steps:

1. Perform a DNS lookup for `google.com` with your VPN disabled.
2. Now enable your VPN for some other location (preferably outside of the
   United States) and repeat the query.
3. Do the IP addresses differ?
4. Try to "geolocate" these IP addresses, for example using a service like [IP
   location](https://www.iplocation.net/) . How do the locations differ, and
   why?
