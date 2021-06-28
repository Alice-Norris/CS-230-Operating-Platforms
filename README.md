# CS-230-Operating-Platforms

1. Briefly summarize The Gaming Room client and their software requirements. Who was the client? What type of software did they want you to design?

The client, The Gaming Room, wanted to deploy their game that currently exists as an Android app as a web application across multiple platforms. Although the core game itself already exists, The Gaming Room needed te set up an environment from which the game could run and be accessed by users. Their requirements included the ability to have multiple uniquely identified and named teams participate in individually named and identified games, with checks to ensure that there are no duplicate team names. Teams could be composed of multiple players, which also had to be uniquely identified to make sure only one instance of the game exists in memory at any time.

2. What did you do particularly well in developing this documentation?
  
  I think I did well with the analysis of pros and cons for each platform for both the server and client purposes, as well as development tools for each. My experieince with all of the referenced platforms was very helpful, although research was still required, especially with the specifics of AWS.
  
3. What about the process of working through a design document did you find helpful when developing the code?
  
  The executive summary, design constraints, and domain model were all extremely helpful when developing the application. Restating and explicitly listing the consequences of the requirement in the domain model made what needed to be achieved in the code much clearer. The domain model was perhaps the most useful, as it clearly explained the logical structure of the progoram. 
  
  
4. If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?
  
  I would probably rework the entire executive summary. I'm not sued to writing in a declarative tone, and so offered options where more certain statements would've been more fitting. I attempted to correct this by reframing the sentences, but I'm still not happy with the way it turned out. I feel it would be best improved by starting over and structuring it from a more top-down, clear approach, starting with bigger pieces first. 

5. How did you interpret the user’s needs and implement them into your software design? Why is it so important to consider the user’s needs when designing?
  
  The user's needs were implemented by using a singleton pattern on the GameService class, which is in charge of creating new players, teams, and game instances. Doing so ensures that only one instance of it can exist, and that instance becomes the sole arbiter of game, team, and player instances. As a result, it is certain that there are no competing game, player, or team instances to coordinate. Each instance of games, players, and teams has a unique identifier assigned by the GameService singleton. Users' needs are of the utmost importance when designing software because software is an expression of an idea. As a developer, my job is to help make the idea reality. Their requirements and needs are the core of what the software will be.
  
6. How did you approach designing software? What techniques or strategies would you use in the future to analyze and design a similar software application?

  The design itself was done from an approach that is entirely new to me. Instead of starting from a whiteboard and making a design pattern of my own device, I read about existing, proven, and tested design patterns and used those, such as the singleton referenced in the implementation of user requirements. I also made sure to follow certain best practices, such as naming conventions, and tried to stick to style guides. Design patterns are incredibly useful, and I intend to acquire a reference of design patterns in general.
