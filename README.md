# Unit 13 PWA Challenge: Online/Offline Rolodex App
Today, your Project Owners ask you to create a Client Rolodex app for the company. However, the backend team has not built the backend API yet, so there is no data for you to query. To add another wrench into the development cycle, your Project Owners say that they want to demo the app for the executive team using an API and want it to be a PWA.

Sounds like you have your work cut out for ya!

## User Story
AS AN employee of the company
I WANT to be able to see all clients that are in the company rolodex
AND be able to create new client records via a form
I WOULD also like to be able to view a detailed version of a client contact information via a modal on the homepage

* View a Demo [here](https://company-dex.netlify.app/)

## Requirements
* General:
  * [ ] The app should render three Pages:
    1. [ ] A Homepage
    2. [ ] A Create Record Page
    3. [ ] A Update Record Page
  * [ ] The app must ingest data from the [jsonplaceholder](https://jsonplaceholder.typicode.com/)
  * [ ] Each page must have a Navbar that has links to:
    * [ ] `Homepage`
    * [ ] `Create Record Page`
* Homepage:
  * [ ] As soon as the page has loaded (`onload`), the page should check `localStorage` to see if user data exist and render it
    * [ ] If no data exist, then the app must perform an API call to the [jsonplaceholder](https://jsonplaceholder.typicode.com/) `users` endpoint and then store the returned data to `localStorage`
      * [ ] The data must be rendered from `localStorage`
  * [ ] Each user data item should be rendered in a card with the following data:
    * [ ] Client's Name
    * [ ] Client's Company Name
    * [ ] Client's Catch Phrase
  * [ ] Each card should render three buttons:
    1. [ ] Contact Info - Onclick this button should render a modal that displays the following data:
       * [ ] Client's Name
       * [ ] Client's Company Name
       * [ ] Client's Company Address
       * [ ] Client's Catch Phrase
       * [ ] Client's Email
       * [ ] Client's Phone Number
       * [ ] Client's Username
       * [ ] Client's Website
       * [ ] The data rendered within the **models** must come from local storage
    2. [ ] Delete Contact - Onclick this button should remove the card from localStorage, the homepage, and cause a page to reload
    3. [ ] Update Contact - OnClick this should navigate the user to the `Update Contact Page`
* [ ] Create Record Page:
  * [ ] This page **must** display a form
  * [ ] On submit, the form must perform a POST request to the [jsonplaceholder](https://jsonplaceholder.typicode.com/) API
    * [ ] Be sure to read the documentation on how data persist via the API
    * [ ] The created record **must** be stored in `localStorage`
    * [ ] On successful submission, the form **must** route the user back to the Homepage and the new record along with all pre-existing records should all be rendered
* [ ] Update Record Page:
  * [ ] This page **must** display a form
    * [ ] The form **must** be populated with the selected `Clients` data.
      * [ ] This data should be pulled from `localStorage`
  * [ ] On submit the form must perform a PUT request to the [jsonplaceholder](https://jsonplaceholder.typicode.com/) API
    * [ ] Be sure to read the documentation on how data persist via the API
    * [ ] The updated record **must** be stored in `localStorage`
    * [ ] On successful submission, the form **must** route the user back to the Homepage and the updated record along with all pre-existing records should all be rendered
- - -

## Commit Early and Often

* One of the most important skills to master as a web developer is version control. Building the habit of committing via Git is important for two reasons:

1. Your commit history is a signal to employers that you are actively working on projects and learning new skills

2. Your commit history allows you to revert your code base in the event that you need to return to a previous state

* Follow these guidelines for committing:

  * Make single purpose commits for related changes to ensure a clean, manageable history. If you are fixing two issues, make two commits

  * Write descriptive, meaningful commit messages so that you and anyone else looking at your repository can easily understand its history

  * Don't commit half-done work, for the sake of your collaborators (and your future self!)

  * Test your application before you commit to ensure functionality at every step in the development process

* We would like you to have well over 200 commits by graduation, so commit early and often!

## Submission on BCS

* You are required to submit the following:

  * the URL to the deployed application

  * the URL to the Github repository
---

## Requirements

This challenge is assessed on the following criteria: 

### Technical Acceptance Criteria: 40%

* Satisfies all of the above acceptance criteria 

### Deployment: 32%

* Application deployed at live URL (if applicable).

* Application loads with no errors.

* Application GitHub URL submitted (if applicable).

* GitHub repository that contains application code.

### Application Quality: 15%

* Application resembles (at least 90%) screenshots provided in the challenge instructions.

### Repository Quality: 13%

* Repository has a unique name.

* Repository follows best practices for file structure and naming conventions.

* Repository follows best practices for class/id naming conventions, indentation, quality comments, etc.

* Repository contains multiple descriptive commit messages.

* Repository contains quality README file with description, screenshot, and link to deployed application.

© 2021 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
