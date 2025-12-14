<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>NOVA - متجر الملابس الرجالي</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header class="site-header">
    <div class="container header-inner">
      <div class="logo">NOVA</div>
      <nav class="nav">
        <a href="index.html">الرئيسية</a>
        <a href="admin.html">لوحة الإدارة</a>
      </nav>
      <div class="cart-btn" id="cartBtn">السلة (<span id="cartCount">0</span>)</div>
    </div>
  </header>

  <main>
    <section class="hero container">
      <h1>أحدث تشكيلات الملابس الرجالي — NOVA</h1>
      <p>جودة عالية، توصيل سريع، تصميمات عصرية.</p>
    </section>

    <section id="products" class="container products-section">
      <!-- منتجات تُضاف بواسطة script.js -->
    </section>
  </main>

  <aside class="cart-drawer" id="cartDrawer" aria-hidden="true">
    <div class="cart-header">
      <h3>عربة التسوق</h3>
      <button id="closeCart">×</button>
    </div>
    <div id="cartItems" class="cart-items"></div>
    <div class="cart-footer">
      <div class="total">الإجمالي: <span id="cartTotal">0</span> ج.م</div>
      <button id="checkoutBtn" class="btn">الدفع</button>
    </div>
  </aside>

  <div class="overlay" id="overlay"></div>

  <div class="modal" id="checkoutModal" aria-hidden="true">
    <div class="modal-content">
      <button class="modal-close" id="closeModal">×</button>
      <h3>نموذج الدفع (تجريبي)</h3>
      <form id="checkoutForm">
        <label>الاسم الكامل<input name="name" required></label>
        <label>العنوان<input name="address" required></label>
        <label>الهاتف<input name="phone" required></label>
        <button type="submit" class="btn">تأكيد الطلب</button>
      </form>
      <div id="checkoutSuccess" class="hidden">
        <h4>تم إنشاء الطلب!</h4>
        <p>شكرًا لتسوقك لدى NOVA. سنعاود التواصل قريبًا.</p>
      </div>
    </div>
  </div>

  <script src="script.js"></script>
</body>
</html>
