# Homework: 20 Questions

## Goal  
To get some practice with:
- Binary tree traversal.
- Structuring data in a tree for decision-making.
- Console-based user interaction.
- Working with peers

## Objective
Apply binary tree structures to implement a decision-based guessing game that uses a question tree to deduce an answer based on user responses.

## Task:  
Write a C# console application that plays a simple "20 Questions" game with the user. The program should start with a few predefined questions in a binary tree structure. Each question should branch to two possible outcomes based on "Yes" or "No" answers, leading to more questions or a final answer.

## Requirements:  

These are things that I care that you implement as you develop the program. I'll be looking for them specifically when I grade. I suggest building out your program in baby steps, rather than coding it up all at once. This is how I would "chunk" out my feature implementation. I think it is important to think about planning like this. It is good to have it semi-guided now in a homework. In future project land, this type of feature "chunk" planning will be on you and your team. Instructor Nick won't be there to hold your hand. 

1. **Design a TreeNode Class**
   - We don't have a simple pre-defined C# class like `Stack` or `Queue` this time. But we can create our own custom class to help build out our cool tree.
   - Create a `TreeNode` class representing each node in the question tree.
   - Each node should store it's data and it's children, I would assume you'll build it something like:
     - Data (A question or answer) as a `string`.
     - A reference to a `Yes` child node object.
     - A reference to a `No` child node object.

2. **Build the Question Tree**
   - Start with a simple tree of at least 4–6 questions and answers.
   - Example structure:
     - "Is it an animal?" 
       - Yes -> "Does it have four legs?" 
         - Yes -> "Is it a pet?" 
           - Yes -> "It’s a dog!"
           - No -> "It’s a horse!"
         - No -> "Does it fly?"
           - Yes -> "It’s a bird!"
           - No -> "It’s a fish!"
       - No -> "Is it a vehicle?"
         - Yes -> "Is it a car?"
         - No -> "Is it a building?"

3. **Traverse the Tree Based on User Input**
   - Begin at the root question and ask it.
   - Based on the user’s input ("Yes" or "No"), move to the corresponding child node.
   - Continue until reaching an answer node.

4. **Multiple rounds**
   - Allow the user to play multiple rounds without restarting the program.
   - Prompt the user if they’d like to play again after each round.

5. **Learning**  
   - Allow the program to “learn” by expanding the tree with new questions and answers based on user feedback when it guesses incorrectly.
   - After a wrong guess, prompt the user to input a new question and answer to expand the tree.

6. **Saving**
  - Allow the program to save out the tree data to a file.
  - Load in the tree data via a file. 

**Example Console Output:**
```plaintext
Welcome to the 20 Questions Game!
Think of something, and I’ll try to guess it.

Is it an animal? (yes/no)
> yes
Does it have four legs? (yes/no)
> yes
Is it a pet? (yes/no)
> no
It’s a horse!
Would you like to play again? (yes/no)
> yes
```

## Reminders

That's all I have to say. Good luck and have fun! Remember to effectivly plan out the assignment with your squad and divide the task and area responsibilities. While hitting all re requirements above, don't forget about other things we have talked about in class such as comments, error handling, and propper object oridented programming.. aka POOP. :shit: :stuck_out_tongue_winking_eye: 

## Submitting

Don't forget to submit to the mycourses dropbox. See the assignment for submission guidelines and rubric.