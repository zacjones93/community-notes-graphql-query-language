<h1 align="center"><a href="https://egghead.io/courses/graphql-query-language">GraphQL Query Language</a></h1>

<p align="center"><img src="https://d2eip9sf3oo6c2.cloudfront.net/series/square_covers/000/000/236/full/EGH_GraphQLQuery_Final.png" width="200"></p>

These notes are being taken as part of an @eggheadio study group working through [GraphQL Query Language](https://egghead.io/courses/graphql-query-language).

Some question(s) are outlined in the essential questions section of the README for you to think about as you take the workshop. There is no 'definitive' answer to these questions but as you learn, you'll develop a more contextualized answer.

Right below is the intended outcomes of the course, these are the skills and knowledge you will learn that you can take to any application to use.

## Essential Questions

[TODO]

## Outcomes
- write queries to obtain all the data needed for an app in one response
- use mutations to add and change data
- GraphQL subscriptions and realtime

## GraphQL Query Language Description

GraphQL is gaining traction as one of the most popular ways to create an API. Regardless of which GraphQL implementation you pick, you’ll use the QL in GraphQL — the query language — to **query data, change data with mutations, and listen for data changes with subscriptions.**

You need to **know the Query Language regardless of the server-side implementation.** In this course, we will learn the GraphQL query language by sending an assortment of GraphQL operations to an existing API.

To start, we’ll learn how to** write queries to obtain all the data needed for an app** in one response. As the course progresses, we’ll use **mutations to add and change** data. To wrap up, we’ll investigate **GraphQL subscriptions and realtime data.**

After the course, you’ll be ready to communicate with a GraphQL API regardless of server-side implementation using the GraphQL query language.

This uses the [GraphQL Playground](https://pet-library.moonhighway.com/)

## **Query, mutation, & subscription**

only one endpoint

write query with the query keyword

    query {
      totalPets
    }

everything wrapped in the curlys is a `selection set`

`allPets` is a field

**Graphql is also a type system for you API** - there's a schema definition language that will define the types on your api

enumatiation type - restricted list of options

**Types can be objects - or a complex type.** When you're type is an object, you need to add another selection set and define a field within that set that you want.

Sometimes you don't want all the data from a query. **GraphQL lets you query based on arguments,** also know as filtering. These **arguments need to be defined by the GraphQL server you are querying from**.

Arguments correlate to some field on the data you are querrying. Some subset of them.

rename queries with graphQL alias's

if you want to use a **query twice in a selection set, you'll run into a naming collision** for the selection set. You need Alias's

You can prepend the query with `{alias}: query-name`

## **GraphiQL playground**

in browser ide that lets you send queries

**command clicking** a field name will take you to the graphql definintion in the field

**ctrl space** will surface all the fields available in a query.

## **Schema**

## **Fragments**

## **Variables**

## **Input types, unions, interfaces, & return payloads**

## **Introspective Queries**

## Contribute

These are community notes that I hope everyone who studies benefits from. If you notice areas that could be improved please feel free to open a PR!
