---
title: 'Reflections on Lorem Ipsum'
updated: 2015-09-09 10:38
---

This is a minimalist Jekyll theme built to focus on writing stuffs that matter. Suitable to be used as a personal blog[^whatblog]!

> "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?"

# Synopsis

This document is intended to familiarize the customer success team with the third iteration of our scripting platform (hereafter `v3`) which they will be relying upon through Q4 2016. After a high-level summary of how `v3` works, an attempt will be made to give customer success a sense of what sorts of functionality can be easily implemented with `v3`, and of which teams will need to contribute to implementations of various kinds.

# What is scripting? What can it do for me?

At root, scripting v3 allows `App Developers` to distribute `Apps` to Lanetix organizations. `Apps` consist of `Handlers`, or small programs written in javascript, which run in response to `LxNotify` notifications. An `App Administrator` specifies parameters for to create an `Install` of an `App` for a particular organization. These parameters allow the `App Administrator` to customize the behavior the handlers which run in response to notifications issued by user actions within a particular organization. In the overwhelming majority of cases, this behavior will consist of calls to internal Lanetix APIs. Highlighted terms are defined below.

## Walkthrough

The above is a lot to take in at once. We suggest walking through [this tutorial](http://imgur.com/a/O4baj), in which you'll find step by step instructions for installing the `fieldjoin` App to get the now familiar "namejoin" behavior, reading thd definitions of key terms below, then returning to the above. Don't hestitate to ping Bjorn with any questions.

[^whatblog]: More of a series of notes.
