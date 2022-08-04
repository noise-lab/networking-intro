# Internet Equity

The Federal Communications Commission (FCC), advocacy groups, scholars, and
others interested in Internet performance have had wide-ranging discussions
over the years on two related (but distinct) topics: (1) benchmarking Internet
performance standards  (“Am I getting what I’m paying for?”); and (2) equity
(“digital divide” challenges, Internet access haves and have-nots). Various
organizations, from regulators to public interest groups, have developed tools,
methods, and datasets to try to answer these questions.

## Overview 

In 2021, the Infrastructure Investment and Jobs Act authorized $65 billion to
expand broadband access and adoption, and address disparities highlighted by
the COVID pandemic and the shift to remote work, school and health care. But to
invest that funding most effectively for improving digital equity in the United
States, new and deep data at a local scale must be gathered and analyzed to
drive effective policy and advocacy solutions for the citizens and
neighborhoods most in need.

In this exercise you will explore how Internet performance in a specific
high-income neighborhood compares with Internet performance in a specific
low-income neighborhood. 

### Part 1: Basic Data Exploration

We have been performing network performance measurements across nearly 30
neighborhoods across Chicago over the past year to try to get a better handle
on some aspects of how performance varies across neighborhood and time.  Load
some of the into a program you are comfortable performing some analysis in.
We have pre-loaded some of the data into the following Google sheets as
read-only.  You may need to make a copy to perform some analysis.

- [Throughput](https://docs.google.com/spreadsheets/d/1XgwV0H6O6mLLZC0iUkxWsHCfR85q2a38YjpRh0VqffE/edit?usp=sharing)
- [Local network throughput](https://docs.google.com/spreadsheets/d/1D9hrFAH44_xyQ_38LB8T3r1algUp5QRRQn_0jPfKhxU/edit?usp=sharing)
- [Latency Under Load](https://docs.google.com/spreadsheets/d/1ZWTWia5Wt8q-JeKhw_cufcQkpPf70z71ad9jQgnwOAk/edit?usp=sharing)
- [DNS Lookup times](https://docs.google.com/spreadsheets/d/1eBj1-qUmy6IpnWp8hTzbivHWHR4vXuZXWJsnFIewI_M/edit?usp=sharing)

Take one of the files of interest and see if you can find any trends.  For
example, how does throughput vary over time?  How does latency or latency
under load correlate with throughput?

(The above links are accessible from the University of Chicago. Public data is
also available from the [project
page](https://github.com/chicago-cdac/netrics-data).

### Part 2: Neighborhood-Level Exploration

The `devices_by_community.csv` file has some information pertaining to devices
by community.  One could perform a neighborhood-by-neighborhood comparison of
these devices to see how performance varies across communities, for different
dimensions.

We have performed some versions of that analysis in this
[paper](https://www.ssrn.com/abstract=4179787) where you can read more about
these comparisons. The data we have provided also allows you to perform some
of that analysis yourself.

Some simple computations you could explore include:
- What is the average throughput (or latency, or DNS lookup time) for a device
  in Logan Square? In South Shore?
- What is the device with the lowest average throughput in each neighborhood?
  What is that value?

## Going Further

Approaches such as those you have explored in this assignment could provide
researchers and policymakers an opportunity to offer citizens a data-driven
approach to address their core concerns about Internet equity. 

How would you frame and formulate questions concerning equity and “digital
redlining” in ways that could be suppoted by data analysis?
