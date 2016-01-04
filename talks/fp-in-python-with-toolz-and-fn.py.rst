Functional programming in Python with Toolz and fn.py
=====================================================

  *In my brief experience people rarely take this [streaming] route.
  They use single-threaded in-memory Python until it breaks, and then
  seek out Big Data Infrastructure like Hadoop/Spark at relatively
  high productivity overhead.* ~ Matt Rocklin

That quote succinctly summarises my computational life, right up
until recent months.

In "traditional" programming, you load a dataset into memory,
process it in some way, and output the result. This is simple to
understand. But in streaming programs, a function processes *some*
of the data, *yields* the processed chunk, then downstream functions
deal with that chunk, then the original function receives a bit
more, and so on... All these things are going on at the same time!
How can one keep them straight?

This talk will introduce Matt Rocklin's *Toolz* library which makes
functional programming easy in Python and provides a framework to
write elegant, concise code to analyse bigger-than-memory data, and
*fn.py*, which has even more FP constructs.  I'll present streaming
data analysis using FP from the ground up, from a simple
"hello-world" example to image illumination correction and streaming
extensions to scikit-learn classifiers, and analysing a genome in a
few minutes.

Juan Nunez-Iglesias
-------------------

Juan is a research scientist at the University of Melbourne's
Victorian Life Sciences Computation Initiative.  His undergraduate
degree was in biomedical science, but he slowly veered towards a
computational biology and software engineering career. He is a core
developer of the scikit-image library, teacher of scientific
programming, and author of an upcoming book about the SciPy library.
I am also author of the (decidedly non-functional!) gala image
segmentation library.

| GitHub: `jni <https://github.com/jni>`_
| Twitter: `jnuneziglesias <https://twitter.com/jnuneziglesias>`_
| Blog: `I Love Symposia! <http://ilovesymposia.com>`_
