# 🚗 Car Rental Service — FastAPI Project

A complete **Car Rental Service backend** built with FastAPI covering all Day 1–6 internship concepts.

## 🚀 Run the Project

```bash
pip install -r requirements.txt
uvicorn main:app --reload
```

Open Swagger UI: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

---

## 📋 All 20 Endpoints

| # | Method | Endpoint | Description |
|---|--------|----------|-------------|
| Q1 | GET | `/` | Home route |
| Q2 | GET | `/cars` | List all cars |
| Q3 | GET | `/cars/{car_id}` | Get car by ID |
| Q4 | GET | `/cars/summary/stats` | Summary & stats |
| Q5 | POST | `/cars` | Add new car |
| Q6 | POST | `/bookings` | Create booking |
| Q7 | GET | `/cars/filter/search` | Filter by category/price/availability |
| Q8 | GET | `/cars/{car_id}/estimate` | Estimate rental price |
| Q9 | PUT | `/cars/{car_id}` | Update car |
| Q10 | DELETE | `/cars/{car_id}` | Delete car |
| Q11 | GET | `/bookings` | Get all bookings |
| Q12 | GET | `/bookings/{booking_id}` | Get booking by ID |
| Q13 | DELETE | `/bookings/{booking_id}` | Cancel booking |
| Q14 | POST | `/cart` | Add car to cart |
| Q15 | GET | `/cart` | View cart |
| Q16 | POST | `/cart/checkout` | Checkout cart → create bookings |
| Q17 | POST | `/bookings/{booking_id}/return` | Return car |
| Q18 | GET | `/rental-history` | View rental history |
| Q19 | GET | `/cars/search/keyword` | Keyword search |
| Q20 | GET | `/cars/browse/all` | Combined: search + filter + sort + paginate |

---

## 🛠 Concepts Implemented

- **Day 1** — GET APIs, home route, list, get by ID, summary
- **Day 2** — POST with Pydantic validation, field constraints, error handling
- **Day 3** — Helper functions (`find_car`, `calculate_total`, `filter_cars`), Query params
- **Day 4** — Full CRUD (POST, PUT, DELETE), 201/404 status codes
- **Day 5** — Multi-step workflow: Cart → Checkout → Return → History
- **Day 6** — Keyword search, sorting, pagination, combined browse endpoint
