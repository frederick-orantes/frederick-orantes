# Multi-User AI Assistant on Claude

A conversational AI assistant built on Anthropic's Claude API and hosted on AWS EC2. It serves multiple users at once and keeps each person's information and conversation context separate, so every user gets a personalized experience. It is live and in daily use by real users.

## Why I built it

I spent nearly six years helping enterprise customers adopt new technology, and in recent years most of that work was about AI. I built this project to understand AI from the builder's side: what it takes to run an assistant reliably, keep users' data separate, and make it useful day to day.

## What it does

- Holds natural conversations powered by Claude through the Anthropic API.
- Supports multiple users at once, with each user's information and context stored separately.
- Runs continuously on an AWS EC2 instance, serving live users.

## Tech stack

- **Language:** Python
- **AI model:** Claude, through the Anthropic API
- **Hosting:** AWS EC2
- **Data:** separate stored context for each user

## Design choices

- **Per-user context:** each person's information is stored on its own, so one user's data never shows up in another user's conversation.
- **Secrets stay out of code:** API keys are loaded from environment variables and never committed to this repository.

## Running it yourself

1. Clone the repository.
2. Install the dependencies listed in the project.
3. Set your Anthropic API key as an environment variable (see `.env.example`).
4. Start the app.

## What I'm exploring next

- Connecting tools and data sources through the Model Context Protocol (MCP), which I already use daily to automate my own work.
- Building agents that automate real business workflows, with a person reviewing before any action.

## About me

I'm Frederick Orantes, a customer success leader and AI builder based in Austin, TX, with a B.S. in Mechanical Engineering. I've led AI adoption for enterprise clients, including governed AI workflows that save each of a client's project managers 7–13 hours a week. Connect with me on [LinkedIn](https://www.linkedin.com/in/orantes).
