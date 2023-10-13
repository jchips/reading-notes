# Reading Notes 2

Todays reading notes are on NodeJS, Express, NPM, TDD and CI/CD. They matter because they involve the stages we will for developing, testing and deploying are code. They are all very common in the Software Development field.

## An introduction to NodeJS and Express

1. Explain middleware, answer as though I were a non-technical recruiter.
    From what I understand, middleware can do some request or response processing and then either pass a request to the next middleware or send a response.
2. Express the most popular ____.
    Node web framework.
3. Express is “unopinionated.” What does that mean?
    It means that there are less limits with Express for choosing how you want to write and implement your code.
4. What is a module and why is modularity useful to us as developers?
  A module is a JavaScript library or file that you can import into your code. To do this, you use Node's require().

Source: <https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction>

## What is NPM?

1. What version of npm are you running on your machine?
    On my computer I am running npm 9.8.1
2. What command would you type to install a library/package called ‘jshint’ into your node project?
    `npm install jshint`

## What is TDD?

1. Explain why tests are important. Please explain as though I were your non technical elder.
    TDD is "test-driven development." Tests are important because they make sure our code is running how we want it to in multiple different cases.
2. What are three expected benefits of testing
    1. Less defect rates in the development.
    2. They make for less work in the final stages of a project development.
    3. Improves design and technical qualities of the code.
3. Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests.
    Individual:
        1. Forgetting to run the tests frequently.
        2. Making tests for parts of the code that aren't very important.
    Team:
        1. Only some team members are using TDD.
        2. TDD gets abandoned.

Source: <https://www.agilealliance.org/glossary/tdd/>

## CI/CD

1. What are three benefits of Continuous Integration?
    1. By adding changes frequently and having automated building and testing, you can quickly detect defects in the code.
    2. By quickly being able to detect bugs and errors, you can fix them quicker and deploy the code faster (so, faster release).
    3. The code will be consistently reliable because it's being tested frequently. So, it will have better quality than without CI.
2. What is the difference between Continuous Delivery and Continuous Deployment?
    Continuous Delivery is staging/testing and making sure the code is ready for deployment, then deploying manually. Continuous Deployment is doing the final production deployment to release the project automatically after the testing.
3. Explain how GitHub fits into this process assuming the listener comes from a non-technical background
    GitHub allows multiple people to work on one project together. When they make changes, GitHub has GitHub Actions that automatically builds, tests your code (if you wrote any tests), and deploys it for release. So, basically, GitHub Actions does CI/CD.

Sources: ChatGPT and <https://www.youtube.com/watch?v=k2aNsQKwyOo>

## Reflection

My learning goal is to get better at writing tests.

## Things I want to know more about
