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
      <li>Under Fetching and over fetching</li>
      When using REST APIs, one of the issues that can arise is under-fetching. This happens when a client needs to retrieve some data from the API, but the API doesn't provide all the data that the client needs in a single request. As a result, the client has to make multiple requests to the API to get all the data it needs, which can be inefficient and slow down the application.

On the other hand, over-fetching can occur when the API provides more data than the client actually needs. This can happen when the API returns all the available data for a particular resource, even if the client only needs a subset of that data. This can also lead to inefficient use of network resources and slow down the application.

GraphQL solves these problems by allowing the client to specify exactly what data it needs in a single request, and no more. The client can define a GraphQL query that specifies exactly what data it needs, and the GraphQL server will only return that data. This means that there is no under-fetching or over-fetching of data, and the client gets exactly what it needs in a single request, making the application more efficient and responsive.

    </ol> 
  </li>
</ol>
