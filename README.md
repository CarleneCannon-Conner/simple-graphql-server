# simple-graphql-server
Following FreeCodeCamp Tutorial: A Beginner’s Guide to GraphQL using `graphpack`

## To run locally:
`npm run dev`

Playground will be served at: [http://localhost:4000/](http://localhost:4000/)

### Example Playground Queries
#### List all Users
```
query {
  users {
    id
    name
    email
    age
  }
}
```

#### Show a user by id
```
query {
  user(id: "1") {
    id
    name
    email
    age
  }
}
```

### Example Playground Mutations
#### Create a new user
```
mutation {
  createUser(id: "3", name: "Robert", email: "robert@gmail.com", age: 21) {
    id
    name
    email
    age
  }
}
```

#### Update an existing user
```
mutation {
  updateUser(id: "3", name: "Bobby", email: "bobby@gmail.com") {
    id
    name
    email
    age
  }
}
```

#### Delete an existing user
```
mutation {
  deleteUser(id: "3") {
    id
    name
    email
    age
  }
}
```
