###Chapter 1

####1.1 
You are in charge of automating a multi-site architectural practice. The cost of developing the software has been estimated to be $530,000. Approx how much additional money will be needed for postdelivery maintenance of the software?

Approx. 75% of total budget is maintenance. 

So, if 25% is development., then 75% is 3x as much.

530000 * 3 = 1590000


####1.2
Is there a way of reconciling the classical temporal definition of maintenance with the operational definition we now use?

Classical "maintenance" is equivalent to modern "postdelivery" maintenance.


####1.3
You are a software engineering consultant. The chief information officer of a regional gasoline 
distribution corporation wants you to develop a software product that will carry out all the 
accounting functions of the company and provide online information to the head office staff
regarding orders and inventory in the various company storage tanks. Computers are required
for 21 accounting clerks, 15 order clerks, and 37 storage ... etc.. 4 weeks. 
What do you tell him?

Explain the need for a longer time frame:
-  The cost of post-maintenance makes it especially important
   to take time to develop a robust product.
-  To ensure a high-quality product, the team doesn't rush straight into but, but performs a significant amount of analysis.
   This is related to the catching of faults early, because the cost of a fixing a bug after release increases tremendously. 
Explain that you cannot simply add more developers either,
-  The mythical man-month.


####1.4
You are a vice-admiral in the Velorian Navy. It has been decided to call in a software development organization to develop the control software for a new generation of ship-to-ship missiles. You are in charge of supervising the project. To protect the government of Veloria, what clauses do you include in the contract with the software developers?

-Rigorous testing would need to performed before field utilization.
-The requirements should be rigorously drawn up. No payment if not met.
-The team should use coding standards that can be verified by a third party for secure code.
-The Valerian government owns all documentation and artifacts, even if development is cancelled.

-Acceptance criteria must be stipulated: software shall meet specifications, be delivered on time, within budget, faults fixed for free for a year, documentation full and complete, source code included.


####1.5
You are a software engineer whose job it is to supervise the development of 1.4 project. 
List ways your company can fail to satisfy the contract with the navy.

Analysis do not reflect requirements -> The implementation will not either. Too many developers may be assigned to the team -> Development stalls. 
Documentation proves insufficient for maintaining standards compliance.


####1.6
Nine months after delivery, a fault is detected in the software a product. Fix cost 18,900.
Approx how much would it have cost during analysis phase?

$154.
From figure 1.6, ratio of cost of postmain fix to analysis fix is 368 to 3 
which equals 123 to 1.

18900 / 123 = 153.6585


####1.7
Suppose that it had been found in the implementation phase.. how much to fix?

$2700

Ratio is approx 7 to 1, 
18900 / 7 = 2700


####1.8
You are the president of an organization that builds large-scale software. You show fig 1.6 to your employees, urging them to find faults early in the software life cycle. Someone responds that it is unreasonable to expect anyone to remove faults early... if it is a coding fault. How do you respond?

60 to 70 percent of all faults detected in large projects are req, analysis, design faults.
Many of these are only noticeable in implementation. Coding is the manifestation of these earlier phases.
By strengthening the quality at earlier stages, coding faults will be much easier to avoid. 


####1.9
Describe a situation in which the client, developer, and user are the same person.

1) A game developer creates an engine for future projects. He is the client as the program is only for him 
or his team. He is the developer as he is creating it. He is the user as he will create games with it.

2) A physicist creates a simulator to test a theory. 

3) A Linux nerd submits a pull request.


####1.10
What problems can arise if the client, user, developer are the same purpose? 
How can these be solved.

May feel less inclined to documentation because he knows how he will use it. 
   Solution: Enforce standards anyway.

May lack portability as it was designed for a specific environment.
   Solution: Develop as if it were for a larger audience.

   
####1.11
What potential advantages acru if the client, developer, and client are the user?

Personal satisfaction of creating something relevant may increase quality.

No trouble of misunderstanding requirements between dev and client, and the needs
are clearly apparent to the developer. 

Budgets and expectations more reasonable, as the client is familiar with the development needs.


####1.12
Look up the word 'system' in a dictionary. Write down those that are related to software engineering.

1. an assemblage or combination of things or parts forming a complex or unitary whole: 

2. any assemblage or set of correlated members: 

