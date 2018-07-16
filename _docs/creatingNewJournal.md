---
title: "Creating a new journal (editor)"
permalink: /docs/new-journal/
date: 2017-10-30T11:48:41-04:00
toc: true
---

## Basic instructions

In order to create a new journal, the editor in charge can pass its address (20 bytes) to RegisterEditor function.

`neo> testinvoke fc47d1b7b2fe38096433af7c5e543033d87a86d1 "5265676973746572456469746f722829" ["AUk19KeZqgryWfxfvfAkCcEFLNGhzoPivi"]`

Used *GAS*: *1.472 Gas*

This function returns an `EditorKey` (32 bytes). This `EditorKey` plays an important role in the next operations.

## Useful information

If an Editor tries to register multiple times, system will return the appropriate message: "Editor is already registered".
