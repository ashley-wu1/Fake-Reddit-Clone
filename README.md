[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/MVUO33FO)
# Term Project

See the three UML design docs in *images/*

## Instructions to setup and run project

1) Ensure you have installed MongoDB and the MongoDB Shell (mongosh). If you have not already done so, follow this link: `https://docs.mongodb.com/manual/administration/install-community/`.

2) Download or clone the repository.

3) Open the Command Prompt or Powershell on your laptop.

4) Go into the directory where the repository is located. (i.e. use `cd file/path`)

5) When the current directory is the entire project folder, run the command: `npm install`.

6) Then move into the server folder of the repository. (i.e. use `cd file/path/server`).

7) In the server folder, run the following command to install the necessary packages: `npm install`

8) Now go to the client folder of the repository (i.e. use `cd file/path/client`).

9) In the client folder, run the command: `npm install`.

10) Once all the package installations are complete, go back to the repository directory. (i.e. use `cd file/path`)

11) Run the command `mongod`. Wait until the code in the Command Prompt/Powershell stops.

12) Open another Command Prompt/Powershell tab. Go to the repository directory. (i.e. use `cd file/path`)

13) Run the command `mongosh`. (If the error `MongoNetworkError: connect ECONNREFUSED 127.0.0.1:27017` appears, check that mongod is finished running in the previous Command Prompt/Powershell tab)

14) Open another Command Prompt/Powershell tab. Then move into the server folder of the repository. (i.e. use `cd file/path/server`).

15) Decide what name, email, and password to use for the admin user account. 

16) Then run the command: `node init.js mongodb://127.0.0.1:27017/phreddit <admin-name> <admin-email> <admin password>`
- Fill in the fields `<admin-name>, <admin-email>, and <admin password>` with the name, email, and password from step 14, respectively.

17) Next, in the same Command Prompt/Powershell tab, run the command: `node server.js mongodb://127.0.0.1:27017/phreddit`

18) Open another Command Prompt/Powershell tab. Then move into the client folder of the repository. (i.e. use `cd file/path/client`).

19) Run the command: `npm start`

20) Open a Google Chrome tab and go to `http://localhost:3000/` to see the Phreddit website. The admin user account will have been automatically initialized, along with other users, posts, comments, and communities.

21) To see the server side data, go to `http://localhost:8000/`
- The users page is `http://localhost:8000/users`
- The communities page is `http://localhost:8000/communities`
- The comments page is `http://localhost:8000/comments`
- The posts page is `http://localhost:8000/posts`
- The linkflairs page is `http://localhost:8000/linkflairs`


## To Run Jest Tests

1) Open a Command Prompt/Powershell tab.
2) Go to the client folder of the repository (i.e. use `cd file/path/client`).
3) Run the command `npm test`. This will return the one `react.test.js` on the client side.
4) Go to all of the Command Prompt/Powershell tabs you have open for running the server or the MongoDB database and run Ctrl + C to close the server and database. Ensure they are closed before proceeding. 
4) Open another Command Prompt/Powershell tab.
5) Go to the client folder of the repository (i.e. use `cd file/path/server`).
6) Run `npm install mongodb-memory-server`.
7) Run the command `npm test`. This will return the two Jest tests on the server side.
Note: If you get an error stating server in use, return to step 4 and make sure you have the server and database closed. If they are running, it will prevent the test from executing properly.


In the sections below, list and describe each contribution briefly.

## Team Member 1 (Ashley Wu) Contribution
- Created Welcome page with register/login/guest options
- Added session cookie for maintaining login
- Implemented user profile page with deletion options
- Added upvotes for posts and use reputation changes
- Ordered navbar from joined and then not joined communities
- Defined schemas for models
- Worked on post sorting (new, old, and active)
- Fixed hover and click color changes for buttons
- Worked on search function and sorting of search posts
- Updated nav bar component to change when communities are added
- Eliminated eslint warnings for best practices
- Worked on listing of posts in different views
- Updated post view to automatically render new comments added
- Created components for the forms on the new comment, new community, and new post page views
- Created components for tracking the clicking and hovering of buttons to change background colors
- Created function for switching the content on the main page
- Created function for updating the list of communities on the nav bar
- Created a component for the search bar and returning relevant posts
- Made components for the horizontal banner and nav bar
- Created a component for updating the sorting of posts based on clicking the sorting buttons
- Wrote a function for displaying timestamps relative to the current time
- Wrote a function for dynamically updating the list of communities on the nav bar
- Wrote functions added through event listeners to the sorting buttons on the home page and community page views
- Wrote a function for displaying each post as specified and added a scrollbar
- Wrote a function for updating the community page view elements
- Wrote a class for saving each post in a data structure with multiple sublevels
- Wrote functions for the words of searches in posts and their comments and displayed the search results
- Wrote functions using the added class to create threading under posts in the post page view
- Created forms for making new communities and new posts
- Added CSS styling to the Create Post button to change color when hovering
- Made the website logo and name clickable for returning to the home page view
- Updated linkflair dropdown to allow for choosing no linkflair

## Team Member 2 (Sandy Wu) Contribution
- Added join/leave community functionality
- Implemented sorting separated by communities joined and communities not joined on main page
- Implemented post sorting by membership in community for search results page
- Fixed upvote and downvote for posts, and the login return session
- Applied CSS styling to the Welcome page
- Created new post submission component
- Defined server routes and modularized routes
- Worked on new comment submission component
- Worked on new community submission
- Defined server routes for handling axios requests
- Integrated link flair functionality and check for duality
- Enhanced the design of the banner, navigation bar, create post section, and main view (including scroll bar adjustments).
- Added a button to create link flair that updates the dropdown list immediately after selection.
- Implemented functionality to allow users to choose between using a dropdown or typing their own for link flair
- Changed input to text areas in the create post, create community, and add comment sections to enable users to write more extensive content
- Corrected the active sorting feature so that it functions based on search results instead of just all posts

