# Cornerstone FE tech test

## Overview

Create a Web app that utilises the Punk API and shows a list of punk beers.

We use React at Cornerstone and would prefer the test to be completed with this library, but if you don't know React, plain JS is fine. Please do not use any other library/framework apart from React.

This test should take at most 4 hours to be completed, including initial setup.

After you complete the test, please create a repo with the final version on either Github or a similar service.

## Requirements

- Use [create-react-app][rca] for the project base and [react-router-dom][rrd] for routing.

- App should be able to run on the latest version of [Node.js][node] with only the following commands:

  ```sh
  npm install
  npm start
  ```

- The app should be responsive.

- Home page should show a list of all the beers returned by the api.

- The home page should have a select input to allow sorting beers by name or abv.

- Pending ajax requests should have a loading state shown on the current page.

- Clicking on a `More details` link should navigate to a separate page showing more details about the selected beer. The url pathname should change to `/beer/:id`. Image and beer name should also link to the beer page.

- The beer page should have a link to go back to the home page.

- Deep-linking to a specific beer page should load that beer data from the api without going through the home page.

- Styles with CSS are required - Please refer to the provided wireframes to know more about how to style the UI.

- No specific fonts are needed, you can use system fonts.

- App should make use of the latest JavaScript features such as:
  - `import` + `export` in place of `require()` + `module.exports`
  - arrow functions where they reduce the complexity of the code or lexical scope
  - `rest` and `spread` properties
  - object destructuring
  - anything else you find nifty

## Punk API

You can read the api docs [here][punk_api].

**HTTP Requests**

- All beers `GET https://api.punkapi.com/v2/beers`
- Single beer `GET https://api.punkapi.com/v2/beers/1`

## Bonus Task

- Unit tests or integration tests (choose one and explain why)
- Use [React component state][react_docs] or [Redux][redux] to store/cache data fetched from the API to avoid hitting the server again for repeat requests
- Style the app using [styled components][styled_components]

[rca]: https://github.com/facebookincubator/create-react-app
[rrd]: https://github.com/ReactTraining/react-router/tree/master/packages/react-router-dom
[node]: https://nodejs.org/en/
[punk_api]: https://punkapi.com/documentation/v2
[react_docs]: https://reactjs.org/docs/getting-started.html
[redux]: https://github.com/reactjs/redux
[styled_components]: https://www.styled-components.com/
