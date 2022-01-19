---
layout: post
title:  "Ace the Amazon Leadership Principle interview questions"
date:   2022-01-19
image: amazon-overlay.jpg
description: This article contains tips and resources that will help you prepare for the Amazon Leadership Principle interview questions
categories:
	- Interview
---



I had recently appeared for an SDE 2 amazon interview and this article will document my experience for the same. The entire process took about 3 months from the day the recruiter contacted me to the time I got the offer. 

Telephonic Screening
[15 days after the first conversation with the recruiter]
This is an elimination round. The goal of this round was for the interviewer to determine if I should be allowed to appear in the on-site rounds. The duration was 45 mins and I was expected to provide a complete solution to the given DS/Algorithm question. 

Q: Search a word inside a given matrix: https://leetcode.com/problems/word-search/

I was quickly able to come up with a solution using a DFS traversal. I hadn’t practiced much before the telephonic round so it took me a while to implement the solution. I was able to finish it with about 10 mins to spare, we did a couple of dry runs with the test cases. Once the interviewer was satisfied with the solution, we discussed time and space complexity for this and alternate solutions using other traversals like BFS.

Overall, the round went well but I took an important data point that I need to speed up my coding by practicing more before I start appearing in on-site rounds. So, I asked the onsite to be scheduled after 20 days. 

Onsite 1: DS and Algo Round
[21 days after Telephonic round]
I had practiced a bit more and was ready to go. The duration of this round was expected to be 1 hour. The interviewer was expected to judge me on leadership principles and DSA. We started off with Leadership Principle related questions. I had really good examples from my past experiences which demonstrated strong LP application. This took about 20 mins of the interview and we proceeded to the DSA round. 
Q 1 : Gas station problem:  https://leetcode.com/problems/gas-station/

I was able to implement this immediately and had discussion around the time complexity of my solution. 

Q 2: Connect the nodes at the same level, similar to:https://leetcode.com/problems/populating-next-right-pointers-in-each-node/

We discussed the solution for this but we ran out of time before I could completely implement the solution. 

Overall, the round started off well but somewhere along the way I lost track of time and wasn’t able to get everything done in time.(One of the reasons this happened was because I was expecting only one DSA question.)

I decided that from next round onwards I will ask the interviewer if there is a followup or another question post this. The recruiter had similar feedback.  

Onsite 2: DA and Algo Round
[Same day as Onsite 1]
The expectation for this round was the same as onsite 1. This round also started off DSA:
Q1: compute the size of the largest island in the given matrix where 0 represents sea and 1 represents land. 

The interviewer confirmed there is a follow up after this. So I quickly implemented the solution using a modified DFS traversal and discussed time/space complexity. While implementing I was also explaining the same to the interviewer so he didn’t need me to explain the solution again at the end.

Follow up: Now you are allowed to change at max 1 sea cell to land cell what would be the size of the largest island formed in this case. https://leetcode.com/problems/making-a-large-island/

So, it wasn’t very difficult considering I already had half the solution implemented in the Q1. I explained the DFS based solution and the interviewer was happy. He asked if there are any other ways to solve the same problem. I proposed using Union find to keep track of connected components and size of the island and then compute the largest. 

Note: DFS based solution was better in terms of time complexity but the interviewer was really interested in how I would handle this with UF. 

He asked me to implement the Union find based solution and I was able to do it fairly quickly. 
Post this, the interviewer asked me LP related questions and I did well on them just like round 1. 
We only had a minute or so to spare for my questions. I had multiple questions around what he did and what the team was working on. 

This round went pretty well. The recruiter said this round had great feedback. The recruiter also gave me a heads up that the upcoming rounds are design rounds and I should take my time to prepare. My day job had a lot of design exposure so I felt well prepped and asked the recruiter to schedule the interview soon. 

Onsite 3: High-level design Round
[7 days after onsite 2]
The expected time for this round was 1 hour 10 mins and the expectation of this round was to judge me on 2 LPs and my High level design skills. 

LP discussion was a little longer in this round. It went very well as I had very good examples to demonstrate the application of those principles. You can find my tips on how to ACE…


The Design Question: Design a chat system  for amazon returns team. Here a bot can respond to customers using a predefined workflow and if the customer reaches the end of bot workflow then allow an option to chat with a live amazon returns agent. The customer can add photos and videos to the chat. Considering agents are working from home and an agent goes offline, new agents should be able to see chat history immediately. 

We used the invisionapp website for the design diagram  and I did really well on this round. My tips for Acing the HLD:
Have a structured approach and be open to suggestions. For example: start with estimation, then make assumptions and decide scope, then come up with very high level design and later discuss individual components. 
Make sure you are properly communicating your rationale behind every tech decision. Like why use web sockets over long polling? Or why do we choose No-sql over SQL DB?
Make sure you discuss limitations and bottlenecks and a plan to avoid those if required. 
Ask frequent feedback explicitly. Ask if there is anything specific that needs to be discussed before I move on to the next component. 
And many more, stay tuned for a blog around this.


Onsite 4: Bar-raiser and Low-level design round
[7 days after onsite 3]
The expected time for this round was 1 hour 10 mins and the expectation of this round was to judge me on 2 LPs and my Low level design skills. 

This round the Discussion of LPs was much detailed and longer. As mentioned before I had prepped really well with great examples so it went very well. We spent about 35 mins just discussing my past experiences.

LLD: Design a snake and ladder software board game. I was asked to keep the design as extendible and modular as possible. 

I made an extendible OOD design and then we kept adding more scenarios that the system can be extended to handle. For example how will you handle a multi-player live action shooting or a cricket game or How easily can you change the board configuration of snakes and ladders, etc.

Make sure you use good design patterns to make your design adaptable and easy to extend. Some design patterns which I used are:
Strategy pattern
Observer pattern
Factory method
State design pattern

Onsite 5: Additional DS and Algo round
[7 days after onsite 4]
This was an additional round conducted to test me a bit more on DSA. The expected time for this was 1 hour and the interviewer was expected to ask 2 DSA questions. By this time I had already cleared on-sites of multiple different companies so was pretty confident.

Q1:A simple DP:  https://leetcode.com/problems/climbing-stairs/
This was basically Fibonaci, solved this in just under 5 mins. 

Q2: Find the order in which a compiler will build given files.If two files that are not dependent on each other then the order does not matter. Before compiling a file, all its dependent modules should be compiled.

Solved this using topological sort. Discussed Space and time complexity. 

I asked the questions I had for the interviewer and we still had about 20 mins to spare. So, we ended the call early. The round went very well.

[7 days after the Onsite] The recruiter called to inform them they were planning to extend an offer. I didn’t accept the offer at the end as I had already accepted an offer from another company. 

One of the major differences between interviewing at Amazon and other FAANG companies is their approach to the behavioural interview. Read more on how to Ace the amazon Leadership principle questions. 
