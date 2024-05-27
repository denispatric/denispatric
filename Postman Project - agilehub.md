# AGILEHUB 05/2024 project: Trello REST API testing with Postman

## :information_desk_person: About project

<p align="justify">Agilehub is a Romanian non-governmental organization, apolitical and unaffiliated with any other entity. During the project, I had the chance to acquire fundamental knowledge of the REST API, become familiar with the Postman tool, create my collections using Trello documentation, learn GIT, and explore GitHub.

The result of the project is a collection of Trello REST API tests performed in the Postman tool.</p>

## :mag_right: Test scope based on [Trello API documentation](https://developer.atlassian.com/cloud/trello/rest/api-group-actions/)
➡️[Link to my TRELLO test cases/Test execution schedule file](https://docs.google.com/spreadsheets/d/1AHsX-jEzcNJ04PBUllaaP32m8lPaab9j/edit?usp=drive_link&ouid=101099971300589548082&rtpof=true&sd=true)

- **Board**
  - Create a Board
  - Get a Board
  - Update a Board
  - Delete a Board
- **List**
  - Create a List on a Board
  - Get Lists on the Board
  - Update a List
- **Card**
  - Create a new Card
  - Get a Card on a Board
  - Update a Card
  - Delete a Card
- **Checklist**
  - Create a Checklist on a Board
  - Get Checklists on a Board
  - Create Checkitem on the Checklist
  - Delete a Checklist
  
## :rocket: Getting started

#### :pushpin: List of steps needed to run collection and tests

1️⃣ [Postman installation](#one)

:two: [Creating a Trello account](#two)

:three: [Trello authentication](#three)

:four: [Importing a file into Postman](#four)

:five: [Run collection and start testing](#six)

------

#### <a name="one">:computer: Postman installation</a>

1. Go to the [Postman website](https://www.postman.com/downloads/) and click the orange button with the name of your operating system.
2. Download the installation file, then run the installer and follow the instructions that appear.
3. Postman is ready to use.
    
#### <a name="two">:date: Creating a Trello account</a>

1. Go to the [Trello website](https://trello.com/) and click the blue button with the text "Get Trello for free".
2. Create a Trello account by following the instructions that appear.
3. Your Trello account is ready to use.

#### <a name="three">:key: Trello authentication</a>

1. Log in to your Trello account.
2. Go to the [Trello developer API key generation page](https://trello.com/app-key).
3. Click on the "Go to the Power-Up Admin Portal", then click the "Create New Key" button and enter the required details.
4. Your API key will be displayed on the page. Copy and save it for later use in Postman.
5. Next, click on the Token link that appears under the key you just generated.
6. Allow the application to access your Trello account.
7. Your token will be displayed on the page. Copy and save it for later use in Postman.

#### <a name="four">:open_file_folder: Importing a file into Postman</a>

1. Go to [my Postman collection file](https://drive.google.com/drive/folders/1IaCE5_1Jbi8jKv5Ac9rz66SspUXm8YOf?usp=drive_link).
2. Find the .json file and click on the three dots icon in the top right corner and click "Download".
3. Run Postman and click on the "Import" button in the top left corner.
4. Drag and drop the downloaded file from the Download folder into the "Import" window.
5. Do the same with the environment files
6. The collection will appear in Postman, ready for use.   

#### <a name="six">:runner: Run collection and start testing</a>

1. Click on the "Collections" icon in Postman.
2. From the list of collections, select the one named "Trello REST API" and click on the icon with three dots that appears when you hover over the collection name.
3. Select "Run collection" from the list.
4. Click on the orange button "Run Trello - REST API".

--------
### :point_down: If the view in your Postman looks like the one on the screenshot below, then you have successfully completed all the steps and run my collection. CONGRATULATIONS! :clap:

![image](https://github.com/denispatric/denispatric/assets/83760732/14240dd6-30d0-45d9-9cd0-4e43088ca21d)
