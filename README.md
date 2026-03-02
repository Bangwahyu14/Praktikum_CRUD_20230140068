# 🚀 User Management API Documentation

**Base URL:** `http://localhost:8080`

---

## 🛠️ Daftar Endpoint (Methods)

### 1. ➕ Tambah User Baru (POST)
**Endpoint:** `/api/users`  
**Fungsi:** Menambahkan data user baru ke database.

**Request Body (JSON):**
```json
{
  "name": "Wahyu",
  "age": 10
}
```
Respon Sukses (201 Created):
```json
{
  "data": {
    "age": 10,
    "id": "0e467055-6bca-4fe4-9f18-70d74623e3d8",
    "name": "Wahyu"
  },
  "status": "success"
}
```

### 2. ➕ Melihat  User (GET)
**Endpoint:** `/api/users`  
**Fungsi:** Melihat data user baru.

**Respon Sukses (200):*

```json

{
  "status": "success",
  "data": {
    "age": 10,
    "id": "0e467055-6bca-4fe4-9f18-70d74623e3d8",
    "name": "Wahyu"
  }
}
```



### 3. ➕ Edit User  (PUT)
**Endpoint:** `http://localhost:8080/api/users/0e467055-6bca-4fe4-9f18-70d74623e3d8`  
**Fungsi:** Mengedit data user baru.

**Request Body (JSON):*

```json

{
  "name": "Wahyu",
  "age": 20
}
```
Respon Sukses (200):
```json
{
  "status": "success",
  "data": {
    "age": 20,
    "id": "0e467055-6bca-4fe4-9f18-70d74623e3d8",
    "name": "Wahyu"
  }
}
```

### 4. ➕ Delete User  (DELETE)
**Endpoint:** `http://localhost:8080/api/users/0e467055-6bca-4fe4-9f18-70d74623e3d8`  
**Fungsi:** Mengedit data user baru.

**Request Body (JSON):*

```json

{
  "name": "Wahyu",
  "age": 20
}
```
Respon Sukses (200):
```json
{
  "status": "success delete user with id 0e467055-6bca-4fe4-9f18-70d74623e3d8"
}
```