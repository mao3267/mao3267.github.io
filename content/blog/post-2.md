---
date: '2026-03-23T10:06:25-07:00'
draft: false
title: 'Updated My Website with Claude Code and Stitch'
tags: ['Web Development', 'Claude Code', 'Stitch']
---

Now is in an era that AI is developing rapidly than ever. Just three month passed in 2026, we have seen the release of newer foundation models, AI agents (Claude Code, OpenClaw, etc.) and the new UI design tool - Stitch. These tools are getting better and better, and I am excited to try them out to see what I can do with them.

The original design of this website is using a template from the hugo community. However, I think the design is not that modern and lack of the "tech" feeling. So I decided to redesign it using Claude Code and Stitch.

First, I started with Stitch to create a frontend design. My prompt is literally simple:

> This is my portfolio & blog website: https://mao3267.github.io, I want to update it to a more modern, technical, high-quality UI for all pages, and add a newsletter subscription section at the bottom of the homepage.

Actually I didn't expect much from Stitch, thinking that we might need more rounds of conversation to get what actually works for me. But surprisingly, it did a great job and gave me a design that I really like.

As for implementation, I used Claude Code with Stitch MCP to fully implement the design. My general workflow looks like this:
1. Ask Claude Code to research on the possiblilties of implementing the design, and ask it to create a plan.
2. Manually review the plan and make sure it looks reasonable.
3. Start Building and actively monitor the progress with local build.
4. Code review with agent and fix bugs.
5. Manually test the features and make sure it works as expected.
6. Push and deploy the website to check if it works as expected.

In my observation, thanks to the help of MCP, the UI design looks exactly the same as the design from Stitch. However, there are still some bugs that need to be fixed. For example, the newsletter subscription section is not working as expected, and the blog post filter has bugs and thus being a little bit messy. I will continue to work on it and finish the functionalities.

This is a great experience on using AI agents with MCP to build a website. I am excited to see what else I can do with these tools in the future. 

Some funny truth:
1. It's really hard to use all the weekly limit of Claude Code, the bottleneck is my brain to come up with ideas, not the AI itself LMAO
2. Annoying that some updates need hard refresh to see the changes, not sure if it will affect users' experience.
3. Really love the design! I don't know how Stitch knows that I like purple... Scary.

