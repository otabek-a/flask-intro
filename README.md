
# Currency Converter API (UZS ↔ USD)

This is a simple Flask API that converts between **Uzbekistan (UZS)** and **United States Dollar (USD)**.  
It provides two endpoints:

- `/api/to-usd` → Converts **UZS to USD**
- `/api/to-uzs` → Converts **USD to UZS**

## 🚀 Getting Started

### **1. Clone the Repository**
```sh
git clone https://github.com/your-username/currency-converter-api.git
cd currency-converter-api
```

### **2. Install Dependencies**
Make sure you have Python installed, then install Flask:
```sh
pip install flask
```

### **3. Run the API**
```sh
python app.py
```
The API will start at `http://127.0.0.1:5000/`.

---

## 📌 API Endpoints

### **1️⃣ Convert UZS to USD**
**Endpoint:**  
```
GET /api/to-usd?amount=<amount>
```
**Example Request:**  
```sh
curl "http://127.0.0.1:5000/api/to-usd?amount=100000"
```
**Example Response:**
```json
{
    "amount": 100000,
    "currency": "UZS",
    "converted": 7.85,
    "convertedCurrency": "USD"
}
```

---

### **2️⃣ Convert USD to UZS**
**Endpoint:**  
```
GET /api/to-uzs?amount=<amount>
```
**Example Request:**  
```sh
curl "http://127.0.0.1:5000/api/to-uzs?amount=10"
```
**Example Response:**
```json
{
    "amount": 10,
    "currency": "USD",
    "converted": 127370,
    "convertedCurrency": "UZS"
}
```
