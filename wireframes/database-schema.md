# Database Schema

## USERS

| Column | Type |
|--------|------|
| id | BIGINT |
| full_name | VARCHAR |
| email | VARCHAR |
| password | VARCHAR |
| role | VARCHAR |

---

## PRODUCTS

| Column | Type |
|--------|------|
| id | BIGINT |
| name | VARCHAR |
| description | TEXT |
| price | DOUBLE |
| image_url | VARCHAR |

---

## ORDERS

| Column | Type |
|--------|------|
| id | BIGINT |
| user_id | BIGINT |
| total_price | DOUBLE |
| status | VARCHAR |

# CART TABLE

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| id | BIGINT | Primary Key |
| user_id | BIGINT | User who owns the cart |
| created_at | TIMESTAMP | Cart creation time |

---

# CART_ITEMS TABLE

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| id | BIGINT | Primary Key |
| cart_id | BIGINT | Connected cart id |
| product_id | BIGINT | Product id |
| quantity | INT | Number of products |
| price | DOUBLE | Product price |

---

# ORDER_ITEMS TABLE

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| id | BIGINT | Primary Key |
| order_id | BIGINT | Connected order id |
| product_id | BIGINT | Product id |
| quantity | INT | Product quantity |
| price | DOUBLE | Product price at order time |