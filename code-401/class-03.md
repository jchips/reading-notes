# Reading Notes 3

## Review: ES6 Classes

1. Classes are a template for creating ____.

    Objects.

2. Can a class declaration be hoisted?

    Class declarations cannot be hoisted.

3. How would you describe a constructor and contextual “this” to a non-technical friend?

    A constructor is kind of like a blueprint or template for making something. You can make multiple 'objects' with a constructor, all with the same blueprint. The 'this' keyword refers to an object itself. So, when you say 'this,' you are referring to a specific object made from the constructor.

Sources: <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes> and ChatGPT.

## Using Express Routing

1. Within Express, what does routing refer to?

    "Routing refers to how an application’s endpoints (URIs) respond to client requests." Different routing methods perform different actions (GET vs POST).

2. What is the difference between a route path and a route method?

    "A route method is derived from one of the HTTP methods and is attached to an instance of the express class. Route paths define the endpoints at which requests can be made." An example of a route method is `app.get` and an example of a route path is '/about'. The route path and the route method are usually combined like so, in a route handler: `app.get('/about', ...)`.

3. When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?

    It's appropriate to add `next()` to the parameters if you are going to use `next()` to move your code to the next middleware function. It's also required to use `next()` in your parameters if the middleware function is to handle all errors globally.

Source of quotes: <https://expressjs.com/en/guide/routing.html>

## Express Routing

1. What is an Express Router?

    The Express Router is like a mini Express Router that you can create instances of and use to make route methods for a specific route. You can apply many Express Routers to one application for different routes.

2. By what mean do we initialize express.Router() in an express server?

    `var router = express.Router();`

3. What do we use route middleware for?

    From what I understand, route middleware gets performed on every route made from the instance of its specific Express Router. So, everything that you put in your route middleware (`router.use(...)`) will happen on every request the user makes before it reaches the route.

## Reflection

My learning goal is to be able to build a REST API using a Postgres database and Sequelize.

## Things I want to know more about
