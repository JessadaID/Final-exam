# Restaurant Review System - Final Exam

## Project Overview
ระบบรีวิวร้านอาหารแบบ Fullstack โดยใช้ SQLite, Express.js, และ React.js

## ผู้จัดทำ
- นายเจษฎา บุญทา รหัส 66543206063-0

## เอกสาร
Google Docs : https://docs.google.com/document/d/1Obc4VLnfV6sN68to6BZWoah3ouQt3a0oB0N5Qu0MxXg/edit?usp=sharing

## Technology Stack
- Frontend: React 18, Vite, CSS3
- Backend: Node.js, Express.js
- Database: SQLite3
- API: REST API

## API Endpoints
Restaurants
- GET /api/restaurants - ดึงรายการร้านทั้งหมด (รองรับ filter)
- GET /api/restaurants/:id - ดึงรายละเอียดร้าน + reviews
- GET /api/restaurants/category/:category - ดึงร้านตามหมวดหมู่

Reviews
- GET /api/reviews/:restaurantId - ดึงรีวิวของร้าน
- POST /api/reviews - เพิ่มรีวิวใหม่

Stats
- GET /api/stats - ดึงสถิติระบบ

## Features
Required Features
- ✓ SQLite database + schema
- ✓ API endpoints (GET restaurants, POST reviews)
- ✓ Frontend components
- ✓ Search & filter functionality
- ✓ Input validation
- ✓ Error handling
- ✓ Loading states

Bonus Features 
- ✓ POST /api/restaurants (เพิ่มร้านใหม่)
- ✓ Category filtering
- ✓ Statistics API
- ✓ Responsive design

## Project Structure
```
restaurant-review-system/
├── backend/
│   ├── db/
│   │   ├── init.sql
│   │   ├── db.js
│   │   ├── seed.js
│   │   └── restaurant.db
│   ├── routes/
│   │   ├── restaurants.js
│   │   └── reviews.js
│   ├── middleware/
│   │   └── validation.js
│   ├── server.js
│   ├── package.json
│   └── .env
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── RestaurantList.jsx
│   │   │   ├── RestaurantCard.jsx
│   │   │   ├── RestaurantDetail.jsx
│   │   │   ├── SearchBar.jsx
│   │   │   ├── FilterPanel.jsx
│   │   │   ├── ReviewForm.jsx
│   │   │   └── ReviewList.jsx
│   │   ├── services/
│   │   │   └── api.js
│   │   ├── App.jsx
│   │   ├── App.css
│   │   ├── main.jsx
│   │   └── index.html
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```