3. an ordered and comprehensive assemblage of facts, principles, doctrines, or the like in a particular 
      field of knowledge or thought: 

4. a coordinated body of methods or a scheme or plan of procedure; organizational scheme: 

5. any formulated, regular, or special method or plan of procedure: 

6. due method or orderly manner of arrangement or procedure: 

11. a method or scheme of classification: 

15. Computers. a working combination of hardware, software, and data communications devices.


####1.13
It is your first day at your first job. Your manager hands you a program listing and says, "see if you can find the bug". What do you reply?

"What is the program intended to do?". Ask for documentation/specifications.


####1.14
You are in charge of developing the product in problem 1.1.
Will you use the object-oriented paradigm or classical?

The OO approach would be better suited to handling potentially changing requirements.
The objects could be used to model the environment, and provide a moduler system that would allow easier postmaintenance. 


Instead of implementing component c9 if a software product, the developers decide to utilize a COTS component with the same specifications as c9. What are the advantages and disadvantages?

Disadvantages:
- As a closed source product, may not be suitable modular for ongoing development.
   As requirements change, this COTS module will not. 
- May not integrate as cleanly.
- May cost more money than just coding it
- May incur additional cost on client if they have to buy this software
- Trusting that the company will continue to exist and support the product


####1.16
Instead of implementing component c37 of a software product, the developers decide to utilize an open-source component with the same specifications as c37. What are the advantages and disadvantages?

Advantages and disadvantages largely depend on the quality and active support of that module.

Advantages:
- If the component is popular, they will be implementing a more standardized approach.
- May have been thoroughly reviewed by a large number of testers.
- May be actively maintained in such a way that it continues to expand and support the postdelivery maintenance. 
- May save money, time
- If need be, team can take over development of the component even if the original contributers cease. 

Disadvantages:
- If the component quality is poor, the advantages disappear.
- The coding style may differ significantly from the rest of the product
- May not integrate as cleanly with the rest of the product.


####1.17
Object P invokes method m1 of object Q....

It is easy to make a system of objects that are heavily dependent on each other and the supposed portability and reusability of OOP goes away.


####1.18
Is it correct to say that, as a result of Linus's Law, all open source software is of high quality?

No- only that it has the potential to be. The quality of open source is entirely dependent on the level of interest in that project and amount of support. 



###Chapter 2


####2.1 
Represent the Winburg mini case study of Sections 2.2 and 2.3 using the waterfall model. Is this more or less effective than the evolution-tree model? Explain your answer.

In the waterfall model:

( null ) -> Requirements -> Analysis -> Design -> Implementation
					^---------|   ^-------|  ^-------|
	
This model shows that the steps were followed, and feedback loops utilized, but does not  capture the order of events as seen in the evolution-tree model. Does not give a clear picture of  what actually happened in development.


####2.2 
Assume that the programmer in the Winburg mini case study had used single-precision numbers from the beginning. Draw the resulting evolution tree.

(Just remove episode 2 from fig 2.2)


####2.3 
What is the connection between Miller's Law and stepwise refinement?

Miller's law states that humans can concentrate on approximately 7 things.
Large software project have much more than 7 components.
Stepwise refinement prioritizes certain aspects, while temporarily abstracting others.
The developers can construct the most critical artifacts, then the next most critical, etc.


####2.4 
Does stepwise refinement correspond to iteration or incrementation?

Incrementation, as it involves incrementally considering further requirements. 


####2.5 
How are a workflow, an artifact, and a baseline related?

A **workflow** describes one of the core activities of development. 
The five core workflows are requirements, analysis, design, implementation, and test.
An **artifact** is one of many kinds of tangible by-product produced during the development of software. Some artifacts (e.g., use cases, class diagrams, and other UML models, requirements and design documents) help describe the function, architecture, and design of software.


####2.6 
What is the connection between the waterfall model and the iterative-and-incremental model?

For each increment a ... n, the phases of the waterfall model correspond to core workflows that may be performed in variable capacity. For example, Increment a may focus heavily on requirements and analysis, while Increment d is concerned with implementation and test.
Testing is the one workflow, if done correctly, guaranteed to be performed within every increment.


####2.7 
Suppose you have to build a product to determine the cube root of 9384.2034 to four decimal places. Once the product has been implemented and tested, it will be thrown away. Which life-cycle model would you use? Give reasons for your answer.

