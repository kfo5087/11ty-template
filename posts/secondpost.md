## What is an API?
An API (Application Programming Interface) is a software that allows for connections between computers and computer programs. For this project we took advantage of Wikipedia's API's.

## Fetch

`fetch` is a method in JavaScript that is used to request resources in the form of HTTP from a webpage. Shown below is an example of `fetch` being used to communicate with Wikipedia. A request is sent out with a resulting JSON response.
![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/t72e2a77b8gu6t7r528m.png)

## Wikipedia API
Before starting with Wikipedia api, make sure to import the necessary packages by adding this line of code to the top
`import '@lrnwebcomponents/wikipedia-query/wikipedia-query.js';`

Wikipedia has a numerous amount of functions that can be referenced [here](https://en.wikipedia.org/w/api.php). This API allows users to connect to Wikipedia and manage different functions. With this lab we are dealing with the query function and it is accessed by using the tag `wikipedia-query`, it uses `fetch` to search for the necessary parameters. 

```
<wikipedia-query search="${this.city}, ${this.state}"></wikipedia-query>
      <wikipedia-query search="${this.city}"></wikipedia-query>
      <wikipedia-query search="${this.state}"></wikipedia-query>
```
The above block of code is three query's that get parameters filling out the state and city, the city alone, and the state alone. They were gained earlier in conjunction with the freegeoip app.

In all, API's are a useful tool that allow for coders to do less coding. Provided is my GitHub [repository](https://github.com/kfo5087/ip-project/tree/master/src)
