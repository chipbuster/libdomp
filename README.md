The Dummy OpenMP Library
========================

Sometimes, you have code that relies on OpenMP function calls, but you really
just want it to run in single-threaded mode without having to link to an 
OpenMP runtime. Maybe you don't have access to an OpenMP implementation, 
or maybe the link flags are a pain in the butt, or maybe you're using some
tool that keep screwing up the linking.

Fortunately, domp (the Dummy OpenMP) fixes all of that. Just include this
version of `omp.h` in your headers, and watch as all of your programs 
magically collapse to single-threaded mode!
