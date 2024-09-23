### Get organized to write some code!
   - [ ] In your GitHub repository, if you have not yet merged your pull request from last week, merge your open lesson-8 pull request by going to the "Pull Requests" tab of your repository. Click on your open pull request, then click on the green 'Merge Pull Request" and confirm the merge. This will update your main branch with the work you did on your lesson-8 branch.
   - [ ] Open your code editor and, in the terminal, make sure you're on your main branch. If you're still on your lesson-8 branch, you can switch to your main branch by using the git command `git checkout main`.
   - [ ] Update your local main branch to include your lesson-9 work by pulling your changes from your GitHub repository main. Use the following git command in your terminal to do this: `git pull origin main`
   - [ ] Still in your terminal, create a new local branch to keep track of just the work you'll do for this assignment by running `git checkout -b lesson-9` in the terminal. Doing this also copies the lesson-8 work you merged to main and pulled to your local machine so now all your branches should be identical on your local machine.
  
### Assignment: Task List / Deliverables
Last week you worked with styling.  This week lets work a little more with formatting and layout (the placement of your elements and their content).
   - [ ] In your index.html file, add a navigational header to your webpage using the `<nav>` element.
   - [ ] Add two sections to your index.html file:
     - [ ] The first section will be "Skills".  Use an h2 tag as you did with your About, Experience, and Connect sections, and be sure to include the id property in the element.  You can leave the section empty for now.  In later weeks we'll use JavaScript to insert a list of your skills.
     - [ ] The second section will be "Projects".  Use an h2 tag as you did with your About, Experience, and Connect sections, and be sure to include the id property in the element.  You need to add an empty `<ul>` element in this section; you will be adding your GitHub Projects via API call to this empty section using JavaScript later in this course.  
   - [ ] The navigation menu should include a link to each of your sections (i.e. "About", "Experience", "Skills", "Projects", "Connect")
     - [ ] STRETCH GOAL (Optional) Make the header sticky/fixed on the page using code in your index.css file.
   - [ ] In your index.css file, change the layout of your "Experience" section using rows and columns so items are displayed in a better layout rather than a list
         Hint: use Flexbox - we suggest have job titles to the left, dates worked that job to the right and brief description of the job below the title.
   - [ ] Also in your index.css file, update the "Connect" section to use Flexbox to improve the layout of your social media icons or links
**NOTE:** This is the basic rubric, but we encourage you to think beyond this list and come up with your own ideas to make your webpage unique!

**_By the end of this lesson, you should have added navigation to your site that uses internal links to "jump" the user to that section of your page.  You should also have reformatted your Experience and Connect sections using Flexbox css code.  Lastly, your site should have a header for your Skills and Projects sections, and an empty `<ul>` element in the Projects section, but no content in either section yet._**

### Backup to the cloud
Once you've made the above changes to your css file, follow the below instructions to push a copy from your local machine like you did at the end of last assignment. Make sure your code gets copied to GitHub by adding changes to staging, committing the staged changes, and pushing them from your local machine to GitHub:
   - [ ] Check the status of the changes you just made (editing the index.css file) by running `git status` in your terminal
   - [ ] Stage all your changes for commit by running `git add .` in your terminal
   - [ ] Run `git status` again to see how things have changed. You should get a response indicating changes staged for commit.
   - [ ] Create a commit message for reference. You can use a different message if you wish. Run `git commit -m "formatted styles added"`
   - [ ] Push these changes to your GitHub repository from your local computer by running `git push`

### Submit Assignment
Now let's make sure that lesson branch will be reviewed.
   - [ ] Go to your GitHub repository page in your web browser now, and you should see a "lesson-9 has a recent push" notice with a green "Compare & pull request" button. Click that button
   - [ ] Feel free to put notes to yourself or notes for your reviewer in the description (be sure you're including any questions to your reviewer in your assignment submission form though!) and click the green "Create pull request" button.
   - [ ] Copy the address of your pull request page (should look like `https://github.com/yourUsername/name-classname/pull/4`) and paste it into your assignment submission form.

### What next?
   - If you're on track with class, wait to get feedback and/or the email notice that your assignment review is complete before confirming and merging your pull request to the main branch.
   - If you're behind or are working ahead:
     - if you're confident your work is accurate, merge your pull request and continue working through class.
     - if you're not sure about your work this week, schedule a 1:1 session with a mentor and review your work together before merging.
