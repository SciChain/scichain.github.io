---
title: "Including a new reviewer (referee)"
permalink: /docs/including-reviewer/
toc: true
---

## Basic instructions

Each editor can register a set of reviewers using `RegisterReviewer` function, passing both its address (20 bytes) and the reviewer address (20 bytes).

`neo> testinvoke 0xfc47d1b7b2fe38096433af7c5e543033d87a86d1 "526567697374657252657669657765722829" ["AUk19KeZqgryWfxfvfAkCcEFLNGhzoPivi","APLJBPhtRg2XLhtpxEHd6aRNL7YSLGH2ZL"]``

**Used GAS:** 1.818 Gas

This function returns true (1) if reviewer is successfully registered. If the reviewer is included many times, system will return the appropriate message: "Reviewer already registered".

## Useful information

This function has already many internals that deal with Endorsement invocations (interacting with several other functions), and in future works (see roadmap below) we will allow for self-managed journals to filter reviewers automatically (integrated with a Dynamic Invoke smart contract called Smart Rules, in the same github project).
