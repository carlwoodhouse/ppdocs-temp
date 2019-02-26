# Introduction
Currently PPQ only supports graphql queries not mutations. The endpoint supports both HTTP GET and HTTP POST for queries. Both GET and POST requests require a valid authenentication header

The graphql api endpoint is located at ```https://dev.patientplatform.io/content/graphql```

### Query Sample

The following graphql query will be used as a sample for the following examples.

```
{
  article(first: 1) {
    name
  }
}
```

### GET

GET Requests require a ```query``` querystring paramater is passed

Given the sample query a GET request would be as follows
```
curl -H "Authorization: Bearer ${TOKEN}" https://dev.patientplatform.io/content/graphql?query=%7Barticle%28first%3A%201%29%20%7Bname%7D%7D%0A
```

Query variables can be sent as a JSON-encoded string in an additional query parameter called variables. If the query contains several named operations, an operationName query parameter can be used to control which one should be executed.

### POST

For POST requests you must include the query in a JSON-encoded body and include a content type header of ```application/json```

The body would as follows for the sample query from early
```
{
  "query":"{article(first: 1) {name}}\","variables":null},
  "variables": { "myVariable": "someValue", ... }
}

```
variables is optional and can be passed as null.


### Response
Regardless of the method by which the query and variables were sent, the response will be returned in the body of the request in JSON format. As mentioned in the spec, a query might result in some data and some errors, and those should be returned in a JSON object of the form:

```
{
  "data": { ... },
  "errors": [ ... ]
}
```
If there were no errors returned, the "errors" field should not be present on the response. 

Given our sample query the response with no errors would look like this

```
{
    "data":{
        "article":[
            {"name":"How to become someone who loves exercise"}
        ]
    }
}
```

## PlayGround

A sandbox enviorment for writing queries is available at [graphqlplayground](https://graphqlplayground.z33.web.core.windows.net/) - authenticate using your client credentials.