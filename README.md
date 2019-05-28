# graphql-playground

## TO DO
- add prisma and apollo

## How to test graphql server with postman
1. Using postman
* Put correct connect type in the header
`Content-Type: application/graphql`
* Put type raw your query for request body
Example
```
{
    hello
}
```

2. Using terminal
```
curl -X POST \
-H "Content-Type: application/json" \
-d '{"query": "{ hello }"}' \
http://localhost:4000/graphql
```