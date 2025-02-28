# Technical assignment
The goal of this assignment is to complete as many tasks as possible listed below in the TODO list. 

## Scenario
An integration specialist has built a landing page for a Live Video Shopping event, but there are still bugs to solve and improvements to make before the page can be used in production. We need you to update the code and fix the tasks listed in the TODO list further down on this page so everything is working as expected once launched. 

## Expectation
Here are the specifications and high-level requirements for this landing page.

On this landing page, we are going to promote a Live Video Shopping show. 

The landing page consists of:
- **A countdown:** A graphical countdown. We should be able to set the date and time of the event. The countdown should disappear when done.
- **A header:** This header should have the value of 'We go live in' before the countdown is done. After the target time is passed, the value of the header should be 'We are live!'.
- **A CTA element:** A card including an image and a button. The whole card should be clickable and trigger the Bambuser Player with a recorded test show.

## Test the current behavior
### 1. Run the project
You are able to run the current project in either way below:
 - In the terminal, run `npm i` and then run `npm start` within the project working directory. (Requires Node.js to be installed.)
 - Or, open the `src/index.html` in a browser.

### 2. Modify the target time
In order to test the countdown on different occasions, in the `src/index.html`, you need to update the `data-date` and `data-time` to a closer time (e.g. current time + 1 min). So you can see how the countdown behaves when it reaches the target time.
## TODO
  - [X]  Make the countdown loop stop once it reaches the target time. Currently, the countdown continues with minus values. 
  - [X]  Make the countdown element disappear after the target time is reached.
  - [X]  The CTA element should show up when the countdown is done.
  - [X]  The default font for the landing page is set to `Neue Haas Grotesk Display`, but the font is not applied. Investigate why and provide a solution.
  - [X]  Center the `wrapper` element by modifying the CSS. The `wrapper` element is not fully centered (It is horizontally centered but not vertically). 
  - [X]  The header text must be changed to 'We Are Live!' when the countdown is done.

## Bonus questions
Once you have fixed the CTA button, you should be able to click it. On click, the Bambuser One-to-many player will be opened. When clicking a product in the player, you will see an error page. You should not solve this error! But, you may explain the questions below. 
   - What is the error?
   - Why does it happen, what is the reason for this error?
   - What would be potential solution(s)?

### Answer
      Place a brief explanation here. You can explain this further during the technical interview.

      - What is the error? The error is a CSP error which blocks external sites from embeeding on their sites
- Why does it happen, what is the reason for this error? It happens so unauthorized websites cannot use the embedding for free.
- What would be the potential solution(s)? Potential solutions would be that assuming we have a whitelist of website we add on our end, we add this clients website to our whitelist.


See how to reproduce the error: [Video](producing-iframe-error.mp4)




## How to deliver the assignment
- You will receive the assignment in a `.zip` file that you can unzip and start working on it.
- Make sure you read the README.md carefully before you start working on the tasks.
- Not necessary but *would be a bonus* to use Git and commit your changes. You can initiate and use a local Git repository or a private remote repository.
- When you are done, make a zip archive of your project, including the .git directory *in case you choose to use Git*.
- There is no right or wrong, so, feel free to be creative while delivering the expectations.
- If you have any questions, reach out via email.