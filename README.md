# LET'S TEST YOU!

This is a **quiz on general knowledge** website that enable the users to test themselves on 8 different topics: History, Geography, Geopolitics, Economy, Nature, English and Psychology. The user can replay he game and have other questions displayed. It will be useful for the user to test his general knowledge or even learn.

![Responsive-Screens](assets/images/responsive-screens.jpg)


Project URL : [Let's Test You!](https://shiimymy.github.io/general-knowledge-quizz/)

## Features

### Landing Page 

The landing page is the index.html that the user will see which has different components.

![Landing-Page](assets/images/landing-page.jpg)

#### Description

The **Description** can be found on all html pages by hovering the mouse on the question mark icon. This will allow to make the user aware of the number subjects and that he can replay the game to have other questions.

![Description](assets/images/description.jpg)

#### Username Form

The **User Form** can be found on the first page that will ask the player to choose an username. This username will then be displayed on the second page of the website.

![Username-Form](assets/images/username-form.jpg)

### The quiz page

#### Score 

The score area show the number of questions *(which is 7)* that one round will display. It will also count the number of correct answers each time an answer is submitted. If the answer is correct, it will add one point to the score.

![score](assets/images/count-right-answers.jpg)

#### Question number 

The **Question number** is actually very useful as this what the game will check to know if whether or not the game needs to end. The game will indeed display 7 questions per round.

![Question-number](assets/images/display-question-number.jpg)

#### Question content

The question content will be chosen randomly by the system between the *14 possibilities*. It is divided in 3 elements that stay connected: the subject, the actual question and 3 different answer options.

![Question-content](assets/images/display-question.jpg)

#### Submit button

The **Submit** button as different roles: 
* Add a point to the score if the answer is correct,
* Display an answer feedback to let the user know if the right answer or not has been selected. If the wrong one has been selected, the message will inform the user what was the correct answer.

![Submit-button](assets/images/submit-selection.jpg)

![Right Answer](assets/images/display-answer-right.jpg)

![Wrong Answer](assets/images/display-answer-wrong.jpg)

#### Next Question button

This button will be display below the answer feedback once the **Submit** button has been clicked. When the **Next Question** button is clicked, it will either display a new question if the maximum of questions hasn't been reach yet. If it has been reach, it will end the quiz round.

![Next Question](assets/images/next-question.jpg)

#### End Message

The **End Message** will be display once the 7 questions have been answered whereas the question area will be hidden. The user will then easily understand that the round is over and a little feedback will show. This feedback will change depending of the score of the round. 

* If the score is below 4 points : 

![End-message-bad](assets/images/end-message-bad.jpg)

* If the score is below 7 points : 

![End-message-good](assets/images/end-message-good.jpg)

* If the score is of 7 points : 

![End-message-great](assets/images/end-message-great.jpg)

#### End buttons

With the **End message**, two buttons will be displayed. The user will have the choice to either restart the game from the quizz.html with the username saved or exit the game and redirect to the index.html.

![End-buttons](assets/images/end-buttons.jpg)

## Testing

### Manual Testing

| Test | Expected result | Passed |
| ---- | ---- | ---- |
| Cross Browser Testing | The Website is working on Google Chrome, Microsoft Edge, and Firefox. | YES |
| Page loading | The pages load correctly with content at the right position | YES |
| Username Form | The form can't be submitted without an username and redirect to quizz.html | YES |
| Question mark icon | When the icon is hover, the description appear and disappear when mouse leave | YES |
| Username display | The username enter in the first form is displayed in the h1 of quizz.html | YES |
| Answer submission | Only one answer can be selected and submit at a time | YES |
| Answer display | Once the answer is submitted, a message appear to let know if the answer is correct | YES |
| Point add | When the answer is correct, a point is added to the score | YES |
| Next Question button | This button appears with the answer and when clicked a new question is displayed | YES |
| Random Question | The new Question is a random question taken from the array with no repeat | YES |
| Round stop | A round is 7 questions only | YES |
| Thanks User | The thanks message is customized with username | YES |
| Feedback display | A different feedback is displayed depending on the score | YES |
| Restart Game | The button restart game start a new round | YES |
| Exit Game | The Exit Game button redirect the user to www.google.com | YES |


### Validator Testing

* HTML Testing: no error found with [W3C Validator](https://validator.w3.org/).
* CSS Testing: no error found with [Jigsaw Validator](https://jigsaw.w3.org/css-validator/validator).

### Performance Testing

I used [Lighthouse](https://developer.chrome.com/docs/lighthouse/overview/) to test the performances of my 2 pages. The results were positive, as scores were between 90 and 93. Please find the result below at the time of the tests:

* Index page performances:

![Index page Performances](assets/images/performance-index.jpg)

* Quiz page performances: 

![Quiz page Performances](assets/images/performance-quiz.jpg)

### Fixed issues 

| Issues | Description | Steps done to fix |
| --- | ---- | ---- |
| Responsiveness | Website not responsive on big screens | Changes done thanks to [Am I Responsive website](https://ui.dev/amiresponsive) as I didn't have access to a bigger screen. |
| Exit Game | Exit Game button giving 404 error | Delete function and add href in the link to redirect user |
| User experience | User didn't know the correct answer when choosing a wrong option | Add message when answer is submitted |
| Score colour | The content was transparent | Update colour in css to make the content visible |
| Input Attribute | In the text input of the first page was "min" attribute | It is now deleted |
| Answer submission | The user could submit without selecting an answer after the first question | Set the localStorage.correct to null when a new question is display and add alert to prevent form submission |

## Deployment

* **Fork template**: The first step before coding was to fork the [ci-full-template](https://github.com/Code-Institute-Org/ci-full-template) from [Code Institute](https://codeinstitute.net/ie/) as asked. 
To do so, once on the ci-full-template in Github (as per the first link), I clicked on **Fork** on the top-right of the page. Then I renamed the repository with the name of my project under **Repository name** and clicked to **Create Fork**. This allowed me to update the template.

* **Project deployment**: Once the site was nearly ready, it was deployed thanks to [Github](https://github.com/) from the [general-knowledge-quizz repository](https://github.com/Shiimymy/general-knowledge-quizz). Once in the repository, I clicked on **Settings** in the top navigation bar, then on Pages in the left menu. Once the page opened, in the Branch section, I chose main in the drop down menu and clicked on **Save**.

* **Clone project**:

This project will be also cloned to work locally on the future realesed by following these setps:

1. Go in [General Knowledge Quizz](https://github.com/Shiimymy/general-knowledge-quizz) repository,
2. Click on Code to find the URL and copy it.
3. In the Terminal write git clone and paste the url.
4. Press Enter to create the clone.

## Credit

### Content

* The question mark icon was taken from [Font Awesome](https://fontawesome.com/),
* The understanding of how a basic quiz using JS is build was found on [Geeks for Geeks](https://www.geeksforgeeks.org/),
* Instructions to know how to use the localStorage property were taken from [MDN](https://developer.mozilla.org/), 
* The instructions to add points to score were founds on [Love Maths Project](https://github.com/Code-Institute-Solutions/love-maths-2.0-sourcecode/tree/master).

### Media

The [Background image](https://www.pexels.com/fr-fr/photo/femme-en-rouge-a-manches-longues-ecrit-sur-tableau-noir-3769714/) has been taken from [Pexels](https://www.pexels.com/).

The images in the feedback have been take from [Pexels](https://www.pexels.com/) too : 
* [Bad score](https://www.pexels.com/fr-fr/photo/femme-melancolique-regarder-une-video-sur-un-ordinateur-portable-a-la-maison-3808012/),
* [Good Score](https://www.pexels.com/fr-fr/photo/personne-faisant-les-pouces-vers-le-haut-193821/),
* [Excellent Score](https://www.pexels.com/fr-fr/photo/photographie-de-personnes-diplomees-1205651/).