---
layout: post
title: "Amazon SDE 2 Interview Experience"
date:   2022-01-19
image: Amazon_interview.jpg
description: I recently appeared for an Amazon SDE 2 interview, and this article will document my experience.
comments: true
categories: [Interview, Amazon]
sitemap:
    priority: 0.7
    changefreq: 'monthly'
    lastmod: 2022-01-28T12:49:30-05:00
---

I recently appeared for an Amazon SDE 2 interview, and this article will document my experience. The entire process took about three months, from the day the recruiter contacted me to the time I got the offer. 

Amazon SDE-2 interview process has one telephonic screening and four on-site rounds. Making a total of five rounds. Sometimes, there are additional rounds conducted as a part of on-site interview. [Because of the global pandemic everything was conducted virtually.]

{% include toc.md %}

#### Telephonic Screening
*[15 days after the first conversation with the recruiter]*

This is an elimination round. The goal of this round was for the interviewer to determine if I should be allowed to appear in the on-site rounds. The duration was 45 mins, and I was expected to provide a complete solution to the given DS/Algorithm question. 

Q: Search a word inside a given matrix, similar to [Leetcode: word search](https://leetcode.com/problems/word-search/)

I quickly came up with a solution using a DFS traversal. I hadn't practised much before the telephonic round, so it took me a while to implement the solution. I finished it with about 10 mins to spare, and we did a couple of dry runs with the test cases. Once the interviewer was satisfied with the solution, we discussed time and space complexity and alternate solutions using other traversals like BFS.

Overall, the round went well, but I took a critical data point to speed up my coding by practising more before appearing in on-site rounds. So, I asked for the on-site to be scheduled after 20 days. 

#### Onsite 1: DS and Algo Round
*[21 days after Telephonic round]*

I had practised a bit more and was ready to go. The duration of this round was expected to be 1 hour. The interviewer was expected to judge me on leadership principles and DSA. We started off with Leadership Principle related questions. I had good examples from my past experiences that demonstrated strong LP application. This took about 20 mins of the interview, and we proceeded to the DSA round. 
**Q1** : Gas station problem:  [Leetcode - Gas Station](https://leetcode.com/problems/gas-station/)

I was able to implement this immediately and discussed the time complexity of my solution. 

**Q2** : Connect the nodes at the same level, similar to [Leetcode - Populating Next Right Pointers in Each Node](https://leetcode.com/problems/populating-next-right-pointers-in-each-node/)

We discussed the solution, but we ran out of time before thoroughly implementing the solution. 

Overall, the round started off well, but somewhere along the way, I lost track of time and couldn't get everything done in time. (One reason was that I was expecting only one DSA question.)

I decided to ask the interviewer if there would be a follow-up question. The recruiter had similar feedback.  

#### Onsite 2: DA and Algo Round
*[Same day as Onsite 1]*

The expectation for this round was the same as on-site 1. This round also started off DSA.

**Q1** : Compute the size of the largest island in the given matrix where 0 represents sea and 1 represents land. 

The interviewer confirmed there is a follow up after this. So I quickly implemented the solution using a modified DFS traversal and discussed time/space complexity. While implementing, I also explained the same to the interviewer, so he didn't need me to explain the solution again at the end.

**Follow up** : Now, you are allowed to change at max one sea cell to land cell what would be the size of the largest island formed in this case. similar to [Leetcode - Make a large island](https://leetcode.com/problems/making-a-large-island/)

It wasn't very difficult, considering I already had half the solution implemented in Q1. I explained the DFS based solution, and the interviewer was happy. He asked if there were any other ways to solve the same problem. I proposed using Union Find to keep track of connected components and the size of the island and then compute the largest. 

**Note**: DFS based solution was better in terms of time complexity, but the interviewer was interested in handling this with Union Find. 

He asked me to implement the Union find based solution, and I was able to do it fairly quickly. 
After this, the interviewer asked me LP-related questions, and I did well on them, just like in round 1. 
We only had a minute or so to spare for my questions for the interviewer. 

This round went pretty well, and my recruiter confirmed that this round had great feedback. The recruiter also told me that the upcoming rounds are design rounds, and I should take my time to prepare. My day job had a lot of design exposure, so I felt well prepped and asked the recruiter to schedule the interview soon. 

#### Onsite 3: High-level design Round
*[7 days after on-site 2]*

The expected time for this round was 1 hour 10 mins, and the expectation of this round was to judge me on 2 LPs and my High level design skills. 

LP discussion was a little longer in this round. It went very well as I had excellent examples to demonstrate the application of those principles. You can find my tips on how to [Ace the LP interview questions](https://jinesh.codes/blog/ace-amazon-lp-questions/).


**HLD**: Design a chat system for the Amazon returns team. Here a bot can respond to customers using a predefined workflow and if the customer reaches the end of the bot workflow, then allow an option to chat with a live Amazon returns agent. The customer can add photos and videos to the chat. Considering agents are working from home and an agent goes offline, new agents should see chat history immediately. 

We used the invisionapp website for the design diagram, and I did well on this round. My tips for acing the HLD:
Have a structured approach and be open to suggestions. Something like:
* Start with estimation.
* Make assumptions and decide scope.
* Come up with a very high-level design 
* Later, discuss individual components in more detail.

And some tips:
* Make sure you are properly communicating your rationale behind every tech decision. Like why use web sockets over long polling? Or why do we choose No-SQL over SQL DB?
* Make sure you discuss limitations and bottlenecks and a plan to avoid those if required. 
* Ask for frequent feedback explicitly and Ask if anything specific needs to be discussed before moving on to the next component. And many more, stay tuned for a blog around this.


#### Onsite 4: Bar-raiser and Low-level design round
*[7 days after on-site 3]*

The expected time for this round was 1 hour 10 mins, and the expectation of this round was to judge me on 2 LPs and my Low level design skills. 

This round, the Discussion of LPs was much more detailed and longer, as mentioned before. I had prepped well with great examples, so it went very smooth. We spent about 35 mins just discussing my past experiences.

**LLD**: Design a snake and ladder software board game. I was asked to keep the design as extendible and modular as possible. 

I made an extendible OOD design, and then we added more scenarios that the system could be extended to handle. For example, how will you handle a multi-player live-action shooting or a cricket game, how easily you can change the board configuration of snakes and ladders, etc.?

Make sure you use suitable design patterns to make your design adaptable and easy to extend. Some design patterns which I used are:
* Strategy pattern
* Observer pattern
* Factory method
* State design pattern

#### Onsite 5: Additional DS and Algo round
*[7 days after on-site 4]*

This additional round was conducted to test me a bit more on DSA. The expected time for this was 1 hour, and the interviewer was expected to ask 2 DSA questions. By this time, I had already cleared on-sites of multiple different companies, so I was pretty confident.

**Q1**:A simple DP similar to [Leetcode: Climbing stairs](https://leetcode.com/problems/climbing-stairs/)

This was basically a Fibonacci type problem, and I solved this in just under 5 mins. 

**Q2**: Find the order in which a compiler will build given files. If the two files are not dependent on each other, the order does not matter. Before compiling a file, all its dependent modules should be compiled.

Solved this using topological sort and discussed space and time complexity. 
We still had about 20 mins to spare. So, we ended the call early. The round went very well.

**[7 days after the interviews]** The recruiter called to inform them they were planning to **extend an offer**. I didn't accept the offer in the end as I had already accepted an offer from another company. 

One of the significant differences between interviewing at Amazon and other FAANG companies is their approach to the behavioural interview. Read more on how to [Ace the Amazon Leadership Principle questions](https://jinesh.codes/blog/ace-amazon-lp-questions/). 

Feel free to read other posts related to interview prep and experience on [jinesh.codes/interview](https://jinesh.codes/interview)

