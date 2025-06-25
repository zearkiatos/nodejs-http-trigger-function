# Description
This is an azure function ⚡️ built in nodejs 🟩 to execute an simple http trigger this is in order to practice and study for az204 certificate exam

# Made with
[![JavaScript](https://img.shields.io/badge/javascript-ead547?style=for-the-badge&logo=javascript&logoColor=white&labelColor=000000)]()
[![Node.js](https://img.shields.io/badge/node.js-76c339?style=for-the-badge&logo=node.js&logoColor=white&labelColor=000000)]()

# cURL example

## httpTriggerWithName

```sh
$ curl --location --request GET 'https://nodejs-http-trigger-function.azurewebsites.net/api/az204-http-trigger?code={CODE}' \
--header 'Content-Type: application/json' \
--data '{
    "name": "Pedro"
}'
```

### Response
```txt
$ Hello, Pedro. This HTTP triggered function executed successfully.
```

## httpTriggerWithoutName

```sh
$ curl --location 'https://nodejs-http-trigger-function.azurewebsites.net/api/az204-http-trigger?code={CODE}'
```

### Response
```txt
$ This HTTP triggered function executed successfully. Pass a name in the query string or in the request body for a personalized response.
```