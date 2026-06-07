# Django REST Framework (DRF) - Backend API Development

A comprehensive Django REST Framework learning repository covering REST API development from fundamentals to advanced concepts.

This repository contains hands-on implementations of Django REST Framework concepts including APIViews, Mixins, Generic Views, ViewSets, Serializers, Filtering, Searching, Pagination, and CRUD API development.

## 🚀 Tech Stack

* Python
* Django
* Django REST Framework (DRF)
* SQLite
* Postman
* Git & GitHub

---

## 📦 Project Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Backend-Api-Development-DRF.git
cd Backend-Api-Development-DRF
```

### 2. Create Virtual Environment

```bash
python -m venv venv
```

Activate virtual environment:

**Windows**

```bash
venv\Scripts\activate
```

**Linux / Mac**

```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Apply Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Run Development Server

```bash
python manage.py runserver
```

Server will start at:

```
http://127.0.0.1:8000/
```

---

## 📚 Topics Covered

### Django REST Framework Fundamentals

* Introduction to REST APIs
* API Architecture
* Request & Response Cycle
* JSON Data Handling
* HTTP Methods

  * GET
  * POST
  * PUT
  * PATCH
  * DELETE

---

### Serializers

* Serializer Class
* ModelSerializer
* Serializer Fields
* Validation
* Custom Validation
* Nested Serializers
* Serializer Relationships

---

### Views

#### Function Based Views (FBV)

* API View Decorators
* CRUD Operations
* Request Handling

#### Class Based Views (CBV)

* APIView
* CRUD Operations using APIView
* Request & Response Handling

---

### Mixins

Implementation of DRF Mixins:

* CreateModelMixin
* ListModelMixin
* RetrieveModelMixin
* UpdateModelMixin
* DestroyModelMixin

Benefits:

* Reusable code
* Cleaner architecture
* Less boilerplate
* Flexible CRUD combinations

---

### Generic Views

Working with:

* GenericAPIView
* CreateAPIView
* ListAPIView
* RetrieveAPIView
* UpdateAPIView
* DestroyAPIView
* ListCreateAPIView
* RetrieveUpdateAPIView
* RetrieveDestroyAPIView
* RetrieveUpdateDestroyAPIView

Generic views combine reusable mixins with GenericAPIView to reduce repetitive code.

---

### ViewSets

* ViewSet
* GenericViewSet
* ModelViewSet
* ReadOnlyModelViewSet

Features:

* Automatic CRUD operations
* Reduced code
* Router integration
* Clean API structure

---

### Routers

* SimpleRouter
* DefaultRouter
* Automatic URL generation

Example:

```python
router = DefaultRouter()
router.register('employees', EmployeeViewSet)
```

---

### Pagination

Implemented:

* PageNumberPagination
* Custom Pagination Classes

Features:

* Custom page size
* Dynamic page size
* API response optimization

---

### Filtering

API Filtering using:

```python
filter_backends
```

Features:

* Field based filtering
* Query parameter filtering
* Custom filter configurations

---

### Searching

Search functionality using:

```python
SearchFilter
```

Examples:

```http
/api/employees/?search=john
```

Features:

* Single field search
* Multiple field search
* Dynamic query search

---

### Ordering

Ordering results using:

```python
OrderingFilter
```

Examples:

```http
/api/employees/?ordering=name
```

```http
/api/employees/?ordering=-salary
```

---

### CRUD API Development

Implemented complete CRUD APIs for:

* Create Records
* Retrieve Records
* Update Records
* Delete Records

---

### API Testing

Tools Used:

* Postman
* DRF Browsable API

Tested:

* GET Requests
* POST Requests
* PUT Requests
* PATCH Requests
* DELETE Requests

---

## 📂 Project Structure

```text
project/
│
├── api/
│   ├── models.py
│   ├── serializers.py
│   ├── views.py
│   ├── urls.py
│   ├── paginations.py
│   └── filters.py
│
├── project/
│   ├── settings.py
│   └── urls.py
│
└── manage.py
```

---

## 🎯 Key Learning Outcomes

After completing this repository, you will understand:

* REST API design principles
* Serializer architecture
* APIView implementation
* Mixins and Generic Views
* ViewSets and Routers
* Filtering and Searching
* Pagination
* CRUD operations
* API testing workflows
* DRF best practices

---

## 🔥 DRF Learning Path Covered

```text
Function Based Views
        ↓
APIView
        ↓
Mixins
        ↓
GenericAPIView
        ↓
Generic Views
        ↓
ViewSets
        ↓
ModelViewSet
        ↓
Routers
        ↓
Pagination
        ↓
Filtering
        ↓
Searching
        ↓
Production Ready APIs
```

---

## 🤝 Contributions

Contributions, suggestions, and improvements are welcome.

Feel free to fork the repository and submit a pull request.

---

## ⭐ Support

If you found this repository helpful, consider giving it a ⭐ on GitHub.

Happy Coding! 🚀
