---
layout: default
---
# Community

There are a number of places around the web where you can get information,
help, or discuss Resque.

## Getting Help

The best place to get help with Resque is to [ask a question on StackOverflow](http://stackoverflow.com/questions/tagged/resque). Make sure to search existing questions, it's possible that your question has already been answered!

## Feature Discussion

If you'd like to follow the development of Resque, or discuss future features
for it, please join [the Resque mailing list](mailto:resque@librelist.com).

## Reporting Bugs

If you've found a bug in Resque, please [file an Issue on GitHub](https://github.com/resque/resque/issues). We'll try to get it taken care of quickly, if possible.

When filing a bug, please follow these tips to help us help you:

### Good report structure

Please include the following four things in your report:

1. What you did.
2. What you expected to happen.
3. What happened instead.
4. What version of Resque you're using. You can find this with 
   `$ gem list resque`.

The more information the better.

### Reproduction

If possible, please provide some sort of executable reproduction of the issue.
Your application has a lot of things in it, and it might be a complex
interaction between components that causes the issue.

To reproduce the issue, please make a simple Job that demonstrates the essence
of the issue. If the basic job doesn't demonstrate the issue, try adding the
other gems that your application uses to the Gemfile, even if they don't seem
directly relevant.

### Version information

If you can't provide a reproduction, a copy of your Gemfile.lock would be
helpful.
