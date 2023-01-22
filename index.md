---
layout: page
title: "Responsible AI"
doodle: "/doodle.png"
permalink: /
---

# DSC180-A05, Data science capstone: Responsible AI 

| Q1 Fall 2022 | [Classes held on **Zoom**](https://ucsd.zoom.us/j/96921239764) | Fridays at 10AM PT |


### Developed by David Danks, Jeffry Liu, Nandita Rahman, Aritra Nath, Emma Harvey, Meira Gilbert, and Rasmus Nielsen.

---
* TOC
{:toc}

---
# Introduction

The explosive proliferation of research around ethical AI (Artificial Intelligence) and AI trustworthiness during the last decade  reflects a rising societal awareness and desire to address potential and actual harmful impacts and consequences of AI. We introduce students to the socio-technical risks of AI fairness and explainability by examining several high-profile algorithmic discrimination debates that have sparked seminal research in this field. We will discuss the range of alternative definitions, the perspectives they represent, and metrics used to examine AI fairness, and the papers that describe the interesting yet mathematically irreconcilable relationships that interweave them. Concepts around AI-fairness will be translated into real-world applications through classroom debates from the perspectives of different disciplines and stakeholders, and by replicating the analyses from a relevant use case example. Students will conduct an independent fairness and explainability analysis on a mock model using industry recognized toolkits, with an emphasis on understanding how issues that originate in code and math eventually affect real human beings and society as a whole.

**In this domain, project proposals will be restricted to the following
areas:**
* What does AI trustworthiness and ethics mean for different stakeholders?
* What are the ways to think about whether or not a model is fair?
* What are the risks of ‘black box’ algorithms, and how do we mitigate them? How is AI explainability related to fairness?
* How do inherent fairness problems in AI models affect human beings?  

### Instructor: Dr. David Danks
David Danks is a Professor of Data Science & Philosophy at University of California, San Diego as well as affiliate faculty in UCSD’s Department of Computer Science & Engineering. He serves on advisory boards for various organizations including: National AI Advisory Committee (NAIAC), Special Competitive Studies Project (SCSP), Partnership to Advance Responsible Technology (PART), Center for Advancing Safety of Machine Intelligence (CASMI), Topos Institute, AI Community of Practice (US Government), and Grefenstette Center for Ethics in Science, Tech., & Law. He has received a James S. McDonnell Foundation Scholar Award (2008) and an Andrew Carnegie Fellowship (2017). Previously, he was the L.L. Thurstone Professor of Philosophy & Psychology at Carnegie Mellon University. While at CMU, he served as the Chief Ethicist of CMU’s Block Center for Technology & Society and co-director of CMU’s Center for Informed Democracy and Social Cybersecurity (IDeaS). 

### Industry Partner: Deloitte, Trustworthy AI Team
As one of the largest professional services organizations in the United States, Deloitte provides a vast array of information security services across 2,800 engagements in major commercial industries and 15 cabinet-level federal agencies. Our Trustworthy AI team has helped many of our clients work through the burgeoning regulatory landscape and growing awareness around ethical and trustworthy AI. For this course, the Deloitte team will consist of Rasmus Nielsen, Aritra Nath, Emma Harvey, Nandita Rahman, Meira Gilbert, and Jeffry Liu. We’re excited to work with UCSD in developing this course, and we look forward to discussing these exciting topics with you.

# Course Resources
### Office Hours
* Professor Danks will hold office hours Wednesdays 1-2PM (PT) in UC 302, Room 101 
* Replication Project: Nandita Rahman (Replication PoC) will hold office hours Mondays 1-2pm (PT) for assistance with replication project materials, held [virtually](https://github.com/nanrahman/capstone-responsible-ai/blob/b48a0f37b19f266e5b32430ee4b85b92b215e826/notes/week-04/replication-office-hour-zoom-info.md)

### Course Communications
Please send any questions to the Responsible AI Slack Channel: 
* Slack Channel link: [Responsible AI Capstone](responsibleaicapstone.slack.com)
* For any issues with Slack, email David Danks (ddanks@ucsd.edu)
* For private or personal questions, you can reach out to David privately via email (ddanks@ucsd.edu)


# Course Expectations and Assignments

### Quarter One Project (70%)
* Introduce students to the area in which they will do their project through replicating a known result.
* Students will complete coding tasks related to the replication project and are also responsible for creating a final writeup
* Create written material and code that serves as a foundation for work in quarter-2’s projects.
* Full details of the requirements for the Q1 project can be found in the [Capstone Program Syllabus](https://dsc-capstone.github.io/syllabus/)

### Quarter Two Project Proposal (15%)
* Students will develop a project proposal for Q2 based on their learnings and interests from the course readings and the replication project
* Full details of the requirements for the project proposal can be found in the [Capstone Program Syllabus](https://dsc-capstone.github.io/syllabus/)

## Participation Credit
Students are responsible for completing the readings in full prior to the start of each week’s session in order to facilitate productive class discussion. All readings will be freely available and linked in the course website. Participation in the weekly discussion section is *mandatory*. Each week, you are responsible for doing the reading/task assigned in the
[schedule](#schedule). Come to section prepared to ask questions about
and discuss the results of these tasks. 

### In-class Participation Questions (5%)
* Prior to class, Students must post responses to participation questions for that week's assigned reading (see: [Schedule](https://github.com/nanrahman/capstone-responsible-ai/edit/master/index.md#schedule)). Responses should be submitted on [Gradescope](https://www.gradescope.com/courses/442598) **24 hours prior to the start of each class session**

### In-class Brief (5%)
Each student is responsible for preparing one five-minute in-class brief on one of the academic papers assigned as readings. 
* Following the first session, students will have the opportunity to [sign up](https://docs.google.com/spreadsheets/d/1DNA4mQLQmbhFEtm74PEPsUDTEGx0pK_BFzlQcltFaMg/edit?usp=sharing) to present on one of the course readings. Students are responsible for creating a PowerPoint presentation summarizing the reading, including its background, methodology, argument/key contributions, and their thoughts on the implications/impact of the article. 
* Reading presentations are due via Gradescope prior to the start of the session for which the reading is assigned; students are also responsible for presenting to the rest of the class during the session. Presentations should take five minutes. 

### Written Assignments (5%)
* For each writeup prompt (see: [Schedule](https://github.com/nanrahman/capstone-responsible-ai/edit/master/index.md#schedule)), students are responsible for responding in at least 500 words (one single-spaced page). Writeups are due via Gradescope before the start of the session in which they are due. 

### Grading
Please see the [Capstone Program Syllabus](https://dsc-capstone.github.io/syllabus/) for a detailed description of the assignment weights and rubric. 

---

# Schedule

|Week|Date|Topic|
|--|--|--|
|1|09/30/22|[Introduction to Trustworthy AI]({{ "weeks/01-Introduction-to-Trustworthy-AI" | absolute_url }})|
|2|10/07/22|[A Multi-Stakeholder Perspective on Ethical AI]({{ "weeks/02-Perspectives-on-Ethical-AI" | absolute_url }})|
|3|10/14/22|[Replication Project Part 0: Introduction]({{ "weeks/03-Replication-Part-00" | absolute_url }})|
|4|10/21/22|[Replication Project Part 1: EDA, Running Data Science Teams]({{ "weeks/04-Replication-Part-01" | absolute_url }})|
|5|10/28/22|[AI Regulations]({{ "weeks/05-AI-Regulations/" | absolute_url }})|
|6|11/04/22|[Replication Project Part 2: Fairness Assessments]({{ "weeks/06-Fairness-Assessments" | absolute_url }})|
|7|11/10/22|[Replication Project Part 3: Bias Mitigation]({{ "weeks/07-Bias-Mitigation" | absolute_url }})|
|8|11/18/22|[Capstone Planning & Avoiding Techno-Solutionism]({{ "weeks/08-Capstone-Planning-Techno-Solutionism" | absolute_url }})|
|9|12/02/22|[Replication Project Part 4: Presentations]({{ "weeks/09-Q1-Replication-Presentations/" | absolute_url }})|

---
