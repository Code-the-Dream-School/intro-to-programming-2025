### Get organized and write some code!
 - [ ] In your GitHub repository, if you have not yet merged your pull request from last week, merge your open lesson-9 pull request by going to the "Pull Requests" tab of your repository. 
 - [ ] Click on your open pull request, then click on the green 'Merge Pull Request" and confirm the merge. This will update your main branch with the work you did on your lesson-9 branch.
 - [ ] Open your code editor and, in the terminal, make sure you're on your main branch. If you're still on your lesson-9 branch, you can switch to your main branch by using the git command `git checkout main`.
 - [ ] Update your local main branch to include your lesson-9 work by pulling your changes from your GitHub repository main. Use the following git command in your terminal to do this: `git pull origin main`
 - [ ] Still in your terminal, create a new local branch to keep track of just the work you'll do for this assignment by running `git checkout -b lesson-10` in the terminal. Doing this also copies the lesson-9 work you merged to main and pulled to your local machine so now all your branches should be identical on your local machine.

### Assignment: Task List / Deliverables
Your site is probably looking good on your browser, but as you learned the majority of users use a mobile device or tablet to view sites.  Let's make your site look good on every device!
**TIP:** When working with sizing, it's best to use percentages, REMs and EMs.. you can read more about those [here](https://www.linkedin.com/pulse/pixels-vs-em-rem-percent-when-why-use-each-milan-savov).  
 - [ ] Open your index.css file
 - [ ] Determine if you'd like to build your site mobile-first or desktop-first (meaning the code you have in there right now will be the default code for a phone or a desktop/laptop monitor)
 - [ ] Add comment notation to help keep yourself organized and make it easier to find your desktop/tablet/mobile style code sections
 - [ ] Based on if you decided to design mobile-first or desktop first, add your media queries for the other two device types.  Example: if you're designing mobile-first, you'll want to add a media query that handles devices that are tablet sized, and a media query that handles anything larger than the largest tablet size.
 - [ ] Make a minimum of two changes to at least three elements for each of your media queries.  Example: In your tablet media query, change the font size (1st change) and color (2nd change) of your headers (1st element), change the padding or margin (1st change) and background color (2nd change) of your unordered lists (2nd element), and change the font size (1st change) and font style (2nd change) of your name at the top of your page (3rd element)

 - [ ] STRETCH GOAL: Since we learned about grid layout this week, reformat one or both of your two flexbox sections (Experience or Connect) to be a grid layout instead to give yourself practice using grid.

The above are just suggestions/examples.  As in the past two lessons, we encourage you to make your site an expression of yourself!  Just keep in mind accessibility, because your awesomeness needs to be visible to everyone!  

**_By the end of this lesson you should have at least two media queries defined in your index.css file and those media queries should be changing a minimum of two style properties across at least three of your html elements._**

### Backup to the cloud
Once you've made the above changes to your css file, follow the below instructions to push a copy from your local machine like you did at the end of last assignment. Make sure your code gets copied to GitHub by adding changes to staging, committing the staged changes, and pushing them from your local machine to GitHub:
 - [ ] Check the status of the changes you just made (editing the index.css file) by running `git status` in your terminal
 - [ ] Stage all your changes for commit by running `git add .` in your terminal
 - [ ] Run `git status` again to see how things have changed. You should get a response indicating changes staged for commit.
 - [ ] Create a commit message for reference. You can use a different message if you wish. Run `git commit -m “responsiveness added"`
 - [ ] Push these changes to your GitHub repository from your local computer by running `git push`

### Submit Assignment
Now let's make sure that lesson branch will be reviewed.  
 - [ ] Go to your GitHub repository page in your web browser now, and you should see a "lesson-10 has a recent push" notice with a green "Compare & pull request" button. Click that button
 - [ ] Feel free to put notes to yourself or notes for your reviewer in the description (be sure you're including any questions to your reviewer in your assignment submission form though!) and click the green "Create pull request" button.
 - [ ] Copy the address of your pull request page (should look like `https://github.com/yourUsername/name-classname/pull/5`) and paste it into your assignment submission form.

### What next?
- If you're on track with class, wait to get feedback and/or the email notice that your assignment review is complete before confirming and merging your pull request to the main branch.
- If you're behind or are working ahead:
  - if you're confident your work is accurate, merge your pull request and continue working through class.
  - if you're not sure about your work this week, schedule a 1:1 session with a mentor and review your work together before merging.
