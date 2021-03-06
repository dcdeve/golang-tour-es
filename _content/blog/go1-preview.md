---
title: A preview of Go version 1
date: 2011-10-05
by:
- Russ Cox
tags:
- go1
- release
summary: What the Go team is planning for Go version 1.
---


We want to be able to provide a stable base for people using Go.
People should be able to write Go programs and expect that they will continue
to compile and run without change,
on a timescale of years.
Similarly, people should be able to write books about Go,
be able to say which version of Go the book is describing,
and have that version number still be meaningful much later.
None of these properties is true for Go today.

We propose to issue a Go release early next year that will be called “Go version 1”,
Go 1 for short, that will be the first Go release to be stable in this way.
Code that compiles in Go version 1 should,
with few exceptions, continue to compile throughout the lifetime of that version,
as we issue updates and bug fixes such as Go version 1.1, 1.2, and so on.
It will also be maintained with fixes for bugs and security flaws even as
other versions may evolve.
Also, production environments such as Google App Engine will support it
for an extended time.

Go version 1 will be a stable language with stable libraries.
Other than critical fixes, changes made to the library and packages for versions 1.1,
1.2 and so on may add functionality but will not break existing Go version 1 programs.

Our goal is for Go 1 to be a stable version of today’s Go,
not a wholesale rethinking of the language.
In particular, we are explicitly resisting any efforts to design new language
features “by committee.”

However, there are various changes to the Go language and packages that
we have intended for some time and prototyped but have not deployed yet,
primarily because they are significant and backwards-incompatible.
If Go 1 is to be long-lasting, it is important that we plan,
announce, implement, and test these changes as part of the preparation of Go 1,
rather than delay them until after it is released and thereby introduce
divergence that contradicts our goals.

Today, we are publishing our preliminary [plan for Go 1](https://docs.google.com/document/pub?id=1ny8uI-_BHrDCZv_zNBSthNKAMX_fR_0dc6epA6lztRE)
for feedback from the Go community.
If you have feedback, please reply to the [thread on the golang-nuts mailing list](http://groups.google.com/group/golang-nuts/browse_thread/thread/badc4f323431a4f6).
