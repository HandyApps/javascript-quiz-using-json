

# Javascript quiz using JSON
:question: :question: :question: :question: :question: :question: :question: :question: :question:


[![Code Climate](https://codeclimate.com/github/Matt-Webb/jquery-quiz-using-json/badges/gpa.svg?style=flat-square)](https://codeclimate.com/github/Matt-Webb/jquery-quiz-using-json)
[![Build Status](https://travis-ci.org/Matt-Webb/jquery-quiz-using-json.svg?branch=master&style=flat-square)](https://travis-ci.org/Matt-Webb/jquery-quiz-using-json)
[![codecov](https://codecov.io/gh/Matt-Webb/jquery-quiz-using-json/branch/master/graph/badge.svg)](https://codecov.io/gh/Matt-Webb/jquery-quiz-using-json)

This code enables you to render questions with optional answers as multiple choice. The data is loaded using [valid JSON](http://jsonlint.com/)
you can provide a list of questions and answers which will render to the user in sequence or at random.

Each question can be assigned a score against each option, this allows for a range of scores for each question.

### ALPHA [v0.2.0](https://github.com/Matt-Webb/jquery-quiz-using-json/tree/v0.2.0-alpha)

This project is currently in ALPHA and activity being worked on. Contributions are welcome!

#### How to use:

**Sample JSON**

Here is a sample of the quiz question data:

      {
          "question": "What year was the film The Terminator released?",
          "info": "The Terminator is a 1984 American science fiction action film directed by James Cameron. It stars Arnold Schwarzenegger as the Terminator, a cyborg assassin sent back in time from 2029 to 1984 to kill Sarah Connor (Linda Hamilton), whose son will one day become a savior against machines in a post-apocalyptic future.",
          "options":
            [
              "1982",
              "1983",
              "1984",
              "1984"
            ],
          "scores":
            [0,3,1,2]
      }

**HTML**

    <!-- dom reference -->
    <div id="quizName"></div>

    <!-- script -->
    <script src="./jquery-quiz-using-json/dist/quiz.min.js"></script>

**JAVASCRIPT**

Initialise the quiz like so. Note this needs to be done after referencing the script shown above.

    Quiz.init({ id: "quizName" });  

**HOW TO INSTALL**

`$ npm i`

`$ npm test`


### TO DO

* [ ] Remove jQuery dependency
* [ ] Abstract the rendered html question into templates for better customisation
* [ ] Add optional style sheets
* [ ] Move TODOs to issues with need-help flag
* [ ] Set up semvar
* [ ] Update Travis Build
* [ ] Add module bundler
* [ ] Add test coverage badge
* [ ] Add Automated Acceptance Tests
* [ ] Add charts to result rendering
* [x] Refactor json data for better clarity e.g "answers" should be "options" etc.
* [x] Configurate as bower package
* [x] Remove Bower, Switch to npm
* [x] Add Unit Tests
