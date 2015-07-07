# reader.htm
A Federated Wiki frontend

Originally found on http://hapgood.us/2015/07/05/calling-all-hackers/

I spent the last couple weekends coding up a standalone federated wiki reader that operates 
purely in javascript. Here it is: reader.htm. Now here’s what you can do if you know how to
program. You can download that file, and and start to play around with it, and build your 
own federated wiki reader. I want you to join us in our mission to create a federation that
can function across servers like a net-enabled Memex. 

I want to see if you can come up with a better way to browse it, or to render it, or to whatever.
Everything is in that one file that you need — code and js. It’s about 300 lines, and you can run
the html file from your desktop. (About 120 of the lines are code). A couple caveats:

  1.  It’s read-only. It solves the easier technical problem.
  2.  I don’t really know javascript. I honestly spent a lot of the time looking up things like how
        to do a case statement, or loop through an array.
  3.  I’m not really a programmer. I was a programmer almost 15 years ago. 
        But even then it was MUMPS, Python, XSLT, ColdFusion, other things.
  4.  Asynchrony confuses the heck out of me. If you look at it and believe I’m misunderstanding how
        to code asynchronous JSON let’s have a hangout. I could learn.
  5.  I had a version of this I wrote about a month or two back that I demo’d to some people, but
        there was an important difference — that version read the federated wiki format but couldn’t
        resolve links in the federation. This one resolves links by looking through the fork history
        of the page and querying those sites about whether they might have a copy of the linked page.
  
The weirdest thing about this code is that it’s so simple in a way. Once you carry the fork history
in the page, the page can travel around wherever it wants, and links can be resolved without hard-coding
brittle and rigid URLs in the wiki markup. Once you use JSON as the basis of pages instead of HTML,
multiple sites can work as one giant site.  

Taken together these two simple ideas (along with the legal technology of Creative Commons) create a 
radically different vision of the web. I guess what I’m saying (and what I’m hoping you see in the code)
is it’s a lot simpler than you might think to get to the vision of a World Wide Wiki. If a hack like me
can get this done in a couple weekends, what could you do? Video on how the code works forthcoming.
But download it now and start playing with it.
