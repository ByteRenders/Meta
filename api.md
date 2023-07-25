This file describes the api spec for this project. For any models included in
this file such as `VideoDescriptor` please see `models.md`

## Format
All requests should append `/api`

Requests will be defined as `METHOD /path/to/endpoint` excluding the root `/api`

Requests may include variables in the path defined like `$variablename`
variable names should generally be self descriptive but may include some
description

All responses will be given as pseudo json representations as such
`field: type | format`
where format is an example or description of a value you may receive

## Meta
### GET /version
```json
{
    version: Utf8 String | "v1.0.0"
}
```

## Video
### GET /search/$query
A query will simply be search terms seperated by dashes instead of spaces

```json
{
    results: [ Video ]
}


