# forecast-for-cats-backend
The ExpressJS backend for the React/Express sites of forecast-for-cats!\
It is hosted on [Heroku](https://dashboard.heroku.com/apps).\
It feeds data to [forecast-for-cats-frontend]().

## Dependencies
* [Axios](https://www.npmjs.com/package/axios)
* [Cookie-parser](https://www.npmjs.com/package/cookie-parser)
* [Cors](https://www.npmjs.com/package/cors)
* [Debug](https://www.npmjs.com/package/debug)
* [Dotenv](https://www.npmjs.com/package/dotenv)
* [Express](https://www.npmjs.com/package/express)
* [Http-errors](https://www.npmjs.com/package/http-errors)
* [Jade](https://www.npmjs.com/package/jade)
* [Morgan](https://www.npmjs.com/package/morgan)

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