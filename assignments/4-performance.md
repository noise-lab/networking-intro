# Internet Performance

One of the main things that the Internet needs to do is perform well, so that
it can provide a good user experience to users. Measuring Internet performance
is challenging, as there are many dimensions to performance, which vary over
time. 

Some of these metrics are complex, and can be difficult for consumers to
understand. By the end of this activity, you will understand the basic metrics
for measuring Internet performance, as well as some of the challenges in
accurately measuring performance.


## Overview 

Internet performance involves many metrics, including the following:
  - **Throughput (``speed'').** Measured in bits per second, this is how much data
    can be transferred across the network in a given amount of time.
  - **Latency.** Measured in milliseconds, this is the amount of time it takes for
    a single piece of data to go from one place to another on the network.
  - **Jitter.** Measured in milliseconds, this is variation in latency, 
  - **Packet loss rate.** Measured in percent or fraction, this is the fraction of
    packets lost.
  - **Latency under load, or responsiveness.** Measured in milliseconds, this is
    the latency as measured when there is traffic being sent on the network.
All of these affect the performance of Internet applications in different
ways. One of the difficulties in measuring and characterizing Internet
performance is that performance is multi-dimensional; another aspect of
performance measurement that is so challenging is that performance varies over
time.  

The tools we will use in the assignment below are used for a variety of
purposes, from troubleshooting Internet connections to generating maps
concerning Internet performance and coverage across geographies (e.g., cities,
states). The data is problematic for generating coverage maps; yet, even for
understanding performance of a single Internet connection, the tools can be
tricky to use and make sense of, as we will explore below.

## Activity

In this activity, we will explore the different components of measuring
Internet performance, notably an Internet speed test. You will run an Internet
speed test under a variety of conditions, multiple times to see how the
performance metrics vary over time, under repeated runs, and under different
conditions.

### Part 1: Basic Speedtest

1. Open up your web browser and go to the [Speedtest](https://speedtest.net/) website.
2. Run a speed test by clicking "Go" on the web page.
3. Make note of the following values:
    - Upload Throughput
    - Download Throughput
    - Latency
    - Ping (latency)
    - Upstream Server
    - Your Internet Service Provider
4. Enter the values above into the following [web form](https://forms.gle/4kDJPFuYPfrxYN3P9).

### Part 2: Varying the conditions

1. Run the same test again above.
    - Do you see the same numbers? Why or why not?
2. Repeat the above steps with the following variations:
    - On your cell phone (with and without WiFi turned on)
    - From the [Measurement Lab website](https://speed.measurementlab.net/#/).
3. Think about the following questions:
    - What differences do you notice?

## Going Further

How well does Internet speed testing reflect user experience? That is a
complex question, and one that really cuts to the chase of many questions at
the intersection of Internet technology and policy.

Read [this article](https://www.wsj.com/graphics/faster-internet-not-worth-it/) about how
fast Internet speeds need to be to support different applications like video
streaming on demand.

- Does a speed test reflect the user experience in this case? 
- How would you design a better speed test that captured user experience?
