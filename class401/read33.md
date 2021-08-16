# Add relationships between types

## @connection

***The @connection directive enables you to specify relationships between @model types. Currently, this supports one-to-one, one-to-many, and many-to-one relationships. You may implement many-to-many relationships using two one-to-many connections and a joining @model type. See the usage section for details.***

## Definition
`directive @connection(keyName: String, fields: [String!]) on FIELD_DEFINITION`

## Usage

***Relationships between types are specified by annotating fields on an `@model` object type with the `@connection` directive.***

***The fields argument can be provided and indicates which fields can be queried by to get connected objects. The keyName argument can optionally be used to specify the name of secondary index (an index that was set up using `@key`) that should be queried from the other type in the relationship.***

***When specifying a `keyName`, the fields argument should be provided to indicate which field(s) will be used to get connected objects. If `keyName` is not provided, then `@connection` queries the target table’s primary index.***

### Has one

***In the simplest case, you can define a one-to-one connection where a project has one team:***<br>
`type Project @model {`
  `id: ID!`
 ` name: String`
 ` team: Team @connection`
`}`

`type Team @model {`
  `id: ID!`
 ` name: String!`
`}`


### Has many

***The following schema defines a Post that can have many comments:***
`type Post @model {id: ID! title: String! comments: [Comment] @connection(keyName: "byPost", fields: ["id"])}`

`type Comment @model`<br>
 `@key(name: "byPost", fields: ["postID", "content"]) { id: ID!postID: ID!content: String!}`