# News Scraper

A web app that scrapes the news articles from the New York Times website (https://www.nytimes.com/), and allow users to view them in a more unifrom format.

The app contains two pages: one for viewing articles and their associated comments, and one for viewing all articles made through the app. The technology and languages used are Node.js, Express, Express-Handlebars, HTML, CSS, JS, and MongoDB with Mongoose.

#How it works

When the home page loads for the first time there will be no news articles, when the scrape button is clicked the app uses Cheerio to scrape the NYTimes website for story headlines, urls, and summaries. With each additional click the newest articles will add to the list.

Each scraped article is saved to a noSQL database and the database stops articles from duplicating. In the case of a duplicate in headline or url, the database looks for the existing article entry in the database and displays that on the page instead. A user can save an article for later viewing

Goals

The page needs improved functionality, as it's currently missing some components. I have saved article working, but would like it to remove it from the main page once it has been saved. I would also like to be able to add a comments field and a way for users to switch to some other pre-saved sites and scrape from them as well.

## The live app can be found at this link
https://mongo-scraper-101.herokuapp.com/