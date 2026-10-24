# My Story

🇲🇽 [Leer en español](MI-HISTORIA.md)

My name is Alejandro. I'm 45 years old and a technology professional whose career has been built mainly around networking, infrastructure, and Cisco solutions.

Throughout my career I've worked as a pre-sales architect for Cisco solutions, a role that has placed me between two worlds: the technical and the human. It's not only about knowing equipment, protocols, or architectures, but about understanding what a client needs, translating that need into a technology solution, and helping different people understand it and make decisions about it.

My experience has allowed me to develop both technical and communication skills. I've worked with Cisco equipment, designed solutions, trained others and shared technical knowledge, taken part in technology projects, and supported clients through decisions that often involve complex technologies.

In recent years I've expanded into **data center architecture**. Today I work with solutions from vendors such as **Dell, Lenovo, and Everpure Storage**, and I'm familiar with backup and data protection tools like **Veeam and Commvault**, as well as virtualization platforms like **VMware and Red Hat**. This step gave me a more complete view of infrastructure: not only how things connect, but where data lives, how it's protected, and how applications run.

A big part of my professional life has been facing that complexity. I've had to keep learning, stay current, and adapt to technologies that are constantly evolving. In technology, standing still practically means falling behind, so learning has become a natural part of my work.

I've also discovered that one of my strengths is explaining complex things in a way others can understand. I can move between a deeply technical conversation and one with someone who needs to understand the impact of a solution without knowing every detail.

Today I'm at a stage where I look at my career with perspective. I have experience, technical knowledge, and a much broader view of what it means to work in technology than I had when I started.

I'm not only the professional who knows Cisco or designs network and data center architectures. I'm someone who has learned to solve problems, work with many kinds of people, take on complex projects, and keep learning even when circumstances change.

## A new chapter: from networks to AI agents

Today I'm taking a step I wouldn't have imagined a few months ago: I'm building AI agents and deploying them on AWS.

I started with an AWS course. When I reached the final project — a full banking architecture with multiple regions, networking, databases, and high availability — I realized I first needed stronger foundations. So I decided to start with something concrete: a research agent that receives a topic, searches the internet, summarizes the information, and saves a report, with no interface and no human intervention.

What makes this interesting is that I started practically from zero in programming. I didn't know Python, had never seriously used the terminal, and didn't know what Git was. In a few days I set up my computer with developer tools, learned Git and GitHub, managed my own API keys securely, and wrote my first programs.

Along the way I also learned something beyond code. I made real mistakes — like accidentally exposing an API key in a screenshot — and learned to fix them immediately and not repeat them. I document every step in a learning log: not just what I do, but what I learn and the problems I solve, because I believe how you think and solve problems matters as much as the result.

### What I've built so far

**1. Research Agent.** It decides on its own what to search for, runs several searches, and writes a report where every claim cites its source. It started on my computer and now runs on AWS with Lambda, API Gateway, and S3. Reviewing its reports taught me my first big lesson: if you don't force an AI to cite every fact and to say "I didn't find this," it fills the gaps with irrelevant information.

**2. Internal Support Agent.** It answers employee questions using a fictional company's documents — vacation, travel expenses, policies — with RAG on Amazon Bedrock. It cites which document the answer came from, and when the answer isn't there, it says "I don't know" instead of inventing. I built an automated exam of 25 questions, including trick questions, and it scored 25/25. Getting there meant calibrating a confidence threshold with real data, catching a trick question about salaries that the AI almost answered, and hunting down a single misplaced letter in my code that dropped the whole exam to zero.

**3. Telegram Ordering Agent.** A fictional neighborhood store takes orders by chat. The customer writes the way they talk — "give me 2 kilos of tortillas and a soda" — and the agent checks the real catalog, builds the order, asks for address and payment, and saves it with a folio number. This one taught me the most:

- Without a catalog, the AI invented products the store didn't sell.
- It told customers "your order is confirmed" without having saved anything. I added a guard in code that checks it.
- An automated test found that the customer saw a total of $84, but the order was saved at $168. To the eye, the conversation looked perfect.
- Even with a "SOLD OUT" label, it kept offering the product. It only stopped when I removed it from the list entirely.

After four attempts, it passed 8 out of 8 test conversations.

### What these agents taught me

AI doesn't fail for lack of intelligence. It fails for lack of data and controls. A rule written in a prompt isn't enough: money and business rules must be decided and verified by code, not by the model. Without automated tests there is no trust, because "it looks fine" is not the same as "it works." And a well-built agent costs only cents per conversation.

I realized my previous experience doesn't stay behind. On the contrary: understanding networks, data centers, storage, backup, virtualization, and security helps me see how the pieces connect in the cloud. And my pre-sales background gives me something many technical profiles don't have: the ability to explain what a solution is for, how much it costs, and what value it brings to a client.

## Where I'm going

My goal is to build five AI agents, each more complex than the last. Two are done and the third is in progress. Next, I'll deploy the ordering agent on AWS with Terraform and a message queue, so no order is ever lost even when something fails. For the last two I'm exploring an AI pre-sales team that drafts technical proposals, and small tools for everyday business tasks.

I chose small-business use cases on purpose: they force me to solve real problems — messy human input, money that must be exact, rules that can't be broken, and costs that must stay low. Every agent is designed with the same questions I've always asked as an architect: is it reliable, is it secure, how much does it cost, and can I measure it?

I also share the process in public, in Spanish, as **El Futuro con Alex**: what I build, what breaks, and what I learn. Explaining it to others is how I make sure I really understand it.

I want to build a "T-shaped" profile: broad foundations in cloud, networking, data center, security, and cost, with deep expertise in AI agents on AWS. My goal is for my GitHub to show real, working, well-documented projects, and to be able to explain every decision I made.

In the long term, I see myself as a Solutions Architect specialized in AI, combining what I've always done well — understanding needs and turning them into solutions — with one of the technologies transforming the world the most today.

At 45, I'm not starting from scratch: I'm adding a new layer to everything I've already built.

And above all, I'm Alejandro: a 45-year-old man who keeps learning, questioning what he knows, and trying to better understand who he is and what he wants to do with everything he has built so far.