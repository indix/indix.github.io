# Indix Open Source Website

[![Build Status](https://travis-ci.org/indix/indix.github.io.svg?branch=source)](https://travis-ci.org/indix/indix.github.io)

## Setup

```bash
bundle install
bundle exec middleman serve
```

By default, all Github information is populated on the client side. But if a lot of users access from the same location, the API might be throttled. It might be ideal to use client side generation for development, and generate the information in deploy time for prod. To generate the Github information on build/deploy, do:

```bash
GITHUB_API=<user>:<token> bundle exec middleman build #or serve
```
