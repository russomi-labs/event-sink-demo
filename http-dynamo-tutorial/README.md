# http-dynamo-tutorial
- [Overview](#overview)
- [Usage](#usage)
  - [To create or update an item](#to-create-or-update-an-item)
  - [To get all items](#to-get-all-items)
  - [To get an item](#to-get-an-item)
  - [To delete an item](#to-delete-an-item)
- [See Also](#see-also)
- [Contributing](#contributing)

## Overview

> In this [tutorial](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-dynamo-db.html), you create a serverless API that creates, reads, updates, and
> deletes items from a DynamoDB table. DynamoDB is a fully managed NoSQL database
> service that provides fast and predictable performance with seamless
> scalability.

## Usage

### To create or update an item

```bash
curl -v -X "PUT" -H "Content-Type: application/json" -d "{\"id\": \"abcdef234\", \"price\": 12345, \"name\": \"myitem\"}" https://hqzxsonx59.execute-api.us-east-1.amazonaws.com/items
```

### To get all items

```bash
curl -v https://hqzxsonx59.execute-api.us-east-1.amazonaws.com/items
```

### To get an item

```bash
curl -v https://hqzxsonx59.execute-api.us-east-1.amazonaws.com/items/abcdef234
```

### To delete an item

```bash
curl -v -X "DELETE" https://hqzxsonx59.execute-api.us-east-1.amazonaws.com/items/abcdef234
```

## See Also

- [Tutorial: Build a CRUD API with Lambda and DynamoDB](https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-dynamo-db.html)

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for details.
