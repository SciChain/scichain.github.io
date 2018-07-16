---
title: "Uploading an article"
permalink: /docs/uploading-paper/
toc: true
---

## Basic instructions

When an author intends to submit a paper to an specific journal (scientific community) , it can call `RequestArticle` function. The first parameter addresses the self address, then thedata content (title + abstract + keywords), then the editor address. Note that the editor itself is allowed to participate.

`testinvoke "5265717565737441727469636c652829" ["AK2nJJpJr6o664CWJKi1QRXjqeic2zRp8y","HelloWorldPaper","AK2nJJpJr6o664CW JKi1QRXjqeic2zRp8y"]``

## Useful information

This function returns an special `ProcessKey` (32 bytes) that can track the author communication with the editor/journal, and store process-related information. Initially, the payload is used for title, abstract and keywords submission, and this information is used by the editor to decide upon reviewer assignment. This part is intended to connect with Endorsement functions in order to allow for autonomous reviewer selection in SciChain self-managed journals.
