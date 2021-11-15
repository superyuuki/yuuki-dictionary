# yuuki-dictionary
Big words for small brain

# disclaimer
Don't depend on the accuracy of these, they are here to help newbies wrap their head around really abstract and hard concepts.
This exists to help me (and people like me) to understand coder jargon that gets thrown around a lot that may confused newbies.

Lots of java stuff since i write java mostly (some rust)

if some asshole in a discord is speaking hundreds of words you don't get when you're literally just trying to write a minecraft mod, open this readme and press Ctrl + F to find the word.

things in <brackets> - something you can Ctrl + F to find more info on

# words
- state - TODO explain this one better - whether something has been created and can be modified or not.
- semantics - little details about something
- concurrency - does it utilize multiple threads?
- parallel - does it do more than one thing at a time
- asynchronous - does it do things out of order
- synchronous - does things in order 
- mutable - it changes state, it can be modified
- immutable - it does not change state, it cannot be modified, safer
- protected keyword - can be inherited. don't use this.
- private keyword - can only be accessed by current instance of current class (OOP). Safe.
- final keyword - it does not change. Makes things immutable.
- static keyword - you can access it from anywhere regardless of if an object exists or not. bad.
- thread - something that runs your code. See why it's unsafe if you have two things running your code and changing things at the same time?
- caching - storing a value in memory(somewhere you can access easily) after a lengthy operation so that it does not take as long to access in the future
- reflection - uses java's internal unsafe stuff to look at parts of your code that you didn't explicitly say should be read
- jvm - java virtual machine, literally a virtual machine where your code is run
- memory - your computers memory, stuff is stored there.
- reference - tells you where an object is. 
- atomic - TODO explain this one well
- cas - compare and swap. Basically get something, make a local modification to it, check if it's still the same in volatile memory (this seems like a no brainer but threads are - evil) and if it is, do the modification. Otherwise, try again.
- threadsafety - sometimes things go wrong when two threads are accessing the same thing due to how computers store data. threadsafety is when you explicitly counter this with    - design and code
- synchronization - making sure that access to something that is mutable (can change) from multiple threads is done safely
- locking - a way of making sure code with multiple threads functions safely by limiting access to something to one thread at a time. Slow.
- mutex - mutual exclusion: only one thing at a time. locking is mutual exclusion of threads. Stupid malware devs advertise 'mutex', they mean only one instance of their shitty    virus is open at one time.
- encapsulation - controlling access to data. Contrary to what your teacher tells you, getters and setters are not encapsulation.
- dependency injection - setting the state (modifiable part) of an object via a constructor (at initialization of the object) rather than after the object already exists. 
- when talked about with higher level developers, they typically mean dependency injection frameworks.
- dependency injection framework - a framework that manages the creation of objects and insertion of those objects into the right slots via the constructor in your code.
- constructor - a special reserved method you can call with the `new` keyword that lets you insert objects that will be used by your object.
- learn java (in a sarcastic tone) - something stupid that insecure paperspigot developers like to tell newbies who are trying to write block game mods. Don't listen to them,you   are learning java as you write. Just focus on getting better as you go, your first code will be shit, that's how it is for everyone.
- abstraction - hiding how a service works from the users of the service, helps make the services interchangeable since you don't depend on the services in the background
- polymorphism - it has multiple shapes: if something is a Duck it fits in any spot an Animal would
- oop - object oriented programming - thinking of your code as objects. a class Duck can quack() and maybe walk(). oop is a good idea but in practice it kind of sucks.
- framework - bundle of useful stuff you can use to make things.
- multithreading - uses lots of threads. contrary to popular belief, making things multithreaded is not always a good idea: creating threads can be slow.
- overhead - slowdown introduced by something
- javadocs (read the) - documentation written directly in the source code. If someone tells you to read the javadocs, they are lazy and/or don't actually know how the application they are providing support for works.
- documentation - developer comments on how their application works
- source code - the code used to make the project.
- open source - anyone can see the source code of a project. this is always a good thing, if anyone tells you otherwise they are greedy or insecure. (or writing malware)
- sql - structured query language. A language written to describe how structured databases (think a microsoft excel csv sheet one of those big fuckin tables) are created and how to get data from those databases.
- mysql - an implementation of <sql> that is stored on a remote server. go-to for people who don't know about mariadb.
- mariadb - updated better version of mysql. go-to.
- - sqlite - type of <sql> that is stored on a local file. you'll see the database itself as a file ending with .sql.
- h2 - type of <sql> that is fast and is stored on a local file. no one uses this (?)
- implementation - the details of how something works or is made to work.
- git - a system that lets you control what changes are made to your code and organize them. Helps make it easy to have many people working on something.
- github - cool place to store code using <git>.
- git repository - a remote place where your code is stored
- gitlab - another cool place to store code
- todo - something you need to do, like perhaps alphabetizing yuuki-dictionary?
- pr - pull request - a request to make modifications to someone else's code base. typically a request to merge one branch into the other
- branch - a collection of changes to a git repository
- merge (git) - combine changes from one branch into another
- maven - a build system which handles compiling your application and managing other projects that your project depends on cool.
- gradle - another build system which handles compiling and dependencies.
- maven repository - a remote place where code is stored. Like <git repository>, but for finished code. 
- maven central - the biggest bestest most fucking swaggy repository for <open source> useful code.
- server - big remote computer that handles requests from lots of things that depend on it (clients)
- client - something that makes requests to a server
- api - application programming interface or some shit - basically an "official" way to access someone elses' code and integrate it with your own
- spi - service provider? programing interface - something that is meant to be <implement>ed by your application.
  interface - a collection of functionalities that can be <implement>ed. these hide how your program actually works so that you could change it and anyone using the interface     does not have to change their code.
- classpath (java) - where all your code is loaded to once your application's compiled jar file is run/loaded. 
- ide - integrated development environment - where you write code. Like notepad but souped up so it can provide you help with errors and also compile your code, etc
- eclipse - old outdated ide. like a cow in terms of how fast you can make stuff with it.
- intellij (idea) - super fast and modern ide. very fast, has lots of integrations with all sorts of tools, themable to a good degree, overall high quality
- recursive - something that may activate itself or something similar to itself (which will in turn activate another thing like itself), which could happen infinitely.
- nodes - recursive data structures.
- groupId - the url representing you or your organization, like com.superyuuki for me, yuuki, and superyuuki.com, or gg.solarmc for the solarmc network at solar.gg. Used to
  group everything you or your organization under one string.
- artifactId - the name of your project.
- package (java) - the path to your project in terms of reverse url, like com.superyuuki.someStupidProject
instance - a distinct copy of an object. If Person is an object, me existing in the world i am an instance of a person. probably the baby someone is thinking about having does
  not exist, so it is not an instance of a person.
- shade - shading - shadowing - inserting a full copy of a project that your project needs into the finished jar file.
- serializer - something that converts an object or data into more concise and storable data
