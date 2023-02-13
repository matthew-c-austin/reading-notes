# Reading

[Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

1. In your own words, describe what each group of status code represents:

    100’s = Informational status codes; they tell the client that the header has been received and the server will try to comply with the demand of the client.
    200’s = Success codes. Not necessarily that the request was successfuly processed, but that it met all the validation requirements at the time of sending
    300’s = Redirection codes. They tell the client the resource doesn't exist at the expected location anymore.
    400’s = Client error codes. These are invalid requests with reasons such as timeouts, incorrect URI, missing authentication,etc.
    500’s = Server error codes (overwhelmed server/unreachable behind proxies/client requests that trigger error exceptions located on the server)

2. What is a status code 202?

    Accepted

3. What is a status code 308?

    Permanent Redirect

4. What code would you use if an update didn’t return data to a client?

    204

5. What code would you use if a resource used to exist but no longer does?

    410

6. What is the ‘Forbidden’ status code?j

    403

[Build A REST API With Node.js, Express, & MongoDB - Quick](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

    To safely and dynamically connect to the database

2. What is middleware?

    Code that runs when the server gets a request, but before it's passed to routes.

3. What does app.use(express.json()) do?

    Let's the server accept JSON as the body instead of a POST or GET element, etc.

4. What does the /:id mean in a route?

    A parameter

5. What is the difference between PUT and PATCH?

    PUT updates all the information, and PATCH updates only the information that gets passed

6. How do you make a default value in a schema?

    with `default: defaultValue`

7. What does a 500 error status code mean?

    Internal Server Error

8. What is the difference between a status 200 and a status 201?

    200 is OK, as in everything is OK. 201 is 'Created', as in teh request has been fulfilled and one or more resources have been created.

## Things I want to know more about

1. The npm i --save-dev that doesn't get pushed to production is not something we did for our install of dotenv or nodemon. Why is that?
2. Is route.rest a more or less powerful Thunder Client type functionality?