Code-and-fix. Requirements, analysis and design appear to be overkill, and there is no concern for documentation that would aid post-maintenance.


####2.8 
You are a software engineering consultant and have been called in by the vice-president for finance of a corporation that manufactures tires and sells them via its large chain of retail outlets. She wants your organization to build a product that will monitor the company's stock, starting with the purchasing of the raw materials and keeping track of the tires as they are manufactured, distributed to the individual stores, and sold to customers. What criteria would you use in selecting a life-cycle model for the project?

The client has a variety of specific needs. Initially, I would use Rapid Prototyping to ensure that the product being developed represents that actual requirements. Then, perhaps agile would be effective to quickly bring usable components as agile "stories" reach fruition. 

This sounds a lot like the types of applications currently done by start-ups using agile methods. For example, my brother is working with a small dev company in Eugene, Oregon to build a web app for managing grocery co-ops.


####2.9 
List the risks involved in developing the software of Problem 2.8. How would you attempt to mitigate each risk?

Moving target:
The client seems to want a "do-it-all" application, which may manifest in "moving targets" further into production. Agile might be quicker to respond to these changes, or even bring about these changes earlier through frequent client interaction.

Post-maintenance:
This application sounds like it will be interfacing with a variety of existing entities. Changes made to these entities may be a burden on the product's future. Try to work with the client to minimize the number of outside components that must be depended upon. Ensure that all components are either from trusted brands (that hopefully will stick around), use standardized interfacing such as ATAPI or POSIX  that will facilitate adoption to alternatives, or is at least open source so that the developers can take over the code if need be.


####2.10 
Your development of the stock control product for the tire company is so successful that your organization decides that it must be reimplemented as a package to be sold to a variety of different organizations that manufacture and sell products via their own retailers. The new product must therefore be portable and easily adapted to new hardware and/or operating systems. How would the criteria you use in selecting a life-cycle model for this project differ from those in your answer to Problem 2.8?

Whereas I chose Agile for Problem 2.8, the stricter requirements of this Problem may be better served with a more formal model. Iteration and Incrementation would allow the developers to focus first and the most important platforms, but incrementally adapt. Also, to serve the needs of a large number of  clients, each increment could employ further requirements analysis with new (or existing) customers
to refine the product and appeal to broader audiences. 


####2.11 
Describe the sort of product that would be an ideal application for open-source software development.

For open source software to be successful, it usually has to appeal to those individuals who  contribute to open source. Operating systems, databases, compilers, text editors, "core utils", thread libraries, etc all appeal to developers. The OS guys can spend days on mailing lists arguing minute details
and whether or not a particular system call is "harmful". 

Scientific applications also benefit greatly. Many physicists and mathematicians are writing code in an academic setting, rather than a commercial one. The software are byproducts of research, and it makes sense for them to be released for free. By opening the source code, scientific progress is encourages, and facilitates reproducibility of results.


####2.12 
Now describe the type of situation where open-source software development is inappropriate.

If the selling the software itself, rather than supporting services, is the product, then it cannot be released free of charge. Technically, open source software can still be sold, but there is little point if the first buyer has the right to dump the code on the web. 


####2.13 
Describe the sort of product that would be an ideal application for an agile process.

From the book, it is smaller projects such as web applications, mobile apps, and interfaces that work best. 
Agile seems appropriate for fleeting, creative projects, where less rigor is required. However, companies such as USAA are challenging that view with a push for widespread adoption.


####2.14 
Now describe the type of situation where an agile process is inappropriate.

Can't really agile working in a massive-scale product with large amounts of strict documentation and small modules being developed by a large number of programmers.
For example, agile does not seem as appropriate for VMware.

####2.15 
Describe the sort of product that would be an ideal application for the spiral life-cycle model.

Maybe the development of cutting-edge (thus risky) in-house research projects into, for example, novel HPC architectures by IBM. They would be closely monitoring progress to ensure that money is not being poured into a useless project.


####2.16 
Now describe the type of situation where the spiral life-cycle model is inappropriate.

In any contract software, termination is not so readily resolved. 


####2.17 
Describe a risk inherent in using the waterfall life-cycle model.

The final product may not be "what the developer wanted", despite seemingly what was requested.
The model is not able to adapt quickly to meet changing requirements and accept new approaches.


