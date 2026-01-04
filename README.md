# SCIM 2.0 Postman Collection

This repository contains a structured **Postman collection for testing SCIM 2.0 APIs**, organized around **Users** and **Groups** resources.

The collection follows **SCIM 2.0 (RFC 7643 & RFC 7644)** standards and is designed from a **QA and API compliance perspective**, covering positive, negative, and edge-case scenarios.

---

## 📂 Collection Structure

```
SCIM-Postman-Collection
├── Users
│   ├── Create User
│   ├── Get User
│   ├── Filter User
│   ├── Update User (PUT)
│   ├── Update User (PATCH)
│   └── Delete User
│
└── Groups
    ├── Create Group
    ├── Get Group
    ├── Filter Group
    ├── Update Group (PUT)
    ├── Update Group (PATCH)
    └── Delete Group
```

---

## 👤 Users Coverage

The **Users** folder includes requests for:

- Creating a SCIM user
- Retrieving a user by ID
- Filtering users (e.g. `userName eq`)
- Updating users using PUT and PATCH
- Deleting users
- Validation of required attributes and SCIM-compliant error responses

---

## 👥 Groups Coverage

The **Groups** folder includes requests for:

- Creating a SCIM group
- Retrieving a group by ID
- Filtering groups
- Updating groups using PUT and PATCH
- Deleting groups
- Group membership validation

---

## 🧪 Test Coverage

Each request contains Postman test scripts that validate:

- HTTP status codes
- SCIM core schemas
- Required vs optional attributes
- PATCH operations behavior
- Error responses (`invalidValue`, `invalidSyntax`, `notFound`)
- UTF-8 support
- SCIM compliance best practices

---

## 🔐 Authentication

All requests use Bearer Token authentication:

Authorization: Bearer {{accessToken}}

---

## 🌍 Environment Variables

```
baseUrl      = https://example.com/scim/v2/
accessToken = <your_access_token>
userId      = <scim_user_id>
groupId     = <scim_group_id>
```

---

## ▶️ How to Use

1. Clone this repository
2. Import the Postman collection (.json) into Postman
3. Create and select a Postman environment
4. Set `baseUrl` and `accessToken`
5. Run requests individually or with Collection Runner

---

## 📚 References

- SCIM 2.0 Core Schema – RFC 7643
- SCIM 2.0 Protocol – RFC 7644

---

## 🛠 Tools

- Postman
- SCIM 2.0

---

## ✨ Author

Created with ❤️ by a QA Engineer 
