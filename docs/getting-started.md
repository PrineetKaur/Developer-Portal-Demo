# Payments API – Quick Start Guide

The Payments API allows you to create and manage transactions securely.

---

## 1. Authentication

All requests must include an API key in the `Authorization` header.

```bash
curl -X GET "https://api.example.com/v1/payments"   -H "Authorization: Bearer YOUR_API_KEY"
```

**Response**
```json
{
  "status": "success",
  "payments": []
}
```
