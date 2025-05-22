This week you'll have two parts to your coding assignment.  The first completes your work with your portfolio site by using API fetch to pull a list of all your GitHub repositories to your portfolio page.  The second part is an open API project to reinforce what you learn this week with fetch, and to give you another project for your portfolio.  

## Portfolio completion

<details>
<summary> Click here to expand your Portfolio completion assignment instructions </summary>
<br>
<h3>Get organized and write some code!</h3>
<ul>
<li>In your GitHub repository, if you have not yet merged your pull request from last week, merge your open lesson-12 pull request by going to the "Pull Requests" tab of your repository. Click on your open pull request, then click on the green 'Merge Pull Request" and confirm the merge. This will update your main branch with the work you did on your lesson-12 branch.</li>
<li>Open your code editor and, in the terminal, make sure you're on your main branch. If you're still on your lesson-12 branch, you can switch to your main branch by using the git command `git checkout main`.</li>
<li>Update your local main branch to include your lesson-12 work by pulling your changes from your GitHub repository main. Use the following git command in your terminal to do this: `git pull origin main`</li>
<li>Still in your terminal, create a new local branch to keep track of just the work you'll do for this assignment by running `git checkout -b lesson-13` in the terminal. Doing this also copies the lesson-12 work you merged to main and pulled to your local machine so now all your branches should be identical on your local machine.</li>
</ul>

### Assignment: Task List / Deliverables

#### Creating your fetch
- [ ] Open your `index.js` file, starting below the code from the previous lesson
- [ ] Using the Fetch API, create a "GET" request to `https://api.github.com/users/{GITHUB_USERNAME}/repos` where `{GITHUB_USERNAME}` is your username for your GitHub account
  - hint: the `fetch` function
  - hint: "GET" is the default method for `fetch`
- [ ] Chain a `then` method to your `fetch` call and pass it a function that returns the response JSON data

#### Handle your JSON data
- [ ] Chain another `then` method and pass it a callback function to parse the response and store it in a variable named `repositories`
  - hint: JSON.parse(this.response)
- [ ] Console.log the value of repositories to better see the data returned from your API fetch
- [ ] Save and refresh your browser _(or just check your browser for changes if using live extension)_
  - You should see the list of your GitHub repositories displayed in your console.

#### Handling errors
 - [ ] Chain a `catch()` function to your `fetch` call to handle errors from the server so the user would know what happened if your Projects section was empty.

#### Display Repositories in List
 - [ ] Create a variable names `projectSection`; using "DOM Selection" to select the projects section by id
 - [ ] Create a variable named `projectList`; using "DOM Selection" query the projectSection (instead of the entire document) to select the <ul> element
 - [ ] Create a for loop to iterate over your repositories Array, starting at index 0
   - [ ] Inside the loop, create a variable named `project` to make a new list item (li) element
     - hint: createElement method
   - [ ] On the next line, set the inner text of your project variable to the current Array element's name property
     - hint: access the Array element using bracket notation
   - [ ] On the next line, append the project element to the projectList element
     - hint: appendChild method
 - [ ] Save and refresh your browser _(or just check your browser for changes if using live extension)_
   - You should see your list of repositories beneath the "Projects" heading on your portfolio site
      
#### Style your Repository List
 - [ ] Open your `index.css` file
 - [ ] Add styling to your projects list, be sure to account for any changes you want in media queries
 - [ ] STRETCH GOAL: Use flexbox (or grid) to style your list of repositories

**_By the end of this assignment, you should have a working API fetch to your GitHub account and be able to see a list of your repository names in the Projects section of your portfolio.  Were there to be a server error during the API fetch, your site would return an error message.  Your project list should be styled using flexbos or grid._**
</details>

## Open API Project begins

<details>
<summary> Click here to expand your Open API Project assignment instructions </summary>
<br>
An "open source" means that the source code of something is freely available and can be redistributed and modified.  We have identified several options of open source APIs that allow you to use their data without paying for access to that data.  Use one of the following open source APIs to create a site that accesses a minimum of 2 data points. (Example: if using Open-Meteo, the weather API, you could display (1) the temperature and (2) the weather condition).  Take a look at the options below and decide which one(s) interest you the most.
**NOTE:** You have from now until the end of class to have your Open API Project meeting the requirements.  Think about what you want to build and how you want your site to look and then break the work into parts to pace yourself.

