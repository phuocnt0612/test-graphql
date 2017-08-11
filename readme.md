# Guide


##Environment


###Laradock


```
Organize test-graphql/laradock folder as below structure:
+ laradock
+ test-graphql
```

## GraphQL

**Access GraphQL UI:**

```
test-graphql.me/graphiql
```

**Create new user with graphQL**
```
mutation {
    createUser (
        name: "phuoc"
        email: "test@gmail.com",
        password: "123123123"
    ){
        id,
        email
    }
}
```

**Select User**

```
query {
    users(id: "1") {
        id,
        email
    }
}
```