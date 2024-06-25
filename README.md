# CS230
coursework for CS230 Operating Platforms

*** Briefly summarize The Gaming Room client and their software requirements. Who was the client? What type of software did they want you to design?

Our client, The Gaming Room, had an existing web based game modeled after the classic tv game show “Win, Loose or Draw” which was similar to the home game Pictionary.  In their web game, teams would try and guess an image as it slowly renders to full resolution over 30 seconds.  Their requirements were as such:
          Web Based – the game must be available to all internet users. 
          The game will consist of one or more teams.
          Each team will consist of multiple players.
          Game name and Team names must be unique.
          Users will be able to check if a name already exists.
          Only one instance of the game service can exist in memory at a single time.  
Once these requirements were identified we outlined the challenges we would have (design constraints) and proceeded to research the various technologies available that would meet our needs and what the benefits and drawbacks were for each.  We ended the document with our final recommendations.  



*** What did you do particularly well in developing this documentation?

Creating this document was right in my wheelhouse.  I have extensive experience explaining technology to non-technical people and I have a extensive experience listing to members of a system or process, figuring out what is wrong, what’s not working, and what their ideal situation would be. Taking that information and developing a technology plan is much more interesting to me than the intricicies of code.  However I believe that in order to do that well, you need a good foundation in multiple languages and technologies.  

*** What about the process of working through a design document did you find helpful when developing the code?

Working through the design document really gives you a sense of how gameplay will work (in the clients vision) and with that knowledge you can focus your code on what meets the clients needs and vision and not waste time on features that they are not asking for, regardless of how beneficial you feel they would be. 


*** If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?

Honestly I’m very pleased with the content of the document,  however if I had to change one aspect I would change the evaluation.  I am not a fan of the layout and I don’t believe it makes comparing each platform easier due to the lack of space.  I would change this to a nested bulleted list. 


*** How did you interpret the user’s needs and implement them into your software design? Why is it so important to consider the user’s needs when designing?

I took the key points that the client needed from the game and determined which code would be needed to meet those requirements.  As I mentioned earlier sticking to the clients needs makes your work more efficient.  If in the process you can make additional recommendations for improvements, and those improvements are approved by the client, along with the additional costs, that’s fine, but initially you are being hired for a specific task and that is what the client is paying for.  Keeping that in focus is a good model for success. 


*** How did you approach designing software? What techniques or strategies would you use in the future to analyze and design a similar software application?

Once the clients requirements were identified,  I knew that setting up a singleton pattern would prevent multiple instances of the game service to exist in memory at any one time.  The player and game management were handled with an iterator pattern  which would check to make sure that no duplicate names were existing at any one time.  Lastly we incorporated the use of a superclass “Entity” which would allow for easier expandability and would simplify the code.  
