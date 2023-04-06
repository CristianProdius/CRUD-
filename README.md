# CRUD

<h1>Aim of Project</h1>
The project is a CRUD API built using GraphQL and the Python frameworks Starlette. It uses MongoDB as a database and is designed to be asynchronous. The data is validated using Pydantic and the code follows a clean architecture. The API allows users to create, read, update, and delete data for a collection of objects that include fields such as name, surname, and dates of last login and registration. The read operation includes pagination and filtering by name, surname, and value. The project is meant to be deployed using Docker Compose and the code is written in Python 3.11 using Poetry for package management. The project also includes integration tests to ensure the functionality of the API.

<h2> Stage of Project </h2>
<ol>
  <li>
    <h3>Learn Basic of GraphQl</h3>
    <ol>
      <li>what is GraphQL</li>
      GraphQl is an API but insded giving all the information from a server it provides you with only the info that you want. For instance when you ask a librian for a book he gaves you only that book instead of providing all books from library.
      <li>Advandages over REST</li>
      GraphQL give us only the information requiered while REST provides all the information
      <li>REST quieres/GraphQL quieres</li>
      Suppose we have an API that provides information about users and their posts. Here's how we might query the API using REST and GraphQL:

REST API:

To get all posts for a user with an ID of 123:

bash
Copy code
GET /users/123/posts
To get all comments for a post with an ID of 456:

bash
Copy code
GET /posts/456/comments
GraphQL API:

To get all posts for a user with an ID of 123:

scss
Copy code
query {
  user(id: 123) {
    posts {
      id
      title
      content
    }
  }
}
To get all comments for a post with an ID of 456:

scss
Copy code
query {
  post(id: 456) {
    comments {
      id
      author
      text
    }
  }
}
As you can see, with GraphQL, we can get all the information we need in a single request, and we can specify exactly what information we want to get back. With REST, we might need to make multiple requests to get all the information we need, and we might get more information than we actually need.
    </ol> 
  </li>
</ol>
