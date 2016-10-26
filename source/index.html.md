---
title: Bucket API Reference

language_tabs:
  - shell

toc_footers:
  - <a href='https://github.com/tripit/slate' target="_blank">Documentation powered by Slate</a>

includes:
  - errors
  - sessions
  - users
  - tools
  - segmentation_funnels
  - quiz_types
  - outcomes
  - question_types
  - questions
  - sections

search: true
---

# Introduction

Welcome to the Bucket.io API!

# Authentication

> To make an authorized request, you can do it like this:

```shell
curl "[API-ENDPOINT]"
  -H "Authorization: [ACCESS-TOKEN]"
```

> Make sure to replace `[ACCESS-TOKEN]` with your access token.

Bucket API expects for the access token to be included in all requests to the server in a header that looks like the following:

`Authorization: [ACCESS-TOKEN]`

<aside class="notice">
You must replace <code>[ACCESS-TOKEN]</code> with your access token.
</aside>
