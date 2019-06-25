
```graphql
query {
  getAllBooks {
    _id
    title
    description
    language
    author {
      _id
      firstName
      lastName
      age
    }
  }
}

```

```graphql
query {
  getAllAuthors {
    _id
    firstName
    lastName
    age
    books {
      _id
      title
      description
      language
    }
  }
}
```

```graphql
query {
  getAuthor(_id: "5c5c423d4aef5c372833dc0c") {
    _id
    firstName
    lastName
    age
    books {
      _id
      title
      description
      language
    }
  }
}
```


```graphql
mutation {
  createAuthor(firstName: "Stephen", lastName: "King", age: 71) {
    _id
    firstName
    lastName
    age
  }
}
```

```graphql
mutation {
  deleteAuthor(_id: "5c5f0cdeeb1772069c8d12e9") {
    _id
    firstName
    lastName
    age
  }
}
```

```graphql
subscription {
  books {
    _id
    title
    description
    language
    author {
      _id
      firstName
      lastName
      age
    }
  }
}
```

```graphql
subscription {
  bookAdded {
    _id
    title
    description
    language
    author {
      _id
      firstName
      lastName
      age
    }
  }
}
```
