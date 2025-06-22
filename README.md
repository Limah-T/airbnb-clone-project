# 🏡 Airbnb Clone – Backend API

## 🚀 Objective

The backend for the **Airbnb Clone** project is designed to provide a robust and scalable foundation for managing user interactions, property listings, bookings, payments, and reviews. Built with Django and Django REST Framework, this service ensures smooth and secure functionality for both hosts and guests.

---

## 🏆 Project Goals

- ✅ **User Management:** Secure registration, authentication, and profile features.
- ✅ **Property Management:** Create, update, and manage property listings.
- ✅ **Booking System:** Reserve properties and manage booking details.
- ✅ **Payment Processing:** Handle secure payment transactions.
- ✅ **Review System:** Enable users to rate and review properties.
- ✅ **Performance Optimization:** Enhance speed via indexing and caching.

---

## 🛠️ Features Overview

### 1. API Standards
- **REST API:** Built using Django REST Framework (DRF).
- **GraphQL:** Supports flexible data querying where required.
- **OpenAPI:** Complete API documentation with schema support.

### 2. Authentication
- **Endpoints:** `/users/`, `/users/{user_id}/`
- **Features:** Register, login, logout, and manage user profiles.

### 3. Property Listings
- **Endpoints:** `/properties/`, `/properties/{property_id}/`
- **Features:** CRUD operations for property listings.

### 4. Booking System
- **Endpoints:** `/bookings/`, `/bookings/{booking_id}/`
- **Features:** Book properties, update bookings, view history.

### 5. Payments
- **Endpoints:** `/payments/`
- **Features:** Payment gateway integration for secure transactions.

### 6. Reviews
- **Endpoints:** `/reviews/`, `/reviews/{review_id}/`
- **Features:** Leave and manage reviews on listings.

### 7. Performance Enhancements
- **Indexing:** On frequently queried fields.
- **Caching:** Redis used for optimized session and data storage.

---

## ⚙️ Technology Stack

| Category          | Tool / Technology                       |
|-------------------|------------------------------------------|
| **Framework**     | Django, Django REST Framework            |
| **Database**      | PostgreSQL                               |
| **Asynchronous**  | Celery + Redis (for background tasks)    |
| **Cache**         | Redis                                    |
| **API Format**    | REST (with optional GraphQL)             |
| **Containerization**| Docker                                 |
| **CI/CD**         | GitHub Actions or GitLab Pipelines       |
| **Documentation** | OpenAPI / Swagger UI                     |

---

## 📌 Endpoints Overview

### 👤 Users
- `GET /users/` - List users  
- `POST /users/` - Create a new user  
- `GET /users/{user_id}/` - Retrieve specific user  
- `PUT /users/{user_id}/` - Update user  
- `DELETE /users/{user_id}/` - Delete user  

### 🏠 Properties
- `GET /properties/` - List all properties  
- `POST /properties/` - Create new property  
- `GET /properties/{property_id}/` - Retrieve property  
- `PUT /properties/{property_id}/` - Update property  
- `DELETE /properties/{property_id}/` - Delete property  

### 📅 Bookings
- `GET /bookings/` - List all bookings  
- `POST /bookings/` - Create new booking  
- `GET /bookings/{booking_id}/` - Retrieve booking  
- `PUT /bookings/{booking_id}/` - Update booking  
- `DELETE /bookings/{booking_id}/` - Cancel booking  

### 💳 Payments
- `POST /payments/` - Process payment  

### 📝 Reviews
- `GET /reviews/` - List reviews  
- `POST /reviews/` - Create review  
- `GET /reviews/{review_id}/` - Retrieve review  
- `PUT /reviews/{review_id}/` - Update review  
- `DELETE /reviews/{review_id}/` - Delete review  

---

## 📂 Project Setup (Basic)

```bash
# Clone repository
git clone https://github.com/your-username/airbnb-clone-backend.git
cd airbnb-clone-backend

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Start the development server
python manage.py runserver

📫 Contact
Built with ❤️ by Limah Temitope
📧 Email: limahtechnology@yahoo.com
🔗 LinkedIn: https://www.linkedin.com/in/limah-temitope/