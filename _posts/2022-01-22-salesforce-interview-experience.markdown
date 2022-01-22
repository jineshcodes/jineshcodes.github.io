---
layout: post
title: "Salesforce MTS Interview Experience"
date:   2022-01-22
image: Salesforce_Interview.jpg
description: I recently appeared for a Salesforce MTS interview, and this article will document my experience.
comments: true
categories: [Interview, Salesforce]
---

I recently appeared for a Salesforce MTS interview, and this article will document my experience. The entire process took less than two weeks, from the day the recruiter contacted me to the time I got the offer.

Note: when the recruiter reached out to me, I had already cleared onsite for two other companies and was waiting to hear back on their offer. I informed the same, and the recruiter decided to fast track my interview process. 

Salesforce MTS interview process has one online screening and three on-site rounds. Making a total of four rounds. [Because of the global pandemic everything was conducted virtually.]

#### Online Screening
*[1 day after the initial call with the recruiter]*

This was an online coding round on hacker rank. There were two coding questions to be implemented in 1 hour. 

Q1: Similar to [Hackerrank - Alien numbers](https://www.hackerrank.com/contests/coderadon/challenges/alien-numbers)

Q2: Similar to [LeetCode - Compare version numbers](https://leetcode.com/problems/compare-version-numbers/)

I completed both the questions with about 10 minutes to spare.

#### Onsite 1: Data Structures and Algorithms
*[4 days after the coding round ]*

The duration of this round was expected to be 1 hour. The interviewer was expected to judge me mostly on DSA. There will be two DSA questions, and the expectation for me was to write code and then run it on hackerrank to pass all test cases. 

The interviewer first asked me a few basic questions about my experience, and I was already well prepared for this. We quickly moved to DSA questions. 

Q1: This was a straightforward and popular question, similar to [interviewbit - meeting rooms](https://www.interviewbit.com/problems/meeting-rooms/)

As I had already solved this question in the past, I solved it fairly quickly. 
 
Q2: There are two train lines(red and blue) from source(index 0) to destination(index n). You will be given weights for travelling on the same line from i to i+1 in red[i] and blue[i]. There is a cost associated with changing lines which will be given to you as redToBlue[i] and blueToRed[i]. You need to find the minimum cost to travel from source to destination. Assume you always start on the blue line. 

I solved it by building a recurrence equation for DP and then implemented it in a bottom-up fashion. I had solved the first one quickly, so I had enough time to finish the implementation and run the test cases. This question took me about 30 minutes to solve and another 5 minutes to fix a corner case I missed. 

This round went well. 

#### Onsite 2: Behavioral and Technical
*[1 day after Onsite 1]*

A director of the organization conducted this round, and the expectation was to talk and get to know me better to make a call if I am a good fit for the role. The estimated time for this round was 1 hour.

We started by introducing each other and sharing a bit about our work experience so far. The round was different from typical interviews and was an excellent opportunity to know more about Salesforce. 

I was interviewing for a security and identity organization. Most of the questions were generic, but a few were focused on security and compliance. Here are some of the questions as I remember them:
* Talk about a project of your choice while highlighting your contributions. 
* How would you go about building the monitoring for a system or a service you just used? 
 * What are the monitoring tools you used in your past organization? How do you build a similar tool if it is not available today at Salesforce?
* What are the things you keep in mind to ensure your system or service is Secure? What are the principles you should follow?
* What are some of the technologies every service should use for Lifecycle management? He was expecting more of a list here. The answers could vary based on experience.   

I was able to do well on the monitoring questions, as I had been a part of the team under the Azure Monitor organization. I was also able to do well on the security-related questions as I studied a Secure Computer Systems course as a part of OMSCS. (which I am pursuing while working as an FTE.)  

Also, as a follow up to most of the answers I shared, I asked about how Salesforce does this scenario, which gave me great insights into what the team does and what I should expect if I join. Anyway, most of these things were discussed again when I talked to the hiring manager. 

#### Onsite 3: Data Structures and Algorithms
*[Same day as the Onsite 2]*

The expectations of this round were same as Onsite 1.

Q1: Find the median of a stream of numbers. The median should be running as new numbers keep coming in. 

I had already seen this problem in the past when I skimmed through Cracking the coding interview. So, I explained how I would handle this with a min and a max heap (my implementation used a Priority queue). I also talked about alternate solutions like using a BST and rank. 

The interviewer asked me to implement a min-heap data structure as a follow-up. I implemented it from scratch, and he was impressed by the pace of implementation.

Q2: Similar to Gas station problem: [Leetcode - Gas Station](https://leetcode.com/problems/gas-station/)

I had recently solved this problem as a part of an Onsite interview with another company, so I was able to solve it in under 5 minutes. I told the interviewer that I had seen this problem before.

Overall, all the interview rounds went very well.

*[3 days after the interviews]* The recruiter shared me an offer. I did not accept the offer in the end as I was keen to accept an offer from another company.

Feel free to read other by me related to interview prep and experience on [jinesh.codes/interview](jinesh.codes/interview)
