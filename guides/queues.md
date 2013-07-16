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

### Delayed Work

Queues are useful any time you don't immediately need the result of some
computation, and your process or user-experience would benefit from assuming
that the work will get done at some point soon.

If some action in your web application were to send notifications to hundreds
of users via e-mail, the user submitting that action shouldn't have to wait for
every one of those e-mails to send before their page loads. Queues allow your
application to take responsibility for some future action, and render the page
to the user *as if* the e-mails were going to be sent;  instead of holding up
the process, the consumers of the queue would then do the units of work given
to them as quickly as they were able.

## Similar tools
