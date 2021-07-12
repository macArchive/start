# Full Stack Development

## Tools

### Languages

- Typescript
- GraphQL

### Frontend

- Next
- Chakra

### Backend

- Apollo
- Database or Storage Solution

### Utilities

- Prettier
- ESLint

## Development Cycle

### 1. Schema Definition

Identify which data the application will need, then structure the data as intuitively as possible.
We can do this by sketching out a data graph of nodes and edges and then building the schema.
Types should always be defined in PascalCase.
Add an `!` to ensure a field is non-nullable.
Use `""` To add comments to a GraphQL Schema.

### 2. Database/Storage Provision

Choose a data storage option suitable for the current project.
Create the basic tables, collections and some test entries for api testing.

### 3. Backend Implimentation

Build GraphQL API using Apollo Server and fetch data from data source.
Build using Mock Data first, then connect to live data source once Frontend is complete.

### 3. Frontend Implimentation

Client consumes data from GraphQL API to render it.
Assign query strings using ALL_CAPS and wrap in the gql template literal.
Export query definitions for use in testing.
Test queries in Apollo Studio first.
Use a query result component to conditionally render Loading, Error and Data states.

## Folder Structure

```
root
|   readme.md
|   .gitignore
|
└─── client
|     | components
|     | pages
|     | public
|     | styles
|     | next-env.d.ts
|     | package.json
|     | tsconfig.json
|     | yarn.lock
|
└─── server
|     | index.js
|     | package.json
```
