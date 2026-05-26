# API Endpoints

## Auth APIs

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/auth/register | Register user |
| POST | /api/auth/login | Login user |
| GET | /api/auth/profile | Get profile |

## Product APIs

| Method | Endpoint |
|--------|----------|
| GET | /api/products |
| GET | /api/products/{id} |
| POST | /api/products |
| PUT | /api/products/{id} |
| DELETE | /api/products/{id} |

## Cart APIs

| Method | Endpoint |
|--------|----------|
| POST | /api/cart/add |
| GET | /api/cart |
| DELETE | /api/cart/remove/{id} |

## Order APIs

| Method | Endpoint |
|--------|----------|
| POST | /api/orders |
| GET | /api/orders |
| GET | /api/orders/{id} |