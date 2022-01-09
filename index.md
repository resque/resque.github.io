# Welcome

Resque is a Redis-backed ruby library for creating background jobs, placing those jobs on multiple queues, and processing them later. Unlike [Sidekiq](https://sidekiq.org) (an well-designed & well-maintained alternative!) it forks a new process for each job, which makes it resilient to memory leaks and eliminates thread-safety concerns. It's been battle-tested with high production loads and has a robust ecosystem of plugins to fill various needs.

[View on Github](https://github.com/resque/resque)

## Getting Started

- [README](https://github.com/resque/resque#resque)
- [RubyDocs](https://rubydoc.info/gems/resque)
- [RailsCasts #271 Resque](http://railscasts.com/episodes/271-resque)

## Site Contents

- [Customizing Resque using its hooks API](docs/HOOKS.md)
- [Plugin development](docs/PLUGINS.md)
- [Resque vs DelayedJob](docs/resque-vs-delayedjob.md)