####2.18 
Describe a risk inherent in using the code-and-fix life-cycle model.

Unlikely to satisfy anyone needs, and wholly unequipped for expansion or revision.


####2.19 
Describe a risk inherent in using the open-source life-cycle model.

Scenario 1)
Someone submits a pull request that changed all documentation's use of pronounce into gender-neutral alternatives. The core team thinks "what in the world?", and rejects it. Goes viral on Tumblr that the patriarchy is using software to trample on minority rights.

Scenario 2)
Too many forks are created, and users and contributors have trouble knowing which to use. Community becomes fragmented and a clear vision of the product is lost; some versions have features that others don't, etc. See: the overwhelming number of special interest Linux distros.

[User1]
"Hi all. This is my first post on the OSDev forums. I just created a new Distro I want to share called 'Archbang' because it combines the WM and aesthetics of Crunchbang with the package management of Arc"

[User2]
"Not bad mate. I just used it to release my own spin-off called 'Archbang-sec' that includes a suite of preconfigured security tools and anti-authoritarian wallpapers"


####2.20 
Describe a risk inherent in using agile processes.

The manifesto and "too cool for waterfalls" attitude empowers the coders to take control over the means of production
and revolt. CEO is publicly executed with an ethernet cable that was lying around. "Its a whole new paradigm", indeed.


####2.21 
Describe a risk inherent in using the spiral life-cycle model.

It is built around risk-analysis, but this is only helpful if the team is sharp enough to detect these risks.
It does not automatically reveal the risks. 

###Chapter 3

####3.1    
Define the terms software process and Unified Process

"Software Process" describes the entirety of the methodologies, life-cyle models, techniques, tools, and individuals. 

"Unified Process" actually refers to a subset of the software process; the primary object-oriented methodology currently in use.
It a large scale system, much of which is only applicable to massive software products.
However, the 5 core workflows are applicable to almost all:
Requirements, Analysis, Design, Implementation, and Testing.



####3.2  
In the software engineering context, what is meant by the term model?

A model is a set of UML diagrams that represent one or more aspect of the software to be developed. Via its graphical nature, facilitates quick and accurate communicating of information.



####3.3  
What is meant by a phase of the Unified Process?  

A phase is a distinct instance of an increment, but given the titles "Inception Phase", "Elaboration Phase", "Construction Phase", and "Transition Phase".



####3.4  
Distinguish clearly between an ambiguity, a contradiction, and incompleteness.  

Ambiguity: language in which the exact meaning may not be clear.
   Includes language such as "it", where one it expected to intuitively interpret what "it" is.
   Adjectives such as "big", "charming", and "troublesome" are also ambiguous.
   
Incompleteness: Omissions of relevant details. 

Both of the above are instrinsic properties of natural languages.

Contradiction: Differing factual statements.



####3.5  
Consider the requirements workflow and the analysis workflow. 
Would it make more sense to combine these two activities into one workflow than to treat them separately?  

No, because the address 2 different needs. Th Requirement's intent is to create an understanding between the client and development company. For this purpose, the use of natural languages is appropriate and is concerned with what the product -is-, rather than -how- it is. 

The analysis workflow converts the results of the requirements phase into an exact understanding.
This workflow exactly described the product specifications, functionality, as well as what CASE tools, techniques, and methodologies will be employed.



####3.6  
More testing is performed during the implementation workflow than in any other workflow. 
Would it be better to divide this workflow into two separate workflows, one incorporating the nontesting aspects, the other all the testing?  

Splitting it up may deemphasize the importance of testing being done in conjunction with all workflows. 



####3.7  
Correctness is the responsibility of the SQA group. Discuss this statement.  

Programmers are concerned with the implementation of the artifacts of the previous phases; it is not their job to ensure that the implementation is correct.



####3.8  
Maintenance is the most important activity of software production and the most difficult to perform. Nevertheless, it is looked down on by many software professionals, and maintenance programmers often are paid less than developers. Do you think that this is reasonable? If not, how would you try to change it?  

It is not reasonable because maintenance is what keeps a software product relevant and useful.
All the work of the original development is nullified if no maintenance is performed.
Maintenance is not merely fault-correction, but provides new features and supports additional environments.


