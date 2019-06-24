'''graphql
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
'''
