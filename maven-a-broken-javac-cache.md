Maven: A broken `javac` cache
===

In recent years there has been a rise of distributed version control
tools like `git` and Continuous Integeration
engines like Jenkins which try to compile every
new commit in a source tree.  This has revealed that the Maven
mindset may need some adjusting to work really well in these
scenarios!

Some of the issues identified so far:

* Artifacts are essentially cached output from `javac`, but with no well-defined course of action
for cache misses.
* Recompiling an artifact with unchanged sources do not produce a binary identical artifact.
* Promoting a given build to be a new version cannot be done without changing
the pom and rebuilding the artifacts.
* Maven versioning only allows for releases and branch-tips.





CACHE PROBLEM
---

...

NON-REPRODUCIBLE BUILDS
---
...

REBUILD TO CREATE NEW VERSION
---

...

MAVEN VERSIONING INSUFFICIENT
---

...

