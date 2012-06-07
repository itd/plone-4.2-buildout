Plone 4.2 site buildout
=======================
A basic Plone 4.2 buildout. I'll update this
when I can to keep up with the latest releases of 4.2.

All the standard Plone stuff applies.
Make sure you have all the libs you need,
and run this from a virtualenv.

What the heck? ./bin/buildout doesn't work!
--------------------------------------------
I run my builds as either develop.cfg or production.cfg
so there's no guessing. We're all smart. Deal with it.

On my dev boxes, I do a:
  ./bin/buildout -c develop.cfg

On production, I do:
  ./bin/buildout -c production.cfg

If you have several development environments, just
cp the develop.cfg and edit away. One for Bob, one for Judy, etc.
Since these should be unobtrusive, you can even check them in.


Because I'm lazy, I have an alias on my devel boxes to do the build:
alias plb=./bin/buildout -c develop.cfg

There's also a bash shell script that does some checks.
You can ask me for it if you want.


Staging and user acceptance
------------------------------------
If you have, say, staging and user acceptance
environments, cp production.cfg and tweak to
your hearts content, and just
  ./bin/buildout -c yourthing.cfg
for whatever yourthing happens to be.


