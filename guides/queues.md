---
layout: default
---
# Queues

(this guide is still in progress)

Why would you need something like Resque? In this guide, you'll learn:

1. What a job queue is.
2. When to deploy one with your application.
3. Other tools that accomplish a similar task.

----------------------------------

## What is a job queue?

A job queue is a piece of software that allows you to asynchronously schedule
units of work, and then process them according to that schedule.

What do I mean by 'a unit of work'? Basically, any sort of programming task
that you need to accomplish. 

Job queues are an implementation of the Producer/Consumer design pattern. An
application 'produces' units of work, and the queue has some sort of worker
processes that consume those units.

## When should I deploy one?

## Similar tools
