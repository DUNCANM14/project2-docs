# Testing the API

The following examples demonstrate how to test the Laravel API using curl with Sanctum Bearer tokens.

---

# 1. Login and Retrieve a Token

```
curl -X POST http://localhost:8000/api/users/login \
  -H "Content-Type: application/json" \
  -d '{"username":"demo","password":"password123"}'
```

Example response:

```json
{ "token": "5|AcIFWuvGKehNRfo1hux8vIdtFg4lar6I25PATirc07372912" }
```

---

# 2. Test a Protected Route (Current Authenticated User)

```
curl -X GET http://localhost:8000/api/users/me \
  -H "Authorization: Bearer 5|AcIFWuvGKehNRfo1hux8vIdtFg4lar6I25PATirc07372912"
```

---

# 3. Update the Authenticated User's Password

```
curl -X PUT http://localhost:8000/api/users/me/password \
  -H "Authorization: Bearer 5|AcIFWuvGKehNRfo1hux8vIdtFg4lar6I25PATirc07372912" \
  -H "Content-Type: application/json" \
  -d '{"password":"newsecurepassword"}'
```

---

# 4. Create a New User

```
curl -X POST http://localhost:8000/api/users \
  -H "Content-Type: application/json" \
  -d '{"username":"bob","email":"bob@test.com","password":"pass"}'
```

---

# 5. List All Users

```
curl -X GET http://localhost:8000/api/users
```

---

# 6. Add a Friend Relationship

```
curl -X POST http://localhost:8000/api/users/1/friends \
  -H "Content-Type: application/json" \
  -d '{"friend_id": 2}'
```

---

# 7. List a User's Friends

```
curl -X GET http://localhost:8000/api/users/1/friends
```
