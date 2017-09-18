# CSC301 git-demo Sept 18

script of this demo:

we pretend we are working on a couple of features.
Tokyo makes f1 and Toronto makes f2.

We do it a couple of ways.. including a conflict.

We pretend it's a little C program.

include.h, source.c, README.md is all there is.

## Script for simple collab

on branch: take-turns

1. Tokyo "implements" f1 in include.h, pushes
1. Toronto pulls, "implements" f2 in source.c
1. Toronto pushes f2

## Script for simple collab that goes wrong

on branch: ff (ff stands for fast forward)

1. Tokyo "implements" f1 in include.h, pushes
1. Toronto "implements" f2 in source.c, commits
1. Toronto tries to push.. fails because behind
1. Toronto fetches, merges
1. Now Toronto can push


## Script for simple collab that goes even more wrong

on branch: conflict

1. Tokyo "implements" f1 by adding second line to source.c
1. Tokyo pushes
1. Toronto "implements" f2 in source.c, commits
1. Toronto tries to push.. fails because behind (again)
1. Toronto fetches, merges.. conflict
1. Toronto now can push

