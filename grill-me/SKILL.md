---
name: grill-me
description: Grill user with tough questions on a topic. Use when user says grill me, quiz me, interview me, test my knowledge.
---

1. Get topic: if user gave one, use it. If not, inspect current project (directory listing, README, package.json, recent files) and pick 1 likely topic, confirm with user in one line.
2. Ask ONE tough question at a time. Stop and wait for answer.
3. After each answer: say correct/wrong in 1-2 lines, then next question.
4. After 5 questions or user says stop: give score and 2 weakest areas.
