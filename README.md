In a language of your choice, write a higher/lower game that satisfies the following criteria: 

- Generates a random number. 
- Takes in a guess. 
- Returns a string with the guess and whether that guess is lower or higher than the random number. E.g., “You answered 9. The correct answer is higher.” 
- If the guess matches the random number, then return a string which confirms this. E.g., “You answered 9. This is the correct answer!” 

This challenge (deliberately) does not give any guidance about ranges, input validation, presentation etc., so you are also required to explain any assumptions that you have made. This can be done using comments in the code or in a readme file, or both. 
You have one hour to complete the task and upload it to GitHub. This can be done any time before the interview. Please do not share answers or discuss with people who have not completed the challenge. 

----

This game asks the user to select a number from a slider, which is currently set to between 1 and 1000.
The user then clicks on the button "Play game!".
Once this button is clicked a sentence is displayed below the button, which states the outcome of the game.

---

Reflections:

- no set seed available for generating random numbers using Math.random(). Look into why this is, perhaps it has been taken care of within this function. See if there are other libraries for this. 
- hard coding the limit values for the user input number. these could be set elsewhere, perhaps read in from an environment file or a SQL database. Alternatively we could give the user the option to set the limits. This would alter their chances of winning or loosing.
- It would be good to add a test for selecting these limits. I manually changed the maxValue to 4000 whilst developing to see if this altered the values on the slider, which it did. A much better way to do this would be to test it using eg. Cypress.
- Also add a test that checks if the > and < are the correct way around in the logic for selecting outcome from the game. As well as if the numbers are equal (it is unlikely the two numbers are equal but important that it is correct).
- THe choice of the slider was initially because this is more visually appealling than a box where the user can write in a number. However, it is difficult to accurately select a number from this. In hindsight perhaps a box would be better so the user could input the number they were thinking of directly.


---
Screenshot of game whilst developing:
<img width="1706" alt="Screenshot 2025-03-20 at 17 55 12" src="https://github.com/user-attachments/assets/7d72710f-fa87-4ed3-9de0-ed84d4dacb5f" />
