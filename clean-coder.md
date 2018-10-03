## Chapter 1 - Professionalism 

* Being a professional means taking full responsibility for one's actions.
> "What would happen if you allowed a bug to slip through a module, and it cost your company $10,000?". The non-professional would shrug his shoulders, say 'stuff happens', and start writing the next module. The professional would write the company a check for $10,000!"
* _[real disaster story about field-failure of a routine each test of which took hours]_

First rule is not doing harm to the function nor the structure of the software. 
* You will always make occasional mistakes, but you must learn from each. Promptly 

You should be certain about all code you release and firmly expect QA to find nothing wrong with it.
* Test it. Test it again.
* Automate your tests.
* Demand 100% coverage.
* Design your code to be easy to test.

You should follow the Boy Scout rule and always leave a module a little cleaner than you found it so that it becomes easier to change over time, not harder.
* Suitable automated tests can allow you to not be afraid to change the code and continually changing it makes sure it stays that way	

Your career is your responsibility, not your boss nor your employers. 
* Spending 20 hours a week beyond your normal work to improve your knowledge and skills 
* Read, experiment, practice (kata), talk to other, collaborate, look over the fence, mentor 
* It should be fun.

Also, know your domain, identify with your customer (no "us vs. them", ever).
* Be aware of arrogance inherent in programming and learn to be humble, too.


## Chapter 2 - Saying No
* Real disaster story about premature deployment of a totally immature distributed system
* Professionals speak truth to power. Professionals have the courage to say no to their managers.
* Managers and developers have roles that are often adversarial, because on the short term, their goals tend to conflict.
* The manager will defend her objectives, but will also expect you to defend yours for the best overall outcome, which is reaching the largest goal that you and the manager share, which may be tricky to determine
* The higher the stakes, the more valuable a "no" becomes, and the harder to say. 
* Good teams will successfully work towards a yes, but only a right yes, that will later work out in practice. 
* Saying "no" is often a prerequisite for getting that right yes. 


## Chapter 3 - Saying Yes

There are three parts to making a commitment
* You say you will do it
* You mean it
* You actually do it
	 
* A professional will not stop after step 1 or step 2. 

Unconditional commitment always takes a form equivalent to "I will achieve goal X until time Y"
* Commitment means taking full responsibility. 
* Most results depend on conditions you cannot fully control, so you will often only commit to actions or commit only conditionally
 
Your commitment must respect the limits of what you expect (based on your experience) you can and cannot do
* If you recognize you will probably not be able to meet a commitment, you need to raise a red flag immediately  


## Chapter 4 - Coding


Coding requires a level of concentration and focus that few other disciplines require. 

* A clean coder codes only if she can guarantee enough focus
* Distractions (personal, environmental, or whatever) are a problem. 
* Overtime is a problem.

Flow ("the zone") is not as good as people think: you will be locally productive, but will often lose sight of the bigger picture and possibly product no-so-good designs 

Interruptions are bad distractions. 
* Pair programming is helpful to cope with them. 
* TDD helps to make the pre-interruption context reproducible 
* Minimize time spent debugging 

If you have writer's block, start pair programming 
* Make sure you take in enough creative input, e.g. reading fiction books. Find out what works for you

Coding is a marathon, not a sprint, so conserve the energy and creativity. 
* Go home when it's time, even in the middle of something important. 
* Showers and cars are problem-solving resources too.
 
Continuously re-estimate your best/likely/worst completion time and speak up as soon as you recognize you will likely be late. 
* Do not allow anyone to rush you. 
* Consider overtime only for short stretch (2 weeks max.) and only if there is fallback plan as well. 
* Use a proper definition of "done", with sufficiently high quality requirements 
 
Programming is too hard for anyone, so get help and provide help to others, in particular (but not only) in mentoring style. 
* Don't protect your turf, don't shy away from asking, don't show away others who ask.

## Chapter 5 - Test-driven development 

TDD is not a cure-all and is impractical or inappropriate in some (rare) cases.

Three principles:
1. You are not allowed to write any production code until you have first written a failing unit test
2. You are not allowed to write more of a unit test than is sufficient to fail, and not compiling is failing 
3. You are not allowed to write more production code than is sufficient to pass the currently failing unit test

The cycle only about 30 second long
* It provides certainly not having broken anything when making changes
* It reduces defect injection rates often 2-10x
* It provides courage for cleaning up messy code
* It documents how code is to be used 
* It makes you create designs with low coupling

## Chapter 6 - Practicing 


A programming Kata is a precise set of choreographed keystrokes and mouse movements that simulates the solving of some programming problem. 

