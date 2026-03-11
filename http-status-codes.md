<p align="center">
<img src="https://cdn.simpleicons.org/http/0055FF" height="70" alt="HTTP"/>
</p>

# HTTP Status Codes Cheat Sheet

HTTP status codes are standardized responses returned by a web server to indicate the result of a client's request. These codes help developers understand whether a request was successful, redirected, or resulted in an error.

Each status code belongs to a specific category that represents the type of response returned by the server.

---

## 1xx Informational Responses

<img src="https://cdn.simpleicons.org/internetarchive" height="22"/> These codes indicate that the request has been received and the process is continuing.

| Code  | Name                | Description                                                                                       |
| ----- | ------------------- | ------------------------------------------------------------------------------------------------- |
| `100` | Continue            | The server has received the request headers and the client can continue sending the request body. |
| `101` | Switching Protocols | The server agrees to switch protocols as requested by the client.                                 |

---

## 2xx Success Responses

<img src="https://cdn.simpleicons.org/checkmarx/00AA55" height="22"/> These codes indicate that the request was successfully received, understood, and processed.

| Code  | Name       | Description                                                            |
| ----- | ---------- | ---------------------------------------------------------------------- |
| `200` | OK         | The request was successful and the server returned the requested data. |
| `201` | Created    | The request succeeded and a new resource was created.                  |
| `204` | No Content | The request was successful but there is no content to return.          |

Example:

```
HTTP/1.1 200 OK
```

---

## 3xx Redirection Responses

<img src="https://cdn.simpleicons.org/redirect" height="22"/> These codes indicate that further action must be taken by the client to complete the request.

| Code  | Name              | Description                                                                             |
| ----- | ----------------- | --------------------------------------------------------------------------------------- |
| `301` | Moved Permanently | The requested resource has permanently moved to a new URL.                              |
| `302` | Found             | The resource is temporarily located at a different URL.                                 |
| `304` | Not Modified      | The resource has not changed since the last request, so the cached version can be used. |

---

## 4xx Client Error Responses

<img src="https://cdn.simpleicons.org/bug" height="22"/> These codes indicate that the request contains incorrect syntax or cannot be fulfilled by the server.

| Code  | Name         | Description                                                        |
| ----- | ------------ | ------------------------------------------------------------------ |
| `400` | Bad Request  | The server could not understand the request due to invalid syntax. |
| `401` | Unauthorized | Authentication is required to access the requested resource.       |
| `403` | Forbidden    | The server understood the request but refuses to authorize it.     |
| `404` | Not Found    | The requested resource could not be found on the server.           |

Example:

```
HTTP/1.1 404 Not Found
```

---

## 5xx Server Error Responses

<img src="https://cdn.simpleicons.org/serverfault" height="22"/> These codes indicate that the server encountered an error while processing the request.

| Code  | Name                  | Description                                                                          |
| ----- | --------------------- | ------------------------------------------------------------------------------------ |
| `500` | Internal Server Error | A generic error occurred on the server.                                              |
| `502` | Bad Gateway           | The server received an invalid response from another server.                         |
| `503` | Service Unavailable   | The server is currently unable to handle the request due to maintenance or overload. |

---

## Summary

HTTP status codes help developers quickly understand the outcome of a request made to a web server. Knowing these codes is essential when building APIs, debugging web applications, or working with backend services.
