
# Hello API

Returns the message 'Hello, World!!!'.

## Endpoint

```
GET http://localhost:8080/hello
```

## Query Parameters

| Parameter | Type   | Default Value | Description                          |
|-----------|--------|---------------|--------------------------------------|
| name      | string | "World"       | The name to be used in the message.   |



### Example Request Without Parameter

```
GET http://localhost:8080/hello
```

## Response

```json
{
  "message": "Hello, World!!!"
}
```

### Example Request With Parameter

```
GET http://localhost:8080/hello?name=John
```

## Response

```json
{
  "message": "Hello, John!!!"
}
```

## Response Codes

- `200 OK` - The request was successful, and the message was returned successfully.
- `400 Bad Request` - The request is invalid due to parameter errors.
