## API Calls & Sample Responses
- GET localhost:3000/generate
```JSON
{
  "randomString": "d89F281KQ0"
  "requests": []
}

{
  "error": "Could not generate new URL. Try again later."
}
```

- GET localhost:3000/display/[randomURLstring]
```JSON
{
  "randomString": "d89F281KQ0"
  "requests": ["requestObject1", "requestObject2"]
}
```

- POST localhost:3000/newRequest
```JSON
{
  "message": "Forwarded to front-end"
}

{
   "message": "Client not connected with WebSocket or not found, payload not forwarded"
}
```
- POST localhost:3002/[randomURLstring]

_End point for 3rd-party webhook requests_