####3.9  
Why do you think that, as stated in Section 3.9, true retirement is a rare event?  
  
Software tends to be relied on more, rather than less. It would normally be desirable for the software to continue to be reliable and relevant rather than abandoned to purchase something new.

  
  
####3.10  
Because of a fire at Elmer's Software, all documentation for a product is destroyed just before it is delivered. What is the impact of the resulting lack of documentation?  

Only the code remains from which to learn how the software works. All would have to carefully analyzed to understand the inner workings: making postmaintenance practically impossible.

Also, having lost the requirements and analysis, it cannot be determined how effectively the client's needs are realized. 




####3.11  
You have just purchased Antedeluvian Software Developers, an organization on the verge of bankruptcy because the company is at maturity level 1. What is the first step you will take to restore the organization to profitability?  

Try to implement some software engineering methodologies. 
In the short term, the transition will be chaotic and will be difficult to enforce highly structured techniques without disruption. May use some level of agile processes during this time; their adaptability and frequent communication may help all parties involved better react to and quickly internalize new policies and unexpected situations.



####3.12  
Section 3.13 states that it makes little sense to introduce CASE environments within organizations at maturity level 1 or 2. Explain why this is so.  

CASE tools promote quality and productivity, but more so in environments that enforce standards and methodologies. The CASE tools often involve entities such as version control, UML, and online interface checkers that are lacking within level 1 & 2 environments.



####3.13  
What is the effect of introducing CASE tools (as opposed to environments) within organizations with a low maturity level?  

CASE tools may be critical in structuring these nonstandardized environments. Implementing version control, testing suites, etc may lead to more stable and productive development.



####3.14  
Maturity level 1, the initial level, refers to an absence of good software engineering management practices. Would it not have been better for the SEI to have labeled the initial level as maturity level 0?  

I understand that you are implying that they "are not even 1 level of maturity", but whether they start counting at 0 or 1 is largely insignificant as long as the numbering system is known.



###Chapter 4

####4.1  
How would you organize a team to develop a payroll project? Explain your answer.  

As a payroll system is quite established at this point, the exploratory nature of the democratic team seems less applicable. Agile could be used, but chief programmer team may be ideal.
The possibilities of information leaking and other vulnerabilities make testing especially critical. Having someone handle test cases, documentation, etc would be great, while the chief focuses on a carefully designed application.



####4.2  
How would you organize a team for developing state-of-the-art military communications software? Explain your answer.  

This would be a perfect case for the democratic team. In a perfect situation, you would have a variety of skilled developers from a multitude of fields and experiences. Radio experts, signal processing, low-level systems programmers.. The environment should promote open communication and sharing of ideas and considerations of novel approaches. 



####4.3  
State Brooks's Law. Explain why it holds.  

As is elaborated in Brook's 'The Mythical Man-Month', adding more developers increases the number of persons to bring up to speed and communicate with. More interfacing and version controls issues arise.



####4.4  
You have just started a new software company. All your employees are recent college graduates; this is their first programming job. Is it possible to implement democratic teams in your organization, and if so, how? 

It is not ideal to have no experienced developers, but a democratic team seems reasonable. The environment could be an extension of that on campus, but more rigorous. As each employee will have pursued different interests and research areas during school, this may allow them to voice ideas that might not have come about if they were boxed into highly specific tasks.



####4.5  
A student programming team is organized as a democratic team. What can be deduced about the students in the team?  




####4.6  
A student programming team is organized as a chief programming team. What can be deduced about the students in the team?  




####4.7  
To compare two different team organizations, TO1 and TO2, within a large software company, the following experiment is proposed. The same software product will be built by two different teams, one organized according to TO1 and the other according to TO2. The company estimates that each team will take about 18 months to build the product. Give three reasons why this experiment is impractical and unlikely to yield meaningful results. 




####4.8  
The company you own has just taken over a smaller competitor, and you discover that one of their programmers is a superprogrammer. How do you ensure that she does not leave and take a job in another company?  




####4.9  
Why do teams for agile processes have to share a computer?  




####4.10  
What are the differences between a democratic team and an open-source team?  




####4.11  
How would you organize an open-source team?  




####4.12  
Would you like to work in an organization that uses synchronize-and-stabilize teams? Explain your answer.  



####4.13  
Which team organizations conform to PCMM?  
