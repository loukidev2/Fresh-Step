<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Fresh Step - المتجر ولوحة التحكم</title>
  <style>
    body {
      margin: 0;
      font-family: sans-serif;
      background-color: #111;
      color: #fff;
    }
    header {
      background-color: #d32f2f;
      padding: 1rem;
      text-align: center;
      font-size: 2rem;
      font-weight: bold;
    }
    .container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      padding: 2rem;
    }
    .product {
      background: #222;
      margin: 1rem;
      padding: 1rem;
      border-radius: 1rem;
      width: 250px;
      box-shadow: 0 0 10px rgba(255, 0, 0, 0.3);
      text-align: center;
    }
    .product img {
      width: 100%;
      border-radius: 0.5rem;
    }
    .product h3 {
      margin: 1rem 0 0.5rem;
    }
    .product p {
      margin: 0.5rem 0;
    }
    .product a {
      display: inline-block;
      background: #d32f2f;
      color: white;
      padding: 0.5rem 1rem;
      margin-top: 1rem;
      border-radius: 0.5rem;
      text-decoration: none;
    }
    footer {
      text-align: center;
      padding: 2rem;
      font-size: 0.9rem;
      color: #aaa;
    }
    .admin-section {
      max-width: 600px;
      margin: 3rem auto;
      background: #222;
      padding: 2rem;
      border-radius: 1rem;
      box-shadow: 0 0 10px red;
    }
    input, textarea {
      width: 100%;
      padding: 0.5rem;
      margin: 0.5rem 0;
      border: none;
      border-radius: 0.5rem;
      font-size: 1rem;
    }
    button {
      background: #d32f2f;
      color: white;
      border: none;
      padding: 0.5rem 1rem;
      border-radius: 0.5rem;
      font-size: 1rem;
      cursor: pointer;
      margin-top: 1rem;
    }
    .hidden { display: none; }
    .product-item {
      border-top: 1px solid #444;
      padding: 0.5rem 0;
    }
  </style>
</head>
<body>
  <header>Fresh Step</header>
  <div class="container" id="store">
    <div class="product">
      <img src="https://via.placeholder.com/250x250?text=Rose+Scent" alt="Rose Scent Spray" />
      <h3>رشاش برائحة الورد</h3>
      <p>الثمن: 140 درهم</p>
      <a href="https://wa.me/?text=سلام، بغيت نطلب رشاش برائحة الورد بثمن 140 درهم">طلب عبر واتساب</a>
    </div>
    <div class="product">
      <img src="https://via.placeholder.com/250x250?text=Ocean+Scent" alt="Ocean Scent Spray" />
      <h3>رشاش برائحة البحر</h3>
      <p>الثمن: 140 درهم</p>
      <a href="https://wa.me/?text=سلام، بغيت نطلب رشاش برائحة البحر بثمن 140 درهم">طلب عبر واتساب</a>
    </div>
    <div class="product">
      <img src="https://via.placeholder.com/250x250?text=Lavender+Scent" alt="Lavender Scent Spray" />
      <h3>رشاش برائحة الخزامى</h3>
      <p>الثمن: 140 درهم</p>
      <a href="https://wa.me/?text=سلام، بغيت نطلب رشاش برائحة الخزامى بثمن 140 درهم">طلب عبر واتساب</a>
    </div>
  </div>  <div class="admin-section">
    <div id="adminLogin">
      <h3>دخول لوحة التحكم</h3>
      <input type="password" id="adminPassword" placeholder="كلمة السر" />
      <button onclick="unlockPanel()">دخول</button>
    </div><div id="adminPanel" class="hidden">
  <h3>لوحة التحكم</h3>
  <input type="text" id="productName" placeholder="اسم المنتج" />
  <input type="text" id="productPrice" placeholder="الثمن" />
  <input type="text" id="productImage" placeholder="رابط الصورة" />
  <textarea id="productDesc" placeholder="الوصف"></textarea>
  <button onclick="addProduct()">إضافة منتج</button>

  <div id="productList"></div>
</div>

  </div>  <footer>
    &copy; 2025 Fresh Step. جميع الحقوق محفوظة.
  </footer>  <script>
    function unlockPanel() {
      const pass = document.getElementById('adminPassword').value;
      if (pass === 'lokidev') {
        document.getElementById('adminLogin').classList.add('hidden');
        document.getElementById('adminPanel').classList.remove('hidden');
      } else {
        alert('كلمة السر غير صحيحة');
      }
    }

    function addProduct() {
      const name = document.getElementById('productName').value;
      const price = document.getElementById('productPrice').value;
      const image = document.getElementById('productImage').value;
      const desc = document.getElementById('productDesc').value;

      const list = document.getElementById('productList');
      const item = document.createElement('div');
      item.className = 'product-item';
      item.innerHTML = `
        <strong>${name}</strong><br>
        <img src="${image}" alt="${name}" style="width:80px;border-radius:0.5rem;"><br>
        <small>${desc}</small><br>
        <strong>${price} درهم</strong><br>
        <button onclick="this.parentNode.remove()">حذف</button>
      `;
      list.appendChild(item);

      // تفريغ الحقول
      document.getElementById('productName').value = '';
      document.getElementById('productPrice').value = '';
      document.getElementById('productImage').value = '';
      document.getElementById('productDesc').value = '';
    }
  </script></body>
</html>
