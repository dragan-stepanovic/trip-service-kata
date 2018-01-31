Trip Service Kata
=================

Kata for legacy code hands-on session. The objective is to test and refactor the legacy TripService class.

The end result should be well-crafted code that express the domain.

You can watch the video with my solution. Although quite long, I explain my whole thought process while writting tests, how I break dependencies, the reasons for refactoring and re-desining the code (tests and production code), and why certain steps are important. I also cover how often I commit and why I do it. 

The video is full of tips and tricks that can be used in any language.

https://www.youtube.com/watch?v=_NnElPO5BU0


------------------------------------------------------

how many of you have watched Sandro's video?

Kata rules: 
you cannot change production code if not covered by tests! (only automated refactorings, by your IDE, are allowed, but never type into the file)
start testing from the shortest do deeper branches
	-it will help you understand code INCREMENTALLY since deepest branches are most difficult to understand at once
	-also, setup for deepest branches is massive, so starting to test from the shortest branch (most outer) will also help you incrementally do this
	
start refactoring from the deepest branch
	-because the deepest branches are isolated in terms of behaviour. if you change it, it is higher probability that you won't affect other parts of the code as it is the case when you try to refactor shallowest branches which can affect other branches (that are deeper in the call chain)
	
run a code coverage after you write the test to see which part of production code you covered and if you can refactor it. If you don't have code coverage functionality in your IDE, try to figure out logically/mentally what part of production code does your tests cover.
some of you don't have much experience in tdd or writing unit tests, but don't be too much bothered by it

after a coding session that will last for hour, we can see and discuss some of the solutions.
pair by languages if possible.

what is most important is to have fun!	
