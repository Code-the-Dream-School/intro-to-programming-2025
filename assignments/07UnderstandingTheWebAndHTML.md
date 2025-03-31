### Get organized and write some code!
   - [ ] In your GitHub repository, if you have not yet merged your pull request from two weeks ago, merge your open lesson-5 pull request by going to the "Pull Requests" tab of your repository.  Click on your open pull request, then click on the green 'Merge Pull Request" and confirm the merge.  This will update your main branch with the work you did on your lesson-5 branch.
   - [ ] Open your code editor and, in the terminal, make sure you're on your main branch.  If you're still on your lesson-5 branch, you can switch to your main branch by using the git command `git checkout main`.  
   - [ ] Update your local main branch to include your lesson-5 work by pulling your changes from your GitHub repository main.  Use the following git command in your terminal to do this: `git pull origin main`.  Doing this copies the lesson-5 work you merged to main and pulls it to your local machine so now all your branches should be identical on your local machine.
   - [ ] Still in your terminal, create a new local branch to keep track of just the work you'll do for this assignment by running `git checkout -b lesson-7` in the terminal.  

### Assignment: Task List / Deliverables
Open your index.html file.  Add "boilerplate" HTML code as a starting point that includes all the required elements and meta tags.  While copy and pasting is common practice, this week we want you to write all the boilerplate code from scratch so you understand the parts of it and what their functions are.  Each line of the boilerplate HTML code is broken down below.  REMINDER: HTML uses code called "tags" and "elements". In HTML, an element consists of a "start tag", some content, and an "end tag".  So when describing the <title> element, for example, we're referring to this: `<title>Your Title</title>` Also, keep in mind some HTML elements are "self-closing", meaning that they have one tag that opens and closes at the same time (e.g. `<meta name="description" content="Your description" />`. In the Body and Additional Elements sections of these instructions you'll find the bulk of the actual site content (what the user will see when they view your page) listed.

#### HTML Boilerplate

##### Doctype
First let's define what type of document the browser will be reading.
   - [ ] Define the document type at the top of the file by typing in `<!DOCTYPE html>` on line 1.

##### Head Element
The "head" of an HTML document contains all the page's meta information, such as title and description.  This information helps with web searches and displays the page title in the browser tab.
   - [ ] Before your name, but after the `<html>` opening tag, insert a `<head>` element.
   - [ ] Inside the <head> element, add a <title> element to title your webpage (ex. Maria Santiago's Portfolio)
   - [ ] Below your <title> element, add additional <meta> elements (at least two) from the meta elements you've learned about and/or find at this resource: [W3Schools HTML Head](https://www.w3schools.com/html/html_head.asp))

##### Body Element
The "body" of an HTML document contains all the page's visible content.
   - [ ] After the closing </head> tag, begin the body of your page by adding the opening `<body>` element. 
   - [ ] Close the body of your page by adding the closing `</body>` element right before the closing `</html>` tag
   - [ ] Make sure all of the following content is inside the `<body>` tags, in this order:
     - [ ] Your name in an `h1` element
     - [ ] The word 'About' in an `h2` element
     - [ ] A paragraph about you in a `p` element
     - [ ] The word 'Experience' in an `h2` element
     - [ ] Your listed experiences in a `ul` element, with each individual item in a `li` element.  Experiences can be courses you've taken, coding/tech languages you've learned, technologies you've worked with, or other experiences that highlight your value.
     - [ ] The word 'Connect' in an `h2` element
     - [ ] Your social media links in `a` elements, and you can also wrap them in `ul` and `li` tags if you wish.  Include at least two, your GitHub and LinkedIn profiles.  You can include more (Facebook, YouTube, Instagram, WhatsApp, TikTok, Discord, X, etc.) if you like.

#### Additional Elements
HTML describes the structure of a webpage using various semantic elements, such as: headings, paragraphs, lists, and more, as you just saw by writing content for the body of your page.  Now let's organize that content...
   - [ ] Wrap each of the About, Experience, and Connect sections in a `<section>` element.  You'll use this later when you style your webpage to stay organized and apply different style settings to each of the different settings.
   - [ ] Give each of these sections an "id" property with the same name as the section.  Example:  The About section would look like this:

``` jsx
<section id="About">
   <h2>About</h2>
      <p>This is a paragraph about me.  Here's more info about me.</p>
</section>
```
   - [ ] STRETCH GOAL (optional):  Feel free to use even more HTML elements by adding images, navigation menus, etc.

**_By the end of these instructions, your index.html page should have boilerplate code that allows your web browser to identify what kind of document it's displaying and the meta data about your page (ex. title, keywords, etc.). You should have your Name, and three sections: (1) an About header with a paragraph about yourself, (2) an Experience header with a list of your experiences, and (3) a Connect header with at least two links.  All of this should be written in HTML in your index.html file._**

### Backup to the cloud
Once you've made the above changes to your html file, follow the below instructions to push a copy from your local machine like you did at the end of last assignment.  Make sure your code gets copied to GitHub by adding changes to staging, committing the staged changes, and pushing them from your local machine to GitHub:
   - [ ] Check the status of the changes you just made (editing the index.html file) by running `git status` in your terminal
   - [ ] Stage all your changes for commit by running `git add .` in your terminal
   - [ ] Run `git status` again to see how things have changed.  You should get a response indicating changes staged for commit.
   - [ ] Create a commit message for reference.  You can use a different message if you wish.  Run `git commit -m "boilerplate and content added"`
   - [ ] Push these changes to your GitHub repository from your local computer by running `git push`

### Submit Assignment
Now let's make sure that lesson branch will be reviewed.
   - [ ] Go to your GitHub repository page in your web browser now, and you should see a "lesson-7 has a recent push" notice with a green "Compare & pull request" button.  Click that button
   - [ ] Feel free to put notes to yourself or notes for your reviewer in the description (be sure you're including any questions to your reviewer in your assignment submission form though!) and click the green "Create pull request" button.
   - [ ] Copy the address of your pull request page (should look like `https://github.com/yourUsername/name-classname/pull/2`) and paste it into your assignment submission form.

### What next?
   - If you're on track with class, wait to get feedback and/or the email notice that your assignment review is complete before confirming and merging your pull request to the main branch.
   - If you're behind or are working ahead:  
     - if you're confident your work is accurate, merge your pull request and continue working through class.
     - if you're not sure about your work this week, schedule a 1:1 session with a mentor and review your work together before merging.
