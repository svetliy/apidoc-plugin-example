# apidoc-plugin-example

Generates and inject [apidoc](http://apidoc.com) example elements from api schemas or files.

`@apiExample {SCHEMA_TYPE=PATH_TO_SCHEMA} ELEMENT_TYPE TITLE`

## Install
`npm install apidoc-plugin-example --save-dev`

## Supported Schema Types
### json
Prettifies JSON and injects in.

### [jsonschema](http://www.jsonschema.org)
Uses [json-schema-faker]() to generate a sample response.


## Example Use
```javascript
/**
 * @api {get} /api GetAPI
 * @apiExample {json=./ex/api.req.json} apiParamExample Request
 * @apiExample {jsonschema=./ex/api.res.json} apiSuccessExample Response
 */
```

## TODO
- Add in xml/wsdl schema