# Math Notes

How can I store math notes as code?

## Using Sage on Macos

1. Install: `brew cask install sage`
2. Run from spotlight/dock: 
  - search using `cmd+spacebar` for "Sage" and run it.
  - drag "Sage" into the dock
  - Sage will load a jupyter notebook.
  - You will be asked where to store your notebooks

- EXTRA: Run from terminal: `sage --notebook=jupyter`
  - This works fine
  - Seems like I end up with multiple instances and the port used is incremented each time
  - Notebooks will default to your `$HOME` path

- DEPRECATED: Run from terminal: `sage -n`
  - I think sage has converted completely to jupyter?
  - The old method was `sage -n` which still works but gives a page with a manual redirect

## Is this form of expression useful for initial problem solving?

If I put the problem in and get the solution, then I've ruined the problem. I should solve it first from my available context (e.g. book, lectures, similar problems in the set or previous sets).

*However, once I've solved it, it's worth it to explore the intermediate space with solvers.*

## Working through problems

I am not sure the best way to work through a problem as code.

I do know that problem solving mimics generating a mathematical proof.

Many proofs exist for a particular math concept, so working through problems is about taking the path relevant to the context you are working within. 

### On Solutions

Perhaps the most bizarre part of math is the concept of "solving a problem".

Math conjectures are solved when expressed as a proof in "existing math".

Often, high profile conjectures are solved by inventing a new "mathematical concept" or "form of mathematical expression".


### Typical Problem Solving

Typical algorithm for doing math problem: Given a problem and some math context, find a solution.

#### Definitions & Expressions

- Problem: expressed by a set of math notations.
- Context: expressed as a collection of lectures, english writing, and math notations.
- Solution: Acceptable transformation of the problem with the provided context.

### TDD: Test Driven Development

Once I have a problem and a solution, I can simply express the intermediate steps and expect to arrive at the same solution.

Given a math problem and solution, I can build a manifold of steps that get there.

Typically we consider "showing your work" to be following the main path, based on the context you are given, from the problem to the solution.

Most problem-solution pairs are intended to cross a set of `critical facts` that cannot be bypassed anyways. Otherwise the problem might be considered poorly designed or simply to have multiple "ways to get there".

It's interesting to think of isomorphic problem spaces and transformations as this repo grows.
