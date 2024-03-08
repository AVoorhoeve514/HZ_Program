
HZ_Program
CheckersGame by Alwyn Voorhoeve and Arne Soyez

Repository: (https://github.com/AVoorhoeve514/HZ_Program)

Used Design Patterns:
Factory Method pattern
Composite pattern
Command pattern
Singleton pattern
Strategy pattern
In the development of CheckersGame, my teammate Arne and I implemented various design patterns to enhance the code's structure, readability, and maintainability. We adopted pair programming, with sessions primarily conducted on my computer, leading to most changes being pushed from my end.

Design Patterns
Factory Method Pattern:
Why: The Factory Method pattern is employed to manage the creation of game pieces (checkers).

What it does: In this checkers game, there's a CheckersPieceFactory class containing the logic to create checkers pieces. It provides a structured way to add new piece types without modifying the main program. This pattern makes it easy to incorporate new checker pieces in the future.

Singleton Pattern:
Why: The Singleton pattern ensures that there is only one instance of the game board (CheckersBoard).

What it does: In the checkers game, having multiple boards simultaneously is undesirable. The Singleton pattern ensures only one board exists, preventing confusion and errors. This pattern guarantees a unique instance of the board accessible from anywhere.

Strategy Pattern:
Why: The Strategy pattern is used for move validation logic in the game.

What it does: In the checkers game, moves need to be validated, and the Strategy pattern provides a way to define different strategies for validation. We've defined an interface called MoveValidator and concrete implementations for regular moves and jump moves. This allows easy switching between different move validation strategies in the game. It provides flexibility for future expansions, such as adding new types of moves.

Command Pattern:
Why: The Command pattern is employed to encapsulate the code of a move on the board.

What it does: In the checkers game, the Command pattern is used to represent a move as a command. For example, moving a piece from b3 to c4 is encapsulated as a command. This pattern provides a way to decouple the sender of the command from the object that performs the operation, allowing for easy extensibility.

Pair Programming and Collaboration
We began by listing all the requirements, such as the need for a board, two types of pieces, their movement, and the names of the board squares. Next, we identified design patterns that could enhance the project. We ensured mutual understanding before coding anything. We regularly switched between typing and reviewing, providing occasional breaks from continuous typing. Each piece of code was promptly reviewed to catch any overlooked errors.

If we encountered a problem, we discussed various solutions before choosing the most effective approach. We collaboratively implemented each design pattern, ensuring both team members contributed to the final solution.

Challenges and Herkansing
Despite our collaboration efforts, there were challenges due to communication issues with another person involved. As a result, I had to independently create this resit of the code. This process involved revisiting and refining the implemented design patterns and ensuring that the code met all specified criteria. If it is sub-par it means it is because of that. I also couldnt access the github anymore since it is his, so i couldnt push to it. 

Conclusion
Through pair programming, the application of design patterns, and addressing challenges independently, we created an easily extensible version of CheckersGame. The design patterns, such as Factory Method, Singleton, Strategy, and Command, significantly improved the code's maintainability and flexibility. The collaborative approach and adaptation during herkansing underscored our commitment to delivering a robust solution.
