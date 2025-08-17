# aws-summit-sessions-jnb-2025
This repo is a dataset in [jsonl](http://jsonlines.org/) format of all the sessions (>100) at AWS Summit Johannesburg 2025 (20th August)
Pulled from https://aws.amazon.com/events/summits/johannesburg/. It's not official and may be out of date.

This data format makes querying easy with your favourite chat or agent-based tool, or JQ etc. The data doesn't seem to be 1:1 with the AWS Events app, I suspect around 30 sessions are duplicated (and are missing times.) Anyway, It's an engaging way to conversationally explore the sessions ahead of time.

Overall Stats
* Total Sessions: 138
* Sessions with a Scheduled Time: 103 (74.6%)
* Sessions without a Scheduled Time: 35 (25.4%)
* Duplicated Session Titles: 30 (These are sessions that are repeated during the event)

Unique Locations: 19

Unique Session Types: 6
* Breakout Session: 90
* Chalk Talk: 21
* Lightning Talk: 20
* Workshop: 5
* Keynote: 1
* Interactive Training: 1

Unique Start Times: 22
* The busiest time slot is 12:00 with 17 concurrent sessions.
* The majority of sessions start on the hour.

Session Durations:
* 45 minutes: 68 sessions (Most common)
* 15 minutes: 14 sessions
* 30 minutes: 12 sessions
* 75 minutes: 3 sessions
* 60 minutes: 2 sessions
* 120 minutes: 2 sessions
* 150 minutes: 1 session (Longest)

Based on the data and a few of my preferences, here's what it Gemini CLI thought I would like.

----
My reasoning combines the session's title, its type (favoring deep dives and technical talks over introductory ones), and the likely relevance of the topic to your specific interests. I'll also use a web search to get more context on some of the speakers and topics.

Top Recommendations for ML & Generative AI

1. Deep Dive into data protection architectures for Amazon Bedrock Agents.
    * Why: This hits the sweet spot between your architect and AI interests. "Deep Dive" suggests technical depth, and "data protection architectures" is a critical, senior-level concern. While not strictly "interpretability," understanding the data flow and security of AI agents is a closely related and crucial topic for any architect in this space.
    * Session Type: Chalk Talk (This is great, as Chalk Talks are typically interactive and technical).

2. Training ML Models for Content Classification: A SageMaker Journey
    * Why: This sounds like a practical, end-to-end case study. As an engineer, seeing a full "journey" on SageMaker would provide valuable hands-on insights that are directly transferable to building real-world ML systems. It moves beyond theory into implementation.
    * Session Type: Chalk Talk.

3. Accelerate ML workflows with Amazon SageMaker Studio and Sanlam
    * Why: This is a customer-led session (Sanlam), which is often invaluable for getting a real-world perspective without a marketing filter. Understanding how a major financial institution accelerates their ML workflows is a fantastic learning opportunity for an architect.
    * Speaker Context: A quick search confirms Sanlam is a major financial services group, so this will be a serious, enterprise-level use case.
    * Session Type: Breakout Session
    * Time: 13:00 - 13:45

These sessions focus on architecture, scale, and patterns that are fundamental for a cloud architect role.

1. Patterns for PrivateLink and VPC Lattice for Hybrid Networks
    * Why: Networking is a cornerstone of cloud architecture. Understanding advanced topics like PrivateLink and VPC Lattice for complex hybrid networks is a non-negotiable skill for a senior architect. This is likely to be a very dense and technical talk.
    * Session Type: Chalk Talk.

2. Fleet Tracking at Scale: Building for 4M Daily Transactions
    * Why: The title says it all: "at Scale." This is a real-world example of architecting a high-throughput system on AWS. The speaker, Jason Nicholls, is a Principal Solutions Architect at AWS, so you can expect a very high level of technical detail and architectural best practices.
    * Session Type: Breakout Session.
    * Time: 16:00 - 16:45

3. Apache Iceberg and what it means for Analytics
    * Why: Data architecture is a huge part of cloud architecture, especially in the ML/AI space. Apache Iceberg is a modern, open table format for huge analytic datasets. Understanding its implications is crucial for designing next-generation data lakes and data warehouses that feed ML models.
    * Session Type: Breakout Session.
    * Time: 12:00 - 12:45

Hidden Gem

1. Your Next User Isn’t Human: Agentic AI in Action
    * Why: This title is forward-looking and touches on the emerging paradigm of AI agents as users of systems. For a senior engineer, thinking about how to design APIs and services for non-human consumers is a fascinating architectural challenge that will become increasingly important.
    * Session Type: Breakout Session.

I would recommend prioritizing the sessions with "Deep Dive" and "at Scale" in the title, and definitely the customer-led session with Sanlam. When you have more specific constraints (like times you are unavailable), I can help you build a personalized schedule from this list.

----

## Side note: Session Types

### Keynotes

* Large, main-stage presentations.
* Delivered by AWS executives, senior engineers, or high-profile customers.
* Cover **major announcements, strategic directions, customer success stories**, and big-picture trends.
* Usually open to all attendees and set the tone for the event.

### Breakout Sessions

* The most common format, usually **45–60 minutes**.
* Deep dives into specific AWS services, architectures, or use cases.
* Grouped by tracks (e.g., AI/ML, serverless, security, migration, data & analytics).
* Can be **introductory (Level 100)**, intermediate (200), advanced (300), or expert (400).

### Workshops

* Hands-on sessions, often **2–3 hours long**.
* Attendees work in teams with guidance from AWS instructors.
* Cover **practical scenarios** like building serverless apps, deploying ML models, or securing workloads.
* Require you to bring your own laptop and AWS account.

### Chalk Talks

* Whiteboard-driven technical discussions.
* Around 45–60 minutes, with an AWS expert leading but **audience-driven Q\&A** shaping the flow.
* Great for **architectural discussions** or clarifying best practices.
* Less slide-heavy, more **dialogue and sketching**.

### Lightning Talks

* Short, **20–30 minute presentations**.
* Focused on **specific topics or quick insights**.
* Often scheduled in expo/demo areas or smaller stages.
* Good for quick overviews without deep technical depth.

### Interactive Training

* Guided, self-paced labs you can do during the summit.
* Walkthroughs on AWS services (like building with Lambda, RDS, or SageMaker).
* Often powered by AWS-provided temporary accounts.
* More structured than workshops, less open-ended.

### Startup Talk
