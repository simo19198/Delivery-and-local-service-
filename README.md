# Delivery-and-local-service-
توصيل و خدمات محلية
```html
<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>موقع خدمات محلية</title>
<style>
  body {
    font-family: Arial, sans-serif;
    background: #f5f5f5;
    direction: rtl;
    margin: 0; padding: 0;
  }
  header {
    background: #007bff;
    color: white;
    padding: 15px;
    text-align: center;
  }.container {
    max-width: 900px;
    margin: 20px auto;
    background: white;
    padding: 20px;
    border-radius: 8px;
  }
  h2 {
    margin-bottom: 15px;
  }.services {
    display: flex;
    flex-wrap: wrap;
    gap: 15px;
    justify-content: center;
  }.service {
    background: #e7f1ff;
    border-radius: 8px;
    flex: 1 1 120px;
    max-width: 140px;
    text-align: center;
    padding: 15px;
    cursor: pointer;
    transition: background 0.3s ease;
  }.service:hover {
    background: #cce4ff;
  }.service img {
    width: 50px;
    height: 50px;
    margin-bottom: 10px;
  }
  form {
    margin-top: 30px;
    display: flex;
    flex-direction: column;
    gap: 12px;
  }
  input, textarea, select {
    padding: 10px;
    border-radius: 6px;
    border: 1px solid #ccc;
    font-size: 16px;
  }
  button {
    background: #007bff;
    color: white;
    border: none;
    padding: 12px;
    font-size: 18px;
    border-radius: 6px;
    cursor: pointer;
    transition: background 0.3s ease;
  }
  button:hover {
    background: #0056b3;
  }
</style>
</head>
<body>

<header>
  <h1>موقع التوصيل والخدمات المحلية</h1>
</header>

<div class="container">
  <h2>خدماتنا</h2>
  <div class="services">
    <div class="service">
      <img src="https://img.icons8.com/dusk/64/000000/delivery--v1.png" alt="توصيل"/>
      <div>توصيل</div>
    </div>
    <div class="service">
      <img src="https://img.icons8.com/dusk/64/000000/cleaning.png" alt="تنظيف"/>
      <div>تنظيف</div>
    </div>
    <div class="service">
      <img src="https://img.icons8.com/dusk/64/000000/home-repair.png" alt="صيانة"/>
      <div>صيانة</div>
    </div>
    <div class="service">
      <img src="https://img.icons8.com/dusk/64/000000/cooking-book.png" alt="طبخ"/>
      <div>طبخ منزلي</div>
    </div>
  </div>

  <h2>اطلب خدمتكم الآن</h2>
  <form id="orderForm">
    <select required>
      <option value="" disabled selected>اختر الخدمة</option>
      <option value="توصيل">توصيل</option>
      <option value="تنظيف">تنظيف</option>
      <option value="صيانة">صيانة</option>
      <option value="طبخ منزلي">طبخ منزلي</option>
    </select>
    <input type="text" placeholder="الاسم الكامل" required />
    <input type="tel" placeholder="رقم الهاتف" required />
    <textarea placeholder="تفاصيل الطلب" rows="4" required></textarea>
    <button type="submit">أرسل الطلب</button>
  </form>
</div>

<script>
  document.getElementById('orderForm').addEventListener('submit', function(e) {
    e.preventDefault();
    alert('شكراً لطلبكم! سيتم التواصل معكم قريبا.');
    this.reset();
  });
</script>

</body>
</html>
```

