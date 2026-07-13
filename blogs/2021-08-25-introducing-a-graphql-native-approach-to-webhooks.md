---
title: "Introducing a GraphQL-native approach to webhooks"
url: "https://sourcehut.org/blog/2021-08-25-graphql-native-webhooks/"
date: "2021-08-25"
author: "SourceHut"
feed_url: "https://sourcehut.org/blog/index.xml"
---
Today, we are shipping a new system for webhooks for use with our suite of GraphQL APIs , which are under development as part of our larger beta plans . We’re not the first to use this design for webhooks, but it is somewhat uncommon, so I’ll take this opportunity to explain it to those who may be unfamiliar with it. Let’s first establish, for contrast, how traditional webhooks work.
