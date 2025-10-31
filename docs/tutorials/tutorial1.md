# Tutorial – Build Your First App

This tutorial walks you through building a simple app that uses the Payments API.

## Prerequisites
- Python 3.8+
- `requests` library installed

## Steps

1. Install dependencies
```bash
pip install requests
```

2. Create a new Python file:
```python
import requests

API_KEY = "YOUR_API_KEY"
url = "https://api.example.com/v1/payments"

data = {"amount": 50, "currency": "EUR", "recipient": "jane.doe@example.com"}

response = requests.post(url, headers={"Authorization": f"Bearer {API_KEY}"}, json=data)
print(response.json())
```

3. Run the script and verify the payment response.
