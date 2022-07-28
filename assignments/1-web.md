# Loading a Webpage - Browser Inspection

## Overview

In this assignment, we will load a webpage and use your browser's "inspect"
tool to explore all of the things that are required to load a web page. We
will do some of this assignment in class, and you can finish it on your own
before Thursday. 

There will be no grading of assignments for this class other than completion,
and so you are welcome to work at your own pace.

## Background

You have all likely loaded web pages many times in your life already. What
happens "under the hood" when you load a website?

As it turns out, there are many tasks involved with loading a site, including:
  * Retrieving the main "index" page
  * Retrieving each individual object on the page
  * Looking up the domain name for each web page
  * Ultimately rendering each object

Retrieving each object requires making a connection to the webpage that
"hosts" that object. Indvidual web pages may be composed of hundreds of
objects, together which are assembled to show you the page.

## Activity

Load a simple web page, like ``https://www.cs.uchicago.edu/``. Once the page
loads:
  * Right click on the page
  * Find the option to "inspect" the page
  * Click on the "network" tab to show the network activity associated with
    the page.
    
This tab shows you lots of information about everything that goes on when
loading a webpage. Network operators, application designers, and engineers
often look at this page to understand things about their webpages and
applciations, from how the network might be slowing down the connection, where
they might host different objects to improve page load times, and even how to
redesign a webpage to speed up performance. 

Below are some questions we can explore in the performance console.

## Questions

Look at the inpsection tool to see if you can figure out the answers to some
of the following questions:

1. How many objects did the browser need to load to load this webpage?
2. Which object loaded first? From where?
3. What other objects loaded next?
4. How many objects does your browser load in parallel?
5. Which object(s) took the longest to load?

Repeat the above for a simple page like `https://www.cs.uchicago.edu/` and
then again for a more complicated page of your choice (e.g.,
`https://nytimes.com/`)

## Going Further

Suppose you wanted to make this webpage load faster. What kinds of
optimizations could you make?

Think about the following, and feel free to experiment if you can!

1. Blocking ads and trackers (install an ad blocker and see what happens)
2. Pre-loading certain content

What if you were on a slower connection, or a connection that charged you a
lot of money for data (e.g., per byte)?  What types of optimizations could
you make?
