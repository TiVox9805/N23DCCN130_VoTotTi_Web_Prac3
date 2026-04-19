# Fullstack Shop — LAB 3

Ứng dụng quản lý sản phẩm và giỏ hàng fullstack, kết nối **NextJS 15** (frontend) với **Express** (backend).

---
## Thông tin sinh viên

| Thông tin     | Chi tiết                                                             |
|---------------|----------------------------------------------------------------------|
| **Họ và tên** | Võ Tót Ti                                                  |
| **MSSV**      | N23DCCN130                                                           |

---

## Cấu trúc dự án

```
fullstack-shop/
├── backend/
│   ├── server.js       # Express server — toàn bộ API
│   ├── data.json       # Dữ liệu sản phẩm (tự tạo khi chạy lần đầu)
│   ├── cart.json       # Dữ liệu giỏ hàng (tự tạo khi chạy lần đầu)
│   └── package.json
└── frontend/
    ├── app/
    │   ├── products/page.tsx   # Trang quản lý sản phẩm
    │   ├── cart/page.tsx       # Trang giỏ hàng
    │   ├── layout.tsx          # Root layout + Toaster
    │   └── providers.tsx       # QueryClient + CartProvider
    ├── components/
    │   └── Header.tsx          # Navbar + badge giỏ hàng
    └── lib/
        ├── api.ts              # Axios instance
        ├── cartContext.tsx     # Cart state (React Context + React Query)
        └── toast.ts            # Toast helper tập trung
```

---

## Cài đặt và chạy

### 1. Clone / tải về

```bash
git clone https://github.com/WilliamsHugh/WilliamsHugh-N23DCCN060_TranTruongThuan_Web_Prac3.git
cd fullstack-shop
```

### 2. Chạy Backend

```bash
cd backend
npm install
node server.js
# Backend chạy tại http://localhost:5000
```

### 3. Chạy Frontend

Mở tab terminal mới:

```bash
cd frontend
npm install
npm run dev
# Frontend chạy tại http://localhost:3000
```

### 4. Mở trình duyệt

| URL | Trang |
|-----|-------|
| http://localhost:3000 | Trang chủ |
| http://localhost:3000/products | Quản lý sản phẩm |
| http://localhost:3000/cart | Giỏ hàng |
