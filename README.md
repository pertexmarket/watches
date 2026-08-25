<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>مجموعة الساعات الرجالية الفاخرة</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;900&display=swap');

  :root {
    --bg: #0a0908;
    --card-bg: #17140f;
    --card-bg-2: #1e1a13;
    --gold: #c9a24b;
    --gold-light: #e8cd8a;
    --gold-dark: #9c7a2e;
    --bronze: #8c6239;
    --text-light: #f3ede0;
    --text-muted: #a89a7d;
    --line: rgba(201,162,75,0.18);
  }

  * { margin:0; padding:0; box-sizing:border-box; }
  body { font-family: 'Cairo', sans-serif; background: var(--bg); color: var(--text-light); overflow-x: hidden; padding-bottom: 90px; }

  .hero { text-align: center; padding: 46px 16px 26px; background: radial-gradient(ellipse at top, #1b160e 0%, #0a0908 70%); border-bottom: 1px solid var(--line); }
  .badge { background: rgba(201,162,75,0.1); color: var(--gold); padding: 6px 18px; border-radius: 20px; font-size: 12px; font-weight: 700; display: inline-block; margin-bottom: 14px; border: 1px solid var(--gold-dark); letter-spacing: 1px; }
  .hero h1 { font-size: clamp(24px, 6vw, 38px); font-weight: 900; line-height: 1.3; margin-bottom: 10px; color: transparent; background: linear-gradient(135deg, var(--gold-light), var(--gold-dark)); -webkit-background-clip: text; background-clip: text; }
  .hero p { font-size: 14px; color: var(--text-muted); max-width: 480px; margin: 0 auto; }

  .products-section { padding: 32px 16px 10px; max-width: 1000px; margin: 0 auto; }
  .section-title { text-align: center; font-size: 18px; font-weight: 700; margin-bottom: 20px; color: var(--gold); letter-spacing: 0.5px; }

  .products-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 16px; }

  .product-card { background: linear-gradient(180deg, var(--card-bg-2), var(--card-bg)); border-radius: 16px; padding: 14px; border: 1px solid var(--line); text-align: center; transition: 0.25s; }
  .product-card:hover { border-color: var(--gold-dark); transform: translateY(-3px); }
  .product-card.in-cart { border-color: var(--gold); box-shadow: 0 0 18px rgba(201,162,75,0.15); }

  .product-img-wrapper { width: 100%; height: 190px; border-radius: 12px; overflow: hidden; background: #0d0b08; margin-bottom: 12px; display: flex; align-items: center; justify-content: center; color: #665a3f; font-size: 13px; border: 1px solid var(--line); }
  .product-img-wrapper img { width: 100%; height: 100%; object-fit: cover; }

  .product-name { font-size: 14px; font-weight: 700; color: var(--text-light); min-height: 38px; margin-bottom: 4px; }
  .product-price { font-size: 17px; font-weight: 900; color: var(--gold); margin-bottom: 12px; }

  .qty-control { display: flex; align-items: center; justify-content: center; gap: 12px; background: rgba(255,255,255,0.03); border-radius: 12px; padding: 6px; border: 1px solid var(--line); }
  .qty-btn { width: 32px; height: 32px; border-radius: 8px; border: none; background: var(--gold-dark); color: #0a0908; font-size: 18px; font-weight: 900; cursor: pointer; display: flex; align-items: center; justify-content: center; transition: 0.15s; }
  .qty-btn:hover { background: var(--gold); }
  .qty-btn:active { transform: scale(0.92); }
  .qty-val { font-size: 16px; font-weight: 900; min-width: 22px; color: var(--text-light); }

  .special-card { border: 1px solid var(--bronze); background: linear-gradient(180deg, #221a10, var(--card-bg)); }
  .special-tag { position: absolute; }
  .special-note { font-size: 11px; color: var(--text-muted); margin-bottom: 8px; line-height: 1.5; }

  .floating-cart { position: fixed; bottom: 0; right: 0; left: 0; background: linear-gradient(135deg, #17140f, #0a0908); border-top: 1.5px solid var(--gold); padding: 12px 16px; display: none; align-items: center; justify-content: space-between; z-index: 50; box-shadow: 0 -6px 24px rgba(0,0,0,0.5); }
  .floating-cart.visible { display: flex; }
  .fc-info { font-size: 13px; color: var(--text-muted); }
  .fc-info b { color: var(--gold); font-size: 16px; }
  .fc-btn { background: linear-gradient(135deg, var(--gold-light), var(--gold-dark)); color: #0a0908; border: none; padding: 12px 22px; border-radius: 12px; font-family: 'Cairo', sans-serif; font-weight: 900; font-size: 14px; cursor: pointer; }

  .order-container { max-width: 560px; margin: 34px auto 40px; padding: 0 16px; }
  .order-card { background: #f8f5ee; color: #1c1a13; padding: 26px 20px; border-radius: 20px; box-shadow: 0 12px 34px rgba(0,0,0,0.5); border-top: 4px solid var(--gold); }
  .order-card h3 { text-align: center; font-size: 19px; font-weight: 900; margin-bottom: 18px; color: #1c1a13; }

  .form-group { margin-bottom: 14px; }
  .form-group label { display: block; font-size: 13px; font-weight: 700; margin-bottom: 6px; color: #4a4330; }
  .form-group input, .form-group select { width: 100%; padding: 12px 14px; border-radius: 10px; border: 1.5px solid #ddd3ba; font-family: 'Cairo', sans-serif; font-size: 14px; outline: none; transition: 0.2s; background: #fffdf8; }
  .form-group input:focus, .form-group select:focus { border-color: var(--gold-dark); }

  .delivery-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-bottom: 14px; }
  .delivery-btn { border: 2px solid #ddd3ba; border-radius: 12px; padding: 12px; text-align: center; cursor: pointer; transition: 0.2s; background: #fffdf8; }
  .delivery-btn.active { border-color: var(--gold-dark); background: rgba(201,162,75,0.12); }
  .delivery-btn.disabled-opt { opacity: 0.4; cursor: not-allowed; pointer-events: none; }
  .delivery-btn .d-title { font-size: 12px; font-weight: 700; }
  .delivery-btn .d-price { font-size: 14px; font-weight: 900; color: var(--gold-dark); margin-top: 2px; }

  .cart-summary { background: #fffdf8; border: 1px dashed #ddd3ba; border-radius: 12px; padding: 12px 14px; margin-bottom: 14px; }
  .cart-summary-title { font-size: 12px; font-weight: 700; color: #4a4330; margin-bottom: 8px; }
  .cart-line { display: flex; justify-content: space-between; font-size: 13px; color: #4a4330; padding: 4px 0; border-bottom: 1px solid #ede5d2; }
  .cart-line:last-child { border-bottom: none; }
  .cart-empty { font-size: 12px; color: #a89a7d; text-align: center; padding: 6px 0; }

  .summary { background: #ede5d2; padding: 16px; border-radius: 12px; margin: 6px 0 18px; border: 1px solid #ddd3ba; }
  .summary-row { display: flex; justify-content: space-between; font-size: 14px; padding: 4px 0; color: #4a4330; }
  .summary-row.total { font-size: 18px; font-weight: 900; color: #1c1a13; border-top: 1px solid #ddd3ba; padding-top: 8px; margin-top: 6px; }
  .summary-row.total span:last-child { color: var(--gold-dark); }

  .btn-submit { display: block; width: 100%; padding: 16px; border-radius: 12px; font-family: 'Cairo', sans-serif; font-size: 18px; font-weight: 900; border: none; background: linear-gradient(135deg, var(--gold-light), var(--gold-dark)); color: #1c1a13; cursor: pointer; transition: 0.2s; box-shadow: 0 6px 20px rgba(201,162,75,0.35); }
  .btn-submit:hover:not(:disabled) { transform: translateY(-2px); box-shadow: 0 8px 25px rgba(201,162,75,0.5); }
  .btn-submit:disabled { opacity: 0.5; cursor: not-allowed; }

  .faq-section { margin-top: 25px; border-top: 2px dashed #ddd3ba; padding-top: 20px; }
  .faq-title { font-size: 16px; font-weight: 900; color: #1c1a13; text-align: center; margin-bottom: 14px; }
  .faq-item { background: #fffdf8; border: 1px solid #ede5d2; border-radius: 12px; padding: 12px 16px; margin-bottom: 10px; }
  .faq-question { font-size: 13px; font-weight: 700; color: #1c1a13; margin-bottom: 4px; }
  .faq-answer { font-size: 13px; font-weight: 600; color: #6b7d3f; padding-right: 20px; }
</style>
</head>
<body>

<div class="hero">
  <span class="badge">⌚ تشكيلة حصرية للرجال</span>
  <h1>مجموعة الساعات الرجالية الفاخرة</h1>
  <p>8 موديلات أنيقة تناسب ذوقك، بالإضافة إلى بخاخ عطر عملي قابل لإعادة التعبئة — اختر ما يناسبك بكل حرية</p>
</div>

<div class="products-section">
  <div class="section-title">🛍️ تسوّق منتجاتنا</div>
  <div class="products-grid" id="products-grid"></div>
</div>

<div class="floating-cart" id="floating-cart">
  <div class="fc-info">عدد القطع: <b id="fc-count">0</b> — المجموع: <b id="fc-total">0 دج</b></div>
  <button class="fc-btn" onclick="scrollToOrder()">إتمام الطلب ←</button>
</div>

<div class="order-container" id="order-section">
  <div class="order-card">
    <h3>🛒 معلومات الطلب والتوصيل</h3>

    <div class="cart-summary">
      <div class="cart-summary-title">🧾 منتجاتك المختارة</div>
      <div id="cart-lines"><div class="cart-empty">لم تختر أي منتج بعد</div></div>
    </div>

    <div class="form-group">
      <label>الاسم واللقب</label>
      <input type="text" id="fullname" placeholder="أدخل اسمك الكامل">
    </div>

    <div class="form-group">
      <label>رقم الهاتف</label>
      <input type="tel" id="phone" placeholder="06XXXXXXXX">
    </div>

    <div class="form-group">
      <label>الولاية</label>
      <select id="wilaya" onchange="updateDelivery()">
        <option value="">— اختر الولاية —</option>
      </select>
    </div>

    <label style="font-size:13px; font-weight:700; margin-bottom:6px; display:block; color:#4a4330;">نوع التوصيل</label>
    <div class="delivery-grid">
      <div class="delivery-btn" id="btn-home" onclick="setDelivery('home')">
        <div class="d-title">🏠 للمنزل</div>
        <div class="d-price" id="p-home">—</div>
      </div>
      <div class="delivery-btn" id="btn-office" onclick="setDelivery('office')">
        <div class="d-title">🏢 للمكتب</div>
        <div class="d-price" id="p-office">—</div>
      </div>
    </div>

    <div class="form-group">
      <label>البلدية / العنوان</label>
      <input type="text" id="address" placeholder="اسم البلدية أو العنوان">
    </div>

    <div class="summary">
      <div class="summary-row"><span>مجموع المنتجات:</span><span id="sum-products">0 دج</span></div>
      <div class="summary-row"><span>سعر التوصيل:</span><span id="sum-del">—</span></div>
      <div class="summary-row total"><span>المجموع الكلي:</span><span id="sum-total">—</span></div>
    </div>

    <button class="btn-submit" id="submit-btn" onclick="sendOrder()" disabled>تأكيد الطلب الآن</button>

    <div class="faq-section">
      <div class="faq-title">❓ أسئلة شائعة</div>
      <div class="faq-item">
        <div class="faq-question">💳 طريقة الدفع؟</div>
        <div class="faq-answer">الدفع يد بيد عند استلام طلبيتك وإعادة معاينتها.</div>
      </div>
      <div class="faq-item">
        <div class="faq-question">🚚 مدة التوصيل؟</div>
        <div class="faq-answer">التوصيل سريع من يومين إلى ثلاثة أيام كأقصى حد.</div>
      </div>
    </div>
  </div>
</div>

<script>
var TELEGRAM_TOKEN = "8984328868:AAEjxhYfk_Iw6PhnSEIrsTZ3zCd_7zZHiLA";
var TELEGRAM_CHAT_ID = "8765345419";

var RATES = {
  "01 - Adrar": [1500, 750],
  "02 - Chlef": [900, 450],
  "03 - Laghouat": [1000, 500],
  "04 - Oum El Bouaghi": [750, 450],
  "05 - Batna": [450, 300],
  "06 - Bejaia": [800, 450],
  "07 - Biskra": [750, 450],
  "08 - Bechar": [1000, 500],
  "09 - Blida": [700, 450],
  "10 - Bouira": [900, 450],
  "11 - Tamanrasset": [1700, 800],
  "12 - Tebessa": [900, 450],
  "13 - Tlemcen": [950, 450],
  "14 - Tiaret": [950, 450],
  "15 - Tizi Ouzou": [700, 450],
  "16 - Alger": [700, 450],
  "17 - Djelfa": [1050, 600],
  "18 - Jijel": [800, 450],
  "19 - Setif": [700, 450],
  "20 - Saida": [900, 500],
  "21 - Skikda": [750, 450],
  "22 - Sidi Bel Abbes": [800, 450],
  "23 - Annaba": [750, 450],
  "24 - Guelma": [750, 450],
  "25 - Constantine": [700, 450],
  "26 - Medea": [800, 450],
  "27 - Mostaganem": [800, 450],
  "28 - Msila": [800, 450],
  "29 - Mascara": [800, 450],
  "30 - Ouargla": [900, 450],
  "31 - Oran": [800, 450],
  "32 - El Bayadh": [1150, 600],
  "33 - Illizi": [1700, 750],
  "34 - Bordj Bou Arreridj": [700, 450],
  "35 - Boumerdes": [700, 450],
  "36 - El Tarf": [750, 450],
  "37 - Tindouf": [1700, 0],
  "38 - Tissemsilt": [800, 450],
  "39 - El Oued": [900, 500],
  "40 - Khenchela": [600, 450],
  "41 - Souk Ahras": [700, 450],
  "42 - Tipaza": [850, 450],
  "43 - Mila": [700, 450],
  "44 - Ain Defla": [800, 450],
  "45 - Naama": [1050, 500],
  "46 - Ain Temouchent": [800, 450],
  "47 - Ghardaia": [950, 600],
  "48 - Relizane": [800, 500],
  "49 - Timimoun": [1400, 0],
  "50 - Bordj Badji Mokhtar": [1500, 0],
  "51 - Ouled Djellal": [950, 500],
  "52 - Beni Abbes": [1000, 0],
  "53 - In Salah": [1500, 750],
  "54 - In Guezzam": [1550, 0],
  "55 - Touggourt": [900, 500],
  "56 - Djanet": [1600, 750],
  "57 - El Mghair": [900, 500],
  "58 - El Meniaa": [1000, 0]
};

var PRODUCTS = [
  { id: 1, name: "ساعة يد رجالية - موديل 1", price: 2000, img: "صورة1.png" },
  { id: 2, name: "ساعة يد رجالية - موديل 2", price: 2000, img: "صورة2.png" },
  { id: 3, name: "ساعة يد رجالية - موديل 3", price: 1500, img: "صورة3.png" },
  { id: 4, name: "ساعة يد رجالية - موديل 4", price: 1500, img: "صورة4.png" },
  { id: 5, name: "ساعة يد رجالية - موديل 5", price: 1500, img: "صورة5.png" },
  { id: 6, name: "ساعة يد رجالية - موديل 6", price: 1500, img: "صورة6.png" },
  { id: 7, name: "ساعة يد رجالية - موديل 7", price: 1600, img: "صورة7.png" },
  { id: 8, name: "ساعة يد رجالية - موديل 8", price: 1600, img: "صورة8.png" },
  { id: 9, name: "بخاخ عطر قابل لإعادة التعبئة", price: 500, img: "صورة9.png", special: true }
];

var cart = {};
var currentDeliveryType = null;

function renderProducts() {
  var grid = document.getElementById('products-grid');
  var html = '';
  PRODUCTS.forEach(function(p) {
    html += '<div class="product-card' + (p.special ? ' special-card' : '') + '" id="card-' + p.id + '">' +
      '<div class="product-img-wrapper"><img src="' + p.img + '" alt="' + p.name + '" onerror="this.parentElement.innerHTML=\'صورة المنتج\'"></div>' +
      '<div class="product-name">' + p.name + '</div>' +
      (p.special ? '<div class="special-note">يُعبّأ بعطرك المفضّل — عملي وسهل الحمل</div>' : '') +
      '<div class="product-price">' + p.price + ' دج</div>' +
      '<div class="qty-control">' +
        '<button class="qty-btn" onclick="changeQty(' + p.id + ', -1)">−</button>' +
        '<div class="qty-val" id="qty-' + p.id + '">0</div>' +
        '<button class="qty-btn" onclick="changeQty(' + p.id + ', 1)">+</button>' +
      '</div>' +
    '</div>';
  });
  grid.innerHTML = html;
}

function changeQty(id, delta) {
  var current = cart[id] || 0;
  var next = current + delta;
  if (next < 0) next = 0;
  cart[id] = next;
  document.getElementById('qty-' + id).innerText = next;
  document.getElementById('card-' + id).classList.toggle('in-cart', next > 0);
  updateCartUI();
}

function getCartItems() {
  var items = [];
  PRODUCTS.forEach(function(p) {
    var qty = cart[p.id] || 0;
    if (qty > 0) items.push({ product: p, qty: qty, lineTotal: qty * p.price });
  });
  return items;
}

function getProductsSubtotal() {
  return getCartItems().reduce(function(sum, item) { return sum + item.lineTotal; }, 0);
}

function updateCartUI() {
  var items = getCartItems();
  var totalCount = items.reduce(function(s, i) { return s + i.qty; }, 0);
  var subtotal = getProductsSubtotal();

  var fc = document.getElementById('floating-cart');
  document.getElementById('fc-count').innerText = totalCount;
  document.getElementById('fc-total').innerText = subtotal + ' دج';
  fc.classList.toggle('visible', totalCount > 0);

  var linesHtml = '';
  if (items.length === 0) {
    linesHtml = '<div class="cart-empty">لم تختر أي منتج بعد</div>';
  } else {
    items.forEach(function(item) {
      linesHtml += '<div class="cart-line"><span>' + item.product.name + ' × ' + item.qty + '</span><span>' + item.lineTotal + ' دج</span></div>';
    });
  }
  document.getElementById('cart-lines').innerHTML = linesHtml;
  document.getElementById('sum-products').innerText = subtotal + ' دج';

  calculateTotal();
}

function scrollToOrder() {
  document.getElementById('order-section').scrollIntoView({ behavior: 'smooth', block: 'start' });
}

document.addEventListener("DOMContentLoaded", function() {
  renderProducts();
  var selectWilaya = document.getElementById("wilaya");
  for (var wilaya in RATES) {
    var option = document.createElement("option");
    option.value = wilaya;
    option.textContent = wilaya;
    selectWilaya.appendChild(option);
  }
});

function updateDelivery() {
  var selectWilaya = document.getElementById('wilaya');
  var w = selectWilaya.value;
  if (!w || !RATES[w]) return;

  var home = RATES[w][0];
  var office = RATES[w][1];
  var btnOffice = document.getElementById('btn-office');

  document.getElementById('p-home').innerText = home ? home + ' دج' : 'غير متوفر';

  if (office > 0) {
    document.getElementById('p-office').innerText = office + ' دج';
    btnOffice.classList.remove('disabled-opt');
  } else {
    document.getElementById('p-office').innerText = 'غير متوفر';
    btnOffice.classList.add('disabled-opt');
    if (currentDeliveryType === 'office') currentDeliveryType = null;
  }

  calculateTotal();
}

function setDelivery(type) {
  var selectWilaya = document.getElementById('wilaya');
  var w = selectWilaya.value;
  if (!w || !RATES[w]) return;

  if (type === 'office' && RATES[w][1] === 0) return;

  currentDeliveryType = type;
  document.getElementById('btn-home').classList.toggle('active', type === 'home');
  document.getElementById('btn-office').classList.toggle('active', type === 'office');
  calculateTotal();
}

function calculateTotal() {
  var selectWilaya = document.getElementById('wilaya');
  var w = selectWilaya.value;
  var subtotal = getProductsSubtotal();

  if (subtotal === 0 || !w || !currentDeliveryType || !RATES[w]) {
    document.getElementById('sum-del').innerText = '—';
    document.getElementById('sum-total').innerText = '—';
    document.getElementById('submit-btn').disabled = true;
    return;
  }

  var deliveryCost = currentDeliveryType === 'home' ? RATES[w][0] : RATES[w][1];
  if (deliveryCost === 0 && currentDeliveryType === 'office') {
    document.getElementById('submit-btn').disabled = true;
    return;
  }

  document.getElementById('sum-del').innerText = deliveryCost + ' دج';
  document.getElementById('sum-total').innerText = (subtotal + deliveryCost) + ' دج';
  document.getElementById('submit-btn').disabled = false;
}

function sendOrder() {
  var selectWilaya = document.getElementById('wilaya');
  var name = document.getElementById('fullname').value;
  var phone = document.getElementById('phone').value;
  var wilaya = selectWilaya.value;
  var address = document.getElementById('address').value;
  var items = getCartItems();
  var subtotal = getProductsSubtotal();
  var deliveryText = currentDeliveryType === 'home' ? 'توصيل للمنزل' : 'توصيل للمكتب';
  var deliveryCost = currentDeliveryType === 'home' ? RATES[wilaya][0] : RATES[wilaya][1];
  var total = subtotal + deliveryCost;

  if (!name || !phone) {
    alert('يرجى كتابة الاسم ورقم الهاتف');
    return;
  }
  if (items.length === 0) {
    alert('يرجى اختيار منتج واحد على الأقل');
    return;
  }

  var btn = document.getElementById('submit-btn');
  btn.disabled = true;
  btn.innerText = "جاري إرسال الطلب...";

  var itemsText = items.map(function(item) {
    return "• " + item.product.name + " × " + item.qty + " = " + item.lineTotal + " دج";
  }).join("\n");

  var message = "🛒 *طلبية جديدة (ساعات رجالية)*\n\n" +
                "👤 *الاسم:* " + name + "\n" +
                "📞 *الهاتف:* " + phone + "\n" +
                "📍 *الولاية:* " + wilaya + "\n" +
                "🏠 *العنوان/البلدية:* " + (address || 'غير محدد') + "\n\n" +
                "📦 *المنتجات:*\n" + itemsText + "\n\n" +
                "🚚 *نوع التوصيل:* " + deliveryText + " (" + deliveryCost + " دج)\n" +
                "💰 *مجموع المنتجات:* " + subtotal + " دج\n" +
                "💰 *المجموع الكلي:* " + total + " دج";

  fetch("https://api.telegram.org/bot" + TELEGRAM_TOKEN + "/sendMessage", {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({
      chat_id: TELEGRAM_CHAT_ID,
      text: message,
      parse_mode: 'Markdown'
    })
  })
  .then(function(res) { return res.json(); })
  .then(function(data) {
    if (data.ok) {
      alert('تم تسجيل طلبك بنجاح! وسنتصل بك قريباً لتأكيده.');
      location.reload();
    } else {
      alert('حدث خطأ أثناء إرسال الطلب، يرجى المحاولة لاحقاً.');
      btn.disabled = false;
      btn.innerText = "تأكيد الطلب الآن";
    }
  })
  .catch(function(err) {
    alert('تعذر الاتصال بالخادم، تحقق من الاتصال بالإنترنت.');
    btn.disabled = false;
    btn.innerText = "تأكيد الطلب الآن";
  });
}
</script>

</body>
</html>