### Open Source API options:
 
* [Open-Meteo](https://open-meteo.com/) – a weather API
* [Swapi.Tech](https://www.swapi.tech/) – an API about Star Wars films
* [Marvel](https://developer.marvel.com/) – an API about the Marvel fandom
* [ARTIC](https://api.artic.edu/docs/#introduction) – an art API from the Art Institute of Chicago
* [TheDogAPI](https://thedogapi.com/) or the [TheCatAPI](https://thecatapi.com/) – APIs about (you guessed it!) Dogs or Cats
* [Soccer](https://api-sports.io/documentation/football/v3) - for all the Soccer lovers out there
* DEPRECATED, certificate expired - [SampleAPIs](https://sampleapis.com/api-list/coffee) – an API for coffee lovers

This week, just focus on accomplishing the following:
 - [ ] Familiarize yourself with the documentation of whichever API you decide to use
 - [ ] Create a new repository in GitHub specifically for your open API project and connect it to your local machine (you can look back at lesson 7 coding assignment instructions to refresh your memory if needed)

⚠️ **_NOTE:_** Be sure you are NOT in your portfolio folder when you clone your repository! Doing this will create a sub-repository which is a complicated problem to resolve. ⚠️ 

 - [ ] Create your basics (index.html, index.js, index.css) but don't go too in depth with any of them yet; just be sure your pages link correctly to each other
 - [ ] Repeat the portfolio part of the assignment above for this project to be sure that your fetch is working and that you're getting a response.  You don't need to display any of it yet, but you should at least be able to console.log the response so you can see what data you get back.  
 - [ ] Put a link to your Open API project repository in the readme.md file of your Portfolio project so your reviewer can easily find/look at your Open API project from your portfolio project.  You can add a link to your read me by using the following syntax:
`[My Open API Project](https://github.com/yourUsernameHere/yourname-open-api)` Put the words you want the link to be in hard brackets `[ ]` and the link to the repository in parentheses `( )` 

**_By the end of this assignment, you should have started on your Open API Project (create a repository, built your basics, and wrote the code for your API fetch to test what response you get back.  You should also see your Open API Project listed on your portfolio by the end of this part of the assignment._**
</details>

### Backup to the cloud
Once you've made the above changes to your index.js file, follow the below instructions to push a copy from your local machine like you did at the end of last assignment. You'll do this same process with your open API project to get any local work on that project backed up to your GitHub repository.  Make sure your code gets copied to GitHub by adding changes to staging, committing the staged changes, and pushing them from your local machine to GitHub:

- [ ] Check the status of the changes you just made (code changes to the index.js files) by running git status in your terminal
- [ ] Stage all your changes for commit by running `git add .` in your terminal
- [ ] Run `git status` again to see how things have changed. You should get a response indicating changes staged for commit.
- [ ] Create a commit message for reference. You can use a different message if you wish. Run `git commit -m "API fetch completed"`
- [ ] Push these changes to your GitHub repository from your local computer by running `git push`

### Submit Assignment
Now let's make sure that lesson branch will be reviewed.

- [ ] Go to your GitHub repository page in your web browser now, and you should see a "lesson-13 has a recent push" notice with a green "Compare & pull request" button. Click that button
- [ ] Feel free to put notes to yourself or notes for your reviewer in the description (be sure you're including any questions to your reviewer in your assignment submission form though!) and click the green "Create pull request" button.
- [ ] Copy the address of your pull request page (should look like https://github.com/yourUsername/name-classname/pull/8) and paste it into your assignment submission form.  **_NOTE: If you'd like your reviewer to check your open API project work in progress, submit the link in the "questions" field of your assignment submission form._**

### What next?
- If you're on track with class, wait to get feedback and/or the email notice that your assignment review is complete before confirming and merging your pull request to the main branch.
- If you're behind or are working ahead:
  - if you're confident your work is accurate, merge your pull request and continue working through class.
  - if you're not sure about your work this week, schedule a 1:1 session with a mentor and review your work together before merging.
