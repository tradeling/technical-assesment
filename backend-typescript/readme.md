## Typescript Backend Challenge

[Indego](https://www.rideindego.com) is Philadelphia's bike-sharing program, with many bike stations in the city.

The [Indego GeoJSON station status API](https://www.rideindego.com/stations/json/) provides a realtime snapshot of the number of bikes available, number of open docks available (not currently containing a bike), and total number of docks at every station. This API is free and requires no API key.

The [Open Weather Map API](https://openweathermap.org/current#name) provides a realtime snapshot of the current weather in a given city. Since Philadelphia is a small geographical area it is sufficient to obtain the weather for a geographical location central to Philadelphia. This API has a free plan, you will need to sign up for an API key.

Using Typescript, Node.js, [Typescript](http://www.typescriptlang.org/), [Mongoose](https://mongoosejs.com/) and [Express](http://expressjs.com/) create a new API server which accumulates data over time and provides access to historical data for both weather and Indego bike availability.

## API endpoints

Use a static token and protect all the endpoints. If that static token is not provided or is invalid return error response with relevant HTTP status code.

### Store data from Indego

An endpoints which downloads fresh data from [Indego GeoJSON station status API](https://www.rideindego.com/stations/json/) and stores it inside MongoDB.

```bash
# this endpoint will be trigger every hour to fetch the data and insert it in the mongo database 
POST http://localhost:3000/api/v1/indego-data-fetch-and-store-it-db
```

### Snapshot of all stations at a specified time

Data for all stations as of 11am Universal Coordinated Time on September 1st, 2019:

```bash
GET http://localhost:3000/api/v1/stations?at=2019-09-01T10:00:00
```

This endpoint should respond as follows, with the actual time of the first snapshot of data on or after the requested time and the data:

```javascript
{
  at: '2019-09-01:T10:00:01',
  stations: { /* As per the Indego API */ },
  weather: { /* As per the Open Weather Map API response for Philadelphia */ }
}
```

If no suitable data is available a 404 status code should be given.

### Snapshot of one station at a specific time

Data for a specific station (by its `kioskId`) at a specific time:

```bash
GET http://localhost:3000/api/v1/stations/KIOSKID_GOES_HERE?at=2019-09-01T10:00:00
```

The response should be the first available on or after the given time, and should look like:

```javascript
{
  at: '2019-09-01T10:00:00',
  station: { /* Data just for this one station as per the Indego API */ },
  weather: { /* As per the Open Weather Map API response for Philadelphia */ }
}
```

Include an `at` property in the same format indicating the actual time of the snapshot.

If no suitable data is available a 404 status code should be given.

## Unit tests

Write functional and API test using using [Jest](https://jestjs.io/).

## Hosting details

You will need to make your API available on a server that we can communicate with. You can make use of the following services:
* [Heroku](https://heroku.com/)
* [MongoDB Cloud](https://www.mongodb.com/cloud)
 
## Criteria

Your work will be evaluated primarily on:

* Use following [coding style guide](https://github.com/airbnb/javascript)
* Correct use of promises, including proper error handling. async/await may be used
* Typescript definitions, types, interfaces.
* Efficient MongoDB queries and indexes
* Mongoose schemas and models
* Unit tests for API endpoints and also do functional testing
* [JSDoc](https://jsdoc.app/) for documenting JavaScript code
* API documentation using [Swagger](https://swagger.io/)

## How to submit your work

Create a private project on Github and push your code on it. And give the access to following users:

* [Mohamed Meabed](https://github.com/meabed)

## Extra credit

* A simple front end React application offering a visualization of all or part of the data utilizing the API you have built as a back end.
* Anything else you think is cool, relevant, and consistent with the other requirements.
