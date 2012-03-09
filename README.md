vector.js
=========

What?
-----

A basic library for common vector operations in 2D. The library also includes a method for annotating the operations with "types" (in practice, just __vector__ and __number__ that will throw errors when the vector operations are passed parameters of the wrong type.

Why?
---

I wanted a reason to learn more about javascript and the module pattern, and I thought a vector library would be useful for canvas creations. Also vectors are pretty much my favorite things to work with.

No, Why?
--------

Oh, why did I try adding some weird semblance of type checking? Temporary insanity I suppose. The problem with vector operations in javascript is that while you're certainly allowed to scalar multiply a vector with a vector, the resulting NaNs aren't so fun in practice, and the problems they cause can be hard to find the root of. So I thought a basic type checking system might help stop those problems before they occur. The system won't stop you from doing whatever you please, but it will write a warning to __console.error__ and give you a bit of information about what function you messed up. 

No extra effort is required on your part.
