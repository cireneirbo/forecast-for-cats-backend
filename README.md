# forecast-for-cats-backend
The ExpressJS backend for the React/Express sites of forecast-for-cats!\
It is hosted on [Heroku](https://dashboard.heroku.com/apps).\
It feeds data to [forecast-for-cats-frontend](https://github.com/cireneirbo/forecast-for-cats-frontend).

## Getting Started
* Clone or fork this repo.
* Install dependencies with `npm install`.
### Start the web app
* Navigate to the project's top directory in a terminal.
* Start the web app in the terminal using `npm start`
* Navigate to `http://localhost:9000/` in your browser.

## Getting your Open Weather Maps API key
* Go to [Open Weather Maps API](https://openweathermap.org/price) and sign up for a free account/key.
* Copy the `.env-sample` and rename it `.env`. 
* Copy and paste your Open Weather Maps API key into the placeholder value.

## Dependencies
* [Axios](https://www.npmjs.com/package/axios) - Promise based HTTP client for the browser and node.js.
* [Cookie-parser](https://www.npmjs.com/package/cookie-parser) - Parse Cookie header and populate req.cookies with an object keyed by the cookie names.
* [Cors](https://www.npmjs.com/package/cors) - CORS is a node.js package for providing a Connect/Express middleware that can be used to enable CORS with various options.
* [Debug](https://www.npmjs.com/package/debug) - A tiny JavaScript debugging utility modelled after Node.js core's debugging technique. Works in Node.js and web browsers.
* [Dotenv](https://www.npmjs.com/package/dotenv) - Dotenv is a zero-dependency module that loads environment variables from a .env file into process.env. Storing configuration in the environment separate from code is based on The Twelve-Factor App methodology.
* [Express](https://www.npmjs.com/package/express) - Fast, unopinionated, minimalist web framework for node.
* [Http-errors](https://www.npmjs.com/package/http-errors) - Create HTTP errors for Express, Koa, Connect, etc. with ease.
* [Jade](https://www.npmjs.com/package/jade) - Jade is a high performance template engine heavily influenced by Haml and implemented with JavaScript for node and browsers.
* [Morgan](https://www.npmjs.com/package/morgan) - HTTP request logger middleware for node.js.
* [Helmet](https://www.npmjs.com/package/helmet) - Helmet helps you secure your Express apps by setting various HTTP headers. It's not a silver bullet, but it can help!

## Hosting On Heroku
Follow [Heroku's NodeJS instructions](https://devcenter.heroku.com/articles/getting-started-with-nodejs)
* Sign up for a free account with Heroku.
* Install HerokuCLI (and be sure to have Git installed too).
* Log in to heroku using `heroku login` in your terminal.
* Create a dyno (instance) of your app on Heroku with `heroku create`.
  * You can specify a name as a parameter too: e.g. `heroku create forecast-for-cats-backend`.
* Set up a [Procfile](https://devcenter.heroku.com/articles/procfile) in the top-level directory of the project.
* Push local changes to heroku with:
  * `git add .`
  * `git commit -m "Push to heroku"`
  * `git push heroku main`
  * This step can be done routinely to update your project once it is running.
* Set up config/environment variables `heroku config:set OPEN_WEATHER_MAPS_API_KEY=your-openweathermaps-api-key`.
