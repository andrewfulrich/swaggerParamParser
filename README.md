# swaggerParamParser
This provides 4 methods

# Methods

## getSwaggerParams

gets the parameters from a swagger doc

#### parameters
| name | description |
| --- | --- |
| req | the Express.js request object |
| swagger | the swagger js object |

#### returns
the object within the swagger object the describes the parameters for that path

## matchPathWithPathParam

matches a given request url with its corresponding swagger path

#### parameters
| name | description |
| --- | --- |
| reqPath | a real request url |
| swaggerPaths | a list of all the swagger paths in a swagger doc |

#### returns
the path string

## swaggerParamsToSchema

converts parrams in a swagger endpoint to a json schema

#### parameters
| name | description |
| --- | --- |
| parameters | the params as they appear in the swagger object |

#### returns
the json schema of the params

## parseBodyParams

parse the params from the swagger doc that are marked as being in the body of the request

#### parameters
| name | description |
| --- | --- |
| parameters | the params as they appear in the swagger object |

#### returns
the json schema of the params

## findPrimaryKey

find the primary key from parameters of a given endpoint in a swagger doc

#### parameters
| name | description |
| --- | --- |
| parameters | the params as they appear in the swagger object |

#### returns
the primary key parameter as it appears in the swagger object