# Payments API Reference

## POST /v1/payments

Creates a new payment.

**Request Example**
```bash
curl -X POST "https://api.example.com/v1/payments"   -H "Authorization: Bearer YOUR_API_KEY"   -H "Content-Type: application/json"   -d '{
        "amount": 100,
        "currency": "EUR",
        "recipient": "john.doe@example.com"
      }'
```

**Response Example**
```json
{
  "payment_id": "pmt_123456789",
  "status": "pending"
}
```
