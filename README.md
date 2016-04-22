# Unit Testing with Javascript

In this project I was given a web-based application that reads RSS feeds. The original developer of this application saw the value in testing, they've already included Jasmine and  wrote their first test suite. Unfortunately, they decided to move on to start their own company and we're now left with an application with an incomplete test suite.


Within this project I learned how to use Jasmine to write a number of tests against a pre-existing application. Testing the underlying business logic of the application as well as the event handling and DOM manipulation.


# Steps to complete this project

1. Review the functionality of the application within the browser.
2. Explore the application's HTML (*./index.html*), CSS (*./css/style.css*) and JavaScript (*./js/app.js*) to gain an understanding of how it works.
3. Explore the Jasmine spec file in *./jasmine/spec/feedreader.js*
4. Edit the allFeeds variable in *./js/app.js* to make the provided test fail and see how Jasmine visualizes this failure in the application.
5. Return the allFeeds variable to a passing state.
6. Write a test that loops through each feed in the allFeeds object and ensures it has a URL defined and that the URL is not empty.
7. Write a test that loops through each feed in the allFeeds object and ensures it has a name defined and that the name is not empty.
8. Write a new test suite named "The menu".
9. Write a test that ensures the menu element is hidden by default. Aanalyze the HTML and the CSS to determine how the hiding/showing of the menu element is performed.
10. Write a test that ensures the menu changes visibility when the menu icon is clicked. This test should has two expectations: does the menu display when clicked and does it hide when clicked again.
11. Write a test that ensures when the loadFeed function is called and completes its work, make sure there is at least a single .entry element within the .feed container. loadFeed() is asynchronous so this test requires the use of Jasmine's beforeEach and asynchronous done() function.
12. Write a test that ensures when a new feed is loaded by the loadFeed function that the content actually changes.
