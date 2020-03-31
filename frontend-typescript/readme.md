## frontend-task
> Build a GitHub repository search application

This case study aims to assess how you approach a problem starting from the high level solution to the low level implementation details and code quality. You will not be penalized for asking questions, so don't hesitate to ask us if you need any clarification.

## The Task

You are required to build a simple React.js application with **TypeScript** that has a search box where a user will be able to search for GitHub repositories by name and see the list of the results. The results will be fetched from the GitHub API.

You can find the GitHub API search docs below:

* [GitHub Search API Docs](https://developer.github.com/v3/search/#search-repositories)
* [Sample Search Request](https://api.github.com/search/repositories?q=tetris+language:assembly&sort=stars&order=desc)

## Requirements

Build a single page React.js application with the following functionality

* Display a search bar where a user can type a search keyword
* Display the results as a grid of 3 columns. For each repository display the repository user details returned from API and the repository name, author, stars and other statistics below it. A sample
 ![](https://i.ibb.co/S5fbcc7/image.png)

* On mobile screens (width <= 768px), the grid will be 2 columns
  ![](https://i.ibb.co/Bfc8qYS/image.png)

* You should start to fetch and display the results from the backend once the user types 3 characters or more in the search bar
* If the user is typing, don't make any API calls until they stop typing for 300ms
* Consider all the possible UI states: initial, loading, error,... and present them to the user clearly. No fancy UI required
* There are no design requirements, but we expect you to use minimal CSS to structure the page and make it a little pleasant. Don’t use external CSS or UI frameworks like bootstrap, bulma, ant.

## Criteria

Your work will be evaluated primarily on:

* `README.md` file explaining your high level solution and any decisions you made and the reasons behind them
* Tests are not needed but will be a big plus
* We will assess the quality of your code. Use modern ES6+ syntax, async/await, elegant & readable code
* Typescript definitions, types, interfaces.
