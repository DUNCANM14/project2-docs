# API Endpoints (Laravel 12 + Sanctum Authentication)

Your API uses Laravel Sanctum for token-based authentication.  
Users authenticate with `/api/users/login` to receive a Bearer token, which must be included in all protected requests.

Authorization header format:

```
Authorization: Bearer YOUR_TOKEN_HERE
```

---

# Authentication

## POST /api/users/login  
Authenticates a user and returns a Sanctum API token.

### Request Body
```json
{
  "username": "demo",
  "password": "password123"
}
```

### Response
```json
{
  "token": "5|xxxxxxxxxxxxxxxxxxxx"
}
```

---

## GET /api/users/me  
Protected route. Returns the currently authenticated user.

### Example
```
curl -X GET http://localhost:8000/api/users/me \
  -H "Authorization: Bearer YOUR_TOKEN"
```

---

## PUT /api/users/me/password  
Protected route. Updates the authenticated user's password.

### Request Body
```json
{
  "password": "newsecurepassword"
}
```

---

# User Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/users | List all users |
| GET | /api/users/{id} | Get a specific user |
| POST | /api/users | Create a new user |
| PUT | /api/users/{id} | Update an existing user |
| DELETE | /api/users/{id} | Delete a user |

---

# Friend Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/users/{id}/friends | Get all friends for a user |
| POST | /api/users/{id}/friends | Add a friend relationship |

### Example POST Body
```json
{
  "friend_id": 3
}
```

---

# Example Protected Curl Request

```
curl -X GET http://localhost:8000/api/users/2 \
  -H "Authorization: Bearer YOUR_TOKEN"
```
