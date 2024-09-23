This week your coding assignment has two parts again.  The first part is to continue your work on your Open API Project.  The second part is to work on debugging techniques.

## Open API Project
<details>
<summary>Click here to see Open API Project Instructions</summary>
<br>
This week, focus on accomplishing the following:

 - [ ] Start digging deeper on how you want to display content for either or both of the data points for your site. 
 - [ ] Start getting some basic styling built
 - [ ] Build your second fetch for your second data point (or adjust your code so clicking your navigation link for your second data point will change/update your fetch accordingly.

**_By the end of this assignment, you should have made additional progress on your Open API Project.  Since you have another assignment due this week, please submit your most recent pull request link in the "questions" field of your assignment submission form if you'd like your reviewer to check your work in progress._**
</details>

## Debugging Assignment
<details>
<summary>Click here to see Debugging Assignment Instructions</summary>
<br>

### Overview

The purpose of this assignment is to get you comfortable with reading already written code you're unfamiliar with, and let you practice debugging skills.  There are lots of helpful tools in programming that help alert you to something being "not right" in your code.  Before you start working through the Task List below, familiarize yourself with the code.  Try and walk through the code and add comments to help yourself understand what the code is doing currently.  You may even find and fix some bugs by looking through it first!  Then read through the Task List below and use developer tools to find and fix the bugs.  You may find it helpful to do your Mindset Assignment on debugging before starting this assignment.  Find and fix as many bugs as you can this week, and submit your work no matter how far you get with this assignment.  You'll have next week as well to continue working on finding and fixing the bugs/app.

### Getting Started

 - [ ] Fork [this GitHub repository](https://github.com/Code-the-Dream-School/intro-to-programming-debugging) to make a copy of it to your GitHub account.  You can do this by clicking the "Fork" button in the top right.
   - [ ] This opens a new page where you can retitle your copy of this repository to `yourname-debugging`
 - [ ] Once you've completed forking the repository, be sure you're looking at your copy (you should see your GitHub username in the top left, not Code-the-Dream-School). 
   - [ ] Click the green "Code" button, select "SSH" as the Local Clone type (not HTTPS or GitHub CLI), click the copy button (two overlapping squares icon) to copy your repository address. 
   - [ ] Your copied link should look like `git@github.com:yourUsernameHere/yourname-debugging.git` (EXAMPLE: a student named Maria Santiago would have this link `git@github.com:mariaDev/maria-santiago-debugging.git`)
   - [ ] Clone this repository so that the code is available on your local machine.
   **BE SURE YOU ARE NOT INSIDE YOUR LOCAL FOLDER FOR YOUR PORTFOLIO PROJECT WHEN YOU CLONE THIS REPOSITORY!**

### Get organized and review the code
 - [ ] Before you change any code, make a new branch to make your changes on by using the command `git checkout -b debugging`
 - [ ] Look at the code in index.html and index.js and add any comments to help you identify what sections of code are doing what.
 - [ ] Play with/practice with the game to see how it's behaving and take note of how you would expect it to behave.

### Task List:

The goal of this assignment is not to create a working application, but to practice debugging JavaScript using the browser developer tools. You should focus less on getting all the "right" answers and more on the process of troubleshooting each issue.

There are **at least 8 bugs** in this assignment, do your best to track down and fix as many as you can.

Below is a list of requirements explaining what the application should do:

- [ ] No errors in the browser console

> _**Note:** keep the console open as you play the game so that you can see the randomly generated "target number"_

- [ ] At the start, the "reset" button and all of the "messages" should be hidden

- [ ] You should be able to type a number into the input field and click "Submit Guess" to submit the form

- [ ] When the form is submitted, you should see the following:

  - [ ] A message displaying the number that was entered
  - [ ] A message displaying how many tries you have left (starts at 5 and decrements by 1)
  - [ ] A message describing the guess (too low, too high, etc.)
  - [ ] A "reset" button that restarts the game

- [ ] If the guessed number is BELOW the target, the message should say "too low"

- [ ] If the guessed number is ABOVE the target, the message should say "too high"

- [ ] If the guessed number is the SAME as the target, then:
  - [ ] The input field and "Submit Guess" button should be disabled
  - [ ] The message should say "guessed correctly"

- [ ] If the guessed number is not the same AND all 5 tries have been used, then:
  - [ ] The input field and "Submit Guess" button should be disabled
  - [ ] The message should say "0 guesses remaining"

- [ ] When you click the "reset" button, the form should return to its initial state (not disabled)

### Stretch Goals:

These items are not necessarily bugs in the code, but rather, missing features that should exist to prevent unexpected behavior.

(Optional) Complete the following:

- [ ] You should not be able to submit a guessed number lower than 1

- [ ] You should not be able to submit a guessed number higher than 99

- [ ] If there is only one guess left, it should say "guess" (singular) instead of "guesses" (plural)
</details>

### Backup to the cloud
Once you've found as many bugs as you can (and changed the code to fix them) follow the below instructions to push a copy from your local machine like you did at the end of last assignment. Make sure your code gets copied to GitHub by adding changes to staging, committing the staged changes, and pushing them from your local machine to GitHub:

 - [ ] Check the status of the changes you made by running `git status` in your terminal
 - [ ] Stage all your changes for commit by running `git add .` in your terminal
 - [ ] Run `git status` again to see how things have changed. You should get a response indicating changes staged for commit.
 - [ ] Create a commit message for reference. You can use a different message if you wish. Run `git commit -m "# bugs found and fixed"`
 - [ ] Push these changes to your GitHub repository from your local computer by running `git push`

### Submit Assignment
Now let's make sure that lesson branch will be reviewed.

 - [ ] Go to your GitHub repository page in your web browser now, and you should see a "debugging has a recent push" notice with a green "Compare & pull request" button. Click that button
 - [ ] Feel free to put notes to yourself or notes for your reviewer in the description (be sure you're including any questions to your reviewer in your assignment submission form though!) and click the green "Create pull request" button.
 - [ ] Copy the address of your pull request page (should look like `https://github.com/yourUsername/intro-to-programming-debugging/pull/1`) and paste it into your assignment submission form. Remember to also submit your pull request to your work in progress for your Open API Project in the "questions" field of your form if you'd like your work looked at.

### What next?
If you found all 8 bugs and completed all the optional stretch goals, congratulations!
If you did not find all bugs (or did but haven't attempted any stretch goals) continue work on this next week to try and find all 8 bugs at minimum.
