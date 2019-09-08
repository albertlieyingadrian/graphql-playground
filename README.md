# graphql-playground

## Deployment
```
sls deploy
```

## How to test graphql server with postman
1. Using postman
* Put correct connect type in the header
`Content-Type: application/graphql`
* Put type raw your query for request body
Example
Query example
```
query {
  getMessage(id: "3f4e6510ee46276da533") {
    content
  }
}

```

Mutation example
```
mutation {
  createMessage(input: {
    author: "andy",
    content: "hope is a good thing 2",
  }) {
    id,
    content
  }
}
```

2. Using terminal
```
curl -X POST \
-H "Content-Type: application/json" \
-d '{"query": "{ hello }"}' \
http://localhost:4000/graphql
```

TODO:
1. Add subscription example
2. Clean up all code structures
3. Add tests