# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
The first time I ran the game, when I try to guess and guessing the game, it always shows the hint "Too low!" even if the guess is too high. The game doesn't seem to be responding to my inputs correctly, and it feels like it's stuck in a loop of giving the same hint regardless of what I do. What's more, when I try to start a new game, the game doesn't reset properly, and it continues to give the same hint from the previous game instead of starting fresh. This made it clear that there were some issues with how the game was handling user input and managing its state.
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").
  1. The hints were always "Too low!" regardless of whether the guess was too high or too low.
  2. The game did not reset properly when starting a new game, causing it to continue giving the same hint from the previous game instead of starting fresh.

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
ChatGPT was the AI tool I used for this project. I used it to help me understand the code and identify potential bugs. I asked ChatGPT specific questions about the logic of the game and how it handles user input, which helped me pinpoint where the issues might be occurring. Additionally, I used ChatGPT to get suggestions on how to fix the bugs once I identified them, which was helpful in guiding my debugging process.
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- I used ChatGPT as an AI tool for this project. I asked it for help in understanding the code and identifying potential bugs. One example of an AI suggestion that was correct was when I asked ChatGPT about the issue with the hints always being "Too low!" It suggested that there might be a problem with the logic that determines the hints, specifically that the conditions for checking if a guess is too high or too low might be reversed. I verified this result by reviewing the code and found that indeed, the conditions were reversed, which explained why the hints were always incorrect. After fixing the logic, I ran the game again and found that the hints were now accurate, confirming that the AI's suggestion was correct.
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
I try to run the code test because I have some issue starting the test, I ask ChatGPT for help. It suggested that I might need to install pytest and provided me with the command to do so. However, when I ran the command, it didn't work because I was using a virtual environment that already had pytest installed. This was misleading because it made me think that there was an issue with my environment setup when in reality, the problem was that I was trying to install something that was already there. I verified this by checking my virtual environment and confirming that pytest was indeed installed, which showed me that the AI's suggestion was not applicable in my specific situation.
---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
To decide whether a bug was really fixed, I ran the game multiple times after making the changes to see if the issue persisted. For example, after fixing the logic for the hints, I played several rounds of the game, making different guesses to see if the hints were now accurate. I also tried starting a new game to ensure that the reset functionality was working properly. If the game responded correctly to my inputs and provided accurate hints consistently, I considered the bug to be fixed. Additionally, I looked for any error messages in the console that might indicate if something was still wrong with the code. Lastly, I run the test file and all test passed, which gave me confidence that the bugs were indeed fixed.
- Describe at least one test you ran (manual or using pytest) and what it showed you about your code.
One test I ran was a manual test where I played the game and made a series of guesses to see if the hints were accurate. I started a new game and made a guess that was too low, expecting to see the hint "Too low!" Then, I made a guess that was too high, expecting to see the hint "Too high!" Finally, I made a correct guess to see if the game recognized it and provided the appropriate response. This manual testing helped me confirm that the logic for providing hints was working correctly after I made the necessary fixes. Additionally, I ran the pytest tests that were provided with the project, and all tests passed successfully, which further confirmed that the bugs were fixed.
  

- Did AI help you design or understand any tests? How?
Yes, AI helped me understand how to design tests for the game. I asked ChatGPT about best practices for testing in Python and how to use pytest effectively. It provided me with examples of how to write test functions and what kind of assertions to use to check the expected outcomes. This guidance helped me structure my tests in a way that was clear and effective for verifying the functionality of the game. Additionally, when I encountered issues with running the tests, I asked ChatGPT for troubleshooting advice, which helped me resolve those issues and successfully run the tests to validate my fixes.

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
Streamlit "reruns" refer to the way Streamlit automatically re-executes the entire script from top to bottom whenever a user interacts with the app, such as clicking a button or entering input. This means that every time you make a change or interact with the app, it starts fresh and runs all the code again. Session state is a way to preserve certain values or data across these reruns. It allows you to store information that you want to keep track of, such as user inputs or game state, so that even when the app reruns, you can access and use that information without losing it. This is particularly useful for applications like games or forms where you need to maintain state across user interactions.

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
The habit I want to reuse in future labs or projects is the practice of asking specific questions to AI tools like ChatGPT to help me understand the code and identify potential issues. This approach allows me to leverage AI as a resource for learning and problem-solving, which can be especially helpful when I'm stuck or unsure about how to proceed. By being specific in my questions, I can get more targeted and useful responses from the AI, which can guide me in the right direction and save time during the debugging process. Additionally, I want to continue using AI to get suggestions for improving my code and testing strategies, as it can provide valuable insights that I might not have considered on my own.
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
One thing I would do differently next time I work with AI on a coding task is to be more critical of the suggestions provided by the AI and to verify them more thoroughly before implementing them. While AI can be a powerful tool for generating ideas and solutions, it's important to remember that it can also provide incorrect or misleading information. In the future, I would take the time to cross-check the AI's suggestions with my own understanding of the code and possibly consult additional resources to ensure that the advice is sound before making changes to my code. This would help me avoid potential pitfalls and ensure that I'm making informed decisions based on accurate information.

- In one or two sentences, describe how this project changed the way you think about AI generated code.
This project made me realize that while AI-generated code can be incredibly helpful for understanding and solving problems, it's not infallible and should be used as a tool rather than a definitive source of truth. It highlighted the importance of critical thinking and verification when working with AI suggestions, as well as the value of using AI to enhance my own problem-solving skills rather than relying on it completely.