* You aren't actually solving the problem because you already know the solution. 
* Rather, you are practicing the movements and decisions involved in solving the problem (IDE, TDD, CI)


## Chapter 7 - Acceptance Test

Avoid garbage in, garbage out. Make sure you understand the requirements, and expect your customer to initially not understand them. 
* Creating this understanding means removing ambiguity 

Best way to do this is defining acceptance tests: 
* Ask the customer for all conditions they will plausibly want the software behavior to fulfill and turn them into automated tests. 
* Customers often will not want to answer all your questions, so developers or tests will have to guess, in particular for the failure cases, and then validate the result with them
* Success of those tests constitutes the definition of "Done"
 
Code implementation should start only when the test implementation is complete. 
* Look out for silly, awkward, or plain incorrect tests and work with the test authors to improve them 

Unlike unit tests (which are for programmers only), the audience of acceptance tests are both business and developers. 
* Prime purpose of both kinds is specification, testing is only secondary. 

Test GUIs mostly one level below the actual GUI (on abstractions of the GUI elements) to reduce test volatility 
	
Run all tests in a continuous integration and immediately fix any failures that may occur.


## Chapter 8 - Test Strategies 

Consider QA part of the team. They act as specifiers: writing acceptance tests, including the failure cases and corner cases, and perform exploratory testing

Testing pyramid 
1. Most tests are unit tests
* By developer and For developers
* Executing almost every statement of the class and asserting its behavior
2. Many tests are component or integration tests 
* By QA or Business assisted by Developers, For Business and Developers
* In a component testing framework, executing all relevant paths through larger combination of classes. 
* Component tests mock away other parts of the system and assert correct business rules.
* Integration tests may or may not mock and assert correct choreography of the pieces 
 
Some tests are automated system tests of the whole, usually at GUI level with the respective tools
 
A bit more testing is done manually at system level in creative, exploratory fashion

## Chapter 9 - Time Management 

Software development, especially in management roles, requires good time management discipline 
 
Meeting are necessary but are also often huge time wasters, so avoid meeting that have no clear benefit -> this is a professional obligation. 
 
Meeting must have an agenda and a clear goal
* Agile stand up meetings can be an efficient format 
* Iteration planning should take 5% of the iteration (2 hours for  one-week iteration)
 
Any argument that can't be settled in five minutes can't be settled by arguing. So don't try to; make measurements, flip a coin or vote
 
Concentration (focus) is a scarce resource
* Use it well when present and recharge with simpler tasks (meetings) and breaks in between 

How to improve? 
* Sport
* Creative input
* Pomodoro techniques (25 - 30' block time)
 
Professionals work on their real tasks, in a sensible priority order, even if they don't like some of them 
* They admit when they have chosen the wrong path and leave it quickly 
* They recognize messes (whether their own or others') and never accept them, they clean up.
* Nothing brings down productivity more than a mess. 

## Chapter 10 - Estimation 

Estimation is the source of most distrust between business people and developers, because the latter provide estimate which the former treat like commitments. 
* both are insufficiently aware that the estimate really is a probability distribution, not a fixed number 

The PERT technique computes and uses such distribution based on base-case, nominal and worst-case estimate for the project or better each task

* Program Evaluation and Review Technique (PERT): analyse and represent the activity in a project to illustrate the flow of events in a project
* PERT is a method to evaluate the time required to complete a task within deadlines, also cost.
* PERT involves following steps

	1. Identifying Tasks and Milestones. 

		* Every project involves a series of required tasks. 
		* These tasks are listed in a table allowing additional information on sequence and timing to be added later
	2. Placing the tasks in a Proper Sequence
		* Tasks are analysed and placed in a sequence to get the desired results 
	3. Network Diagramming
		* A network diagram is drawn using the activity sequence data showing the sequence of serial and parallel activities 
	4. Time Estimating: this is the time required to carry out each activity, in three parts:
		1. Optimistic timing: the shortest time to complete an activity 
		2. The most likely timing: the completion time having the highest probability 
		3. Pessimistic timing: the longest time to complete an activity 
	5. Critical Path Estimating: 
		* Determines the total time required to complete a project
		
Wideband Delphi (e.g. Planning Poker) is an estimation procedure where several estimators iteratively work towards agreement. 
* Can be combine with PERT



## Chapter 11 - Pressure 


## Chapter 12 - Collaboration 
 

## Chapter 13 - Teams and Projects


## Chapter 14 - Mentoring, Apprenticeship and Craftsmanship 


## Chapter 15 - Applications and Tools
