<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>SMART PHONE ZONE – Latest Smartphones</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@500;600;700;800&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<script src="https://cdn.tailwindcss.com"></script>
<script>
tailwind.config = {
  theme: { extend: {
    colors: { ink:'#0a0f0d', panel:'#111a16', line:'#1f2d27', brand:{ DEFAULT:'#10b981', dark:'#059669' } },
    fontFamily: { head:['Poppins','sans-serif'], body:['Inter','sans-serif'] }
  } }
}
</script>
<style>
  :root { box-sizing:border-box; padding-top:env(safe-area-inset-top,0px); }
  html { height:100%; scroll-padding-top:env(safe-area-inset-top,0px); scroll-behavior:smooth; }
  body { font-family:'Inter',sans-serif; background:#0a0f0d; color:#e5efe9; min-height:100%; }
  .section { display:none; }
  .section.active { display:block; animation:fade .35s ease; }
  @keyframes fade { from{opacity:0;transform:translateY(8px)} to{opacity:1;transform:none} }
  .no-scrollbar::-webkit-scrollbar{display:none} .no-scrollbar{scrollbar-width:none}
  .glow { box-shadow:0 0 40px -10px rgba(16,185,129,.55); }
  .nav-btn.active { color:#10b981; }
  .tab.active { background:#10b981; color:#04130d; border-color:#10b981; }
  select,input,textarea { color-scheme:dark; }
</style>
</head>
<body class="pb-20 md:pb-0">

<header class="sticky top-0 z-40 bg-ink/90 backdrop-blur border-b border-line">
  <div class="max-w-6xl mx-auto px-4 h-16 flex items-center justify-between">
    <button onclick="showSection('home')" class="flex items-center gap-2">
      <span class="w-9 h-9 rounded-xl bg-brand flex items-center justify-center text-ink">
        <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><rect x="7" y="2" width="10" height="20" rx="2"/><path d="M11 18h2"/></svg>
      </span>
      <span class="font-head font-extrabold tracking-wide text-lg">SMART PHONE <span class="text-brand">ZONE</span></span>
    </button>
    <nav class="hidden md:flex items-center gap-1">
      <button class="nav-btn px-4 py-2 rounded-lg hover:text-brand font-medium" data-target="home" onclick="showSection('home')">Home</button>
      <button class="nav-btn px-4 py-2 rounded-lg hover:text-brand font-medium" data-target="catalog" onclick="showSection('catalog')">Phones</button>
      <button class="nav-btn px-4 py-2 rounded-lg hover:text-brand font-medium" data-target="booking" onclick="showSection('booking')">Enquire</button>
      <button class="nav-btn px-4 py-2 rounded-lg hover:text-brand font-medium" data-target="about" onclick="showSection('about')">About</button>
    </nav>
    <a href="tel:+918870027473" class="hidden sm:inline-flex bg-brand hover:bg-brand-dark text-ink font-semibold px-4 py-2 rounded-xl text-sm transition">📞 +91 88700 27473</a>
  </div>
</header>

<main class="max-w-6xl mx-auto px-4">

  <!-- HOME -->
  <section id="home" class="section active py-10 md:py-16">
    <div class="grid md:grid-cols-2 gap-10 items-center">
      <div>
        <span class="inline-block text-xs font-semibold tracking-widest uppercase text-brand bg-brand/10 border border-brand/30 px-3 py-1 rounded-full">Your One-Stop Mobile Store</span>
        <h1 class="font-head font-extrabold text-4xl sm:text-5xl lg:text-6xl leading-tight mt-5">Find Your Perfect <span class="text-brand">Smartphone</span> Today</h1>
        <p class="mt-5 text-lg text-gray-400 max-w-lg">From Samsung and iPhone to OnePlus, Vivo, OPPO and more — genuine phones, best prices, easy exchange and trusted after-sales support.</p>
        <div class="mt-8 flex flex-wrap gap-3">
          <button onclick="showSection('catalog')" class="bg-brand hover:bg-brand-dark text-ink font-semibold px-6 py-3 rounded-xl transition glow">Browse Phones</button>
          <button onclick="showSection('booking')" class="border border-brand text-brand hover:bg-brand hover:text-ink font-semibold px-6 py-3 rounded-xl transition">Enquire on WhatsApp</button>
        </div>
      </div>
      <div class="relative">
        <div class="absolute -inset-4 bg-brand/20 blur-3xl rounded-full"></div>
        <img id="heroImg" alt="Smartphones at Smart Phone Zone" class="relative rounded-3xl border border-line w-full h-72 sm:h-96 object-cover" onerror="imgFallback(this)">
      </div>
    </div>

    <div class="mt-14 grid sm:grid-cols-2 lg:grid-cols-4 gap-4">
      <div class="bg-panel border border-line rounded-2xl p-5 hover:border-brand/60 transition"><div class="text-2xl">✅</div><h3 class="font-head font-semibold mt-3">100% Genuine</h3><p class="text-sm text-gray-400 mt-1">Brand-new sealed phones with GST bill and warranty.</p></div>
      <div class="bg-panel border border-line rounded-2xl p-5 hover:border-brand/60 transition"><div class="text-2xl">💰</div><h3 class="font-head font-semibold mt-3">Best Price</h3><p class="text-sm text-gray-400 mt-1">Competitive prices, bank offers and easy EMI.</p></div>
      <div class="bg-panel border border-line rounded-2xl p-5 hover:border-brand/60 transition"><div class="text-2xl">🔄</div><h3 class="font-head font-semibold mt-3">Easy Exchange</h3><p class="text-sm text-gray-400 mt-1">Instant value for your old phone on any upgrade.</p></div>
      <div class="bg-panel border border-line rounded-2xl p-5 hover:border-brand/60 transition"><div class="text-2xl">🛠️</div><h3 class="font-head font-semibold mt-3">Service & Support</h3><p class="text-sm text-gray-400 mt-1">Screen guards, setup help and after-sales assistance.</p></div>
    </div>

    <div class="mt-14">
      <h2 class="font-head font-bold text-2xl mb-4">Brands We Carry</h2>
      <div id="brandChips" class="flex flex-wrap gap-2"></div>
    </div>
  </section>

  <!-- CATALOG -->
  <section id="catalog" class="section py-10">
    <h2 class="font-head font-extrabold text-3xl">Our <span class="text-brand">Phones</span></h2>
    <p class="text-gray-400 mt-2">Pick a brand to filter. Prices are approximate — message us for today's best offer.</p>
    <div id="filterTabs" class="mt-6 flex gap-2 overflow-x-auto no-scrollbar pb-2"></div>
    <div id="catalogGrid" class="mt-6 grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4"></div>
    <p id="emptyMsg" class="hidden text-center text-gray-400 py-10">No phones in this category yet.</p>
  </section>

  <!-- BOOKING -->
  <section id="booking" class="section py-10">
    <div class="max-w-2xl mx-auto">
      <h2 class="font-head font-extrabold text-3xl">Enquire / <span class="text-brand">Book on WhatsApp</span></h2>
      <p class="text-gray-400 mt-2">Fill in the details and your enquiry opens directly in WhatsApp.</p>
      <div class="mt-6 bg-panel border border-line rounded-2xl p-5 sm:p-7 space-y-5">
        <div class="grid sm:grid-cols-2 gap-4">
          <div><label class="block text-sm font-medium mb-1" for="fName">Your Name *</label>
            <input id="fName" type="text" placeholder="Enter your name" class="w-full bg-ink border border-line rounded-xl px-4 py-3 focus:outline-none focus:border-brand"></div>
          <div><label class="block text-sm font-medium mb-1" for="fPhone">Your Mobile Number *</label>
            <input id="fPhone" type="tel" inputmode="numeric" placeholder="10-digit number" class="w-full bg-ink border border-line rounded-xl px-4 py-3 focus:outline-none focus:border-brand"></div>
        </div>
        <div><label class="block text-sm font-medium mb-1" for="fType">I want to *</label>
          <select id="fType" class="w-full bg-ink border border-line rounded-xl px-4 py-3 focus:outline-none focus:border-brand">
            <option>Buy a new phone</option><option>Exchange my old phone</option><option>Get a price quote</option><option>Book a store visit</option>
          </select></div>
        <div class="grid sm:grid-cols-2 gap-4">
          <div><label class="block text-sm font-medium mb-1" for="fBrand">Brand *</label>
            <select id="fBrand" class="w-full bg-ink border border-line rounded-xl px-4 py-3 focus:outline-none focus:border-brand"></select></div>
          <div><label class="block text-sm font-medium mb-1" for="fModel">Model *</label>
            <select id="fModel" class="w-full bg-ink border border-line rounded-xl px-4 py-3 focus:outline-none focus:border-brand"></select></div>
        </div>
        <div class="grid sm:grid-cols-2 gap-4">
          <div><label class="block text-sm font-medium mb-1" for="fBudget">Budget</label>
            <select id="fBudget" class="w-full bg-ink border border-line rounded-xl px-4 py-3 focus:outline-none focus:border-brand">
              <option>Not decided</option><option>Under ₹10,000</option><option>₹10,000 – ₹20,000</option><option>₹20,000 – ₹35,000</option><option>₹35,000 – ₹60,000</option><option>Above ₹60,000</option>
            </select></div>
          <div><label class="block text-sm font-medium mb-1" for="fDate">Preferred Visit Date</label>
            <input id="fDate" type="date" class="w-full bg-ink border border-line rounded-xl px-4 py-3 focus:outline-none focus:border-brand"></div>
        </div>
        <div><label class="block text-sm font-medium mb-1" for="fMsg">Message (optional)</label>
          <textarea id="fMsg" rows="3" placeholder="Storage, colour, EMI, old phone details..." class="w-full bg-ink border border-line rounded-xl px-4 py-3 focus:outline-none focus:border-brand"></textarea></div>
        <p id="formError" class="hidden text-red-400 text-sm"></p>
        <button onclick="submitForm()" class="w-full bg-brand hover:bg-brand-dark text-ink font-semibold py-3.5 rounded-xl transition glow">💬 Send Enquiry on WhatsApp</button>
      </div>
    </div>
  </section>

  <!-- ABOUT -->
  <section id="about" class="section py-10 md:py-14">
    <div class="grid md:grid-cols-2 gap-10 items-center">
      <img id="aboutImg" alt="Smart Phone Zone store" class="rounded-3xl border border-line w-full h-72 md:h-96 object-cover" onerror="imgFallback(this)">
      <div>
        <h2 class="font-head font-extrabold text-3xl">About <span class="text-brand">Smart Phone Zone</span></h2>
        <p class="mt-4 text-gray-400">Smart Phone Zone is your trusted neighbourhood mobile store. We bring every popular smartphone brand under one roof, with honest advice, transparent pricing and friendly after-sales support.</p>
        <ul class="mt-5 space-y-2 text-gray-300">
          <li class="flex gap-2"><span class="text-brand">✔</span> Brand-new phones with warranty</li>
          <li class="flex gap-2"><span class="text-brand">✔</span> Exchange offers, EMI and finance help</li>
          <li class="flex gap-2"><span class="text-brand">✔</span> Accessories, screen guards and data transfer</li>
        </ul>
        <button onclick="showSection('booking')" class="mt-7 bg-brand hover:bg-brand-dark text-ink font-semibold px-6 py-3 rounded-xl transition">Talk to Us</button>
      </div>
    </div>
    <div class="mt-14 grid grid-cols-2 md:grid-cols-4 gap-4">
      <div class="bg-panel border border-line rounded-2xl p-6 text-center"><div class="font-head font-extrabold text-4xl text-brand"><span class="counter" data-to="5000">0</span>+</div><p class="text-sm text-gray-400 mt-1">Happy Customers</p></div>
      <div class="bg-panel border border-line rounded-2xl p-6 text-center"><div class="font-head font-extrabold text-4xl text-brand"><span class="counter" data-to="17">0</span></div><p class="text-sm text-gray-400 mt-1">Top Brands</p></div>
      <div class="bg-panel border border-line rounded-2xl p-6 text-center"><div class="font-head font-extrabold text-4xl text-brand"><span class="counter" data-to="300">0</span>+</div><p class="text-sm text-gray-400 mt-1">Models Available</p></div>
      <div class="bg-panel border border-line rounded-2xl p-6 text-center"><div class="font-head font-extrabold text-4xl text-brand"><span class="counter" data-to="98">0</span>%</div><p class="text-sm text-gray-400 mt-1">Satisfaction Rate</p></div>
    </div>
  </section>
</main>

<footer class="border-t border-line mt-10 py-8 text-center text-sm text-gray-500 px-4">
  <p class="font-head font-semibold text-gray-300">SMART PHONE ZONE</p>
  <p class="mt-1">Call / WhatsApp: <a class="text-brand" href="tel:+918870027473">+91 88700 27473</a></p>
  <p class="mt-1">&copy; <span id="yr"></span> Smart Phone Zone. Prices are indicative and may change.</p>
</footer>

<nav class="md:hidden fixed bottom-0 inset-x-0 z-40 bg-ink/95 backdrop-blur border-t border-line grid grid-cols-4" style="padding-bottom:env(safe-area-inset-bottom,0px)">
  <button class="nav-btn py-3 flex flex-col items-center text-xs text-gray-400" data-target="home" onclick="showSection('home')"><span class="text-lg">🏠</span>Home</button>
  <button class="nav-btn py-3 flex flex-col items-center text-xs text-gray-400" data-target="catalog" onclick="showSection('catalog')"><span class="text-lg">📱</span>Phones</button>
  <button class="nav-btn py-3 flex flex-col items-center text-xs text-gray-400" data-target="booking" onclick="showSection('booking')"><span class="text-lg">💬</span>Enquire</button>
  <button class="nav-btn py-3 flex flex-col items-center text-xs text-gray-400" data-target="about" onclick="showSection('about')"><span class="text-lg">ℹ️</span>About</button>
</nav>

<script>
  const SHOP_PHONE = "918870027473";

  // Brand-styled phone illustrations: [color1, color2, camera layout]
  const BRAND_STYLE = {
    "Samsung":["#1428a0","#0b1654","vert"], "Apple iPhone":["#9ca3af","#4b5563","tri"],
    "OnePlus":["#f5010c","#7a0006","circle"], "Vivo":["#415fff","#1a2a8a","circle"],
    "OPPO":["#1d9a6c","#0b4d36","circle"], "Xiaomi":["#ff6900","#8a3a00","circle"],
    "Redmi":["#e11d2e","#6b0f18","dual"], "Realme":["#ffc915","#8a6a00","circle"],
    "Motorola":["#0b6fb8","#063a63","dual"], "iQOO":["#2563eb","#111827","vert"],
    "Google Pixel":["#6b7280","#111827","bar"], "Nothing":["#e5e7eb","#9ca3af","glyph"],
    "POCO":["#f5c400","#3a3a3a","dual"], "HONOR":["#00a0e9","#0a3d62","circle"],
    "Infinix":["#7c3aed","#2e1065","dual"], "Tecno":["#0ea5e9","#0c4a6e","circle"],
    "Nokia":["#124191","#0a2150","dual"]
  };
  function svgImg(label, sub) {
    const st = BRAND_STYLE[sub] || ["#10b981", "#064e3b", "circle"];
    const c1 = st[0], c2 = st[1], cam = st[2];
    const lens = function (x, y, r) {
      return '<circle cx="' + x + '" cy="' + y + '" r="' + r + '" fill="#05080a" stroke="#cbd5e1" stroke-opacity=".6" stroke-width="2"/>' +
             '<circle cx="' + x + '" cy="' + y + '" r="' + (r * 0.4) + '" fill="#1e293b"/>';
    };
    let camSvg = "";
    if (cam === "tri") camSvg = '<rect x="160" y="40" width="48" height="48" rx="12" fill="#0b0f12" fill-opacity=".55"/>' + lens(173,53,8) + lens(195,53,8) + lens(184,75,8);
    else if (cam === "vert") camSvg = lens(172,52,8) + lens(172,74,8) + lens(172,96,8);
    else if (cam === "bar") camSvg = '<rect x="150" y="62" width="100" height="28" fill="#05080a" fill-opacity=".8"/>' + lens(180,76,10) + lens(212,76,10);
    else if (cam === "dual") camSvg = '<rect x="160" y="42" width="30" height="56" rx="15" fill="#05080a" fill-opacity=".6"/>' + lens(175,58,9) + lens(175,82,9);
    else if (cam === "glyph") camSvg = '<g stroke="#111827" stroke-width="3" stroke-linecap="round" fill="none"><path d="M170 120v40M185 130v30M200 110v50"/><circle cx="215" cy="140" r="6"/></g>' + lens(176,56,9) + lens(176,80,9);
    else camSvg = '<circle cx="186" cy="68" r="28" fill="#05080a" fill-opacity=".6" stroke="#cbd5e1" stroke-opacity=".5" stroke-width="2"/>' + lens(176,60,8) + lens(197,60,8) + lens(186,80,8);
    const esc = function (t) { return String(t).replace(/&/g, "&amp;").replace(/</g, "&lt;"); };
    const brandName = BRAND_STYLE[sub] ? sub.toUpperCase() : "";
    const s = '<svg xmlns="http://www.w3.org/2000/svg" width="400" height="300" viewBox="0 0 400 300">' +
      '<defs><linearGradient id="bg" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="' + c2 + '" stop-opacity=".55"/><stop offset="1" stop-color="#0a0f0d"/></linearGradient>' +
      '<linearGradient id="bd" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="' + c1 + '"/><stop offset="1" stop-color="' + c2 + '"/></linearGradient>' +
      '<linearGradient id="sh" x1="0" y1="0" x2="1" y2="0"><stop offset="0" stop-color="#fff" stop-opacity=".25"/><stop offset=".5" stop-color="#fff" stop-opacity="0"/></linearGradient></defs>' +
      '<rect width="400" height="300" fill="url(#bg)"/>' +
      '<ellipse cx="200" cy="208" rx="70" ry="8" fill="#000" opacity=".35"/>' +
      '<rect x="150" y="30" width="100" height="176" rx="18" fill="url(#bd)" stroke="#e5e7eb" stroke-opacity=".35" stroke-width="2"/>' +
      '<rect x="150" y="30" width="100" height="176" rx="18" fill="url(#sh)"/>' + camSvg +
      '<text x="200" y="240" font-family="Arial,sans-serif" font-weight="bold" font-size="15" fill="#ffffff" text-anchor="middle">' + esc(label) + '</text>' +
      '<text x="200" y="262" font-family="Arial,sans-serif" font-weight="bold" font-size="12" letter-spacing="3" fill="' + (c1 === "#e5e7eb" ? "#e5e7eb" : "#6ee7b7") + '" text-anchor="middle">' + esc(brandName || sub || "") + '</text></svg>';
    return 'data:image/svg+xml;utf8,' + encodeURIComponent(s);
  }
  
  const PLACEHOLDER = svgImg("Smart Phone Zone", "");
  function imgFallback(el) { el.onerror = null; el.src = PLACEHOLDER; }

  const BRANDS = {
    "Samsung": [["Galaxy S24 FE",54999,"AMOLED display, Exynos 2400e"],["Galaxy A55 5G",39999,"Metal frame, 50MP OIS camera"],["Galaxy M35 5G",19999,"6000mAh battery, 120Hz AMOLED"]],
    "Apple iPhone": [["iPhone 15",69900,"A16 Bionic, 48MP camera, USB-C"],["iPhone 16",79900,"A18 chip, Camera Control"],["iPhone 13",49900,"A15 Bionic, great value"]],
    "OnePlus": [["OnePlus 12R",39999,"Snapdragon 8 Gen 2, 100W"],["OnePlus Nord CE4",24999,"Snapdragon 7 Gen 3, 100W"],["Nord CE4 Lite",17999,"5500mAh, 80W charging"]],
    "Vivo": [["Vivo V40",34999,"Zeiss camera, curved AMOLED"],["Vivo T3 5G",19999,"Dimensity 7200, 120Hz AMOLED"],["Vivo Y28 5G",13999,"5000mAh battery, 5G"]],
    "OPPO": [["OPPO Reno12",32999,"AI portrait camera, 80W"],["OPPO F27 Pro+",27999,"IP69 rated, durable"],["OPPO A3x",11999,"Military-grade shock resistance"]],
    "Xiaomi": [["Xiaomi 14 Civi",42999,"Leica optics, 4700mAh"],["Xiaomi 13T",39999,"Leica camera, 144Hz display"],["Xiaomi Pad 6",24999,"11-inch 144Hz tablet"]],
    "Redmi": [["Redmi Note 13 Pro+",29999,"200MP camera, 120W charging"],["Redmi 13C 5G",10999,"Budget 5G, 90Hz display"],["Redmi Note 13",16999,"AMOLED, 108MP camera"]],
    "Realme": [["Realme 12 Pro+",29999,"Periscope telephoto camera"],["Realme Narzo 70 Pro",18999,"Sony IMX890 OIS camera"],["Realme C65 5G",10999,"Dimensity 6300, 5000mAh"]],
    "Motorola": [["Moto Edge 50 Fusion",22999,"pOLED curved display, 68W"],["Moto G85 5G",17999,"Curved pOLED, 5G"],["Moto G45 5G",10999,"Snapdragon 6s Gen 3, 120Hz"]],
    "iQOO": [["iQOO Neo 9 Pro",36999,"Snapdragon 8 Gen 2, gaming chip"],["iQOO Z9 5G",19999,"Dimensity 7200, 120W"],["iQOO Z9x 5G",12999,"6000mAh battery, 5G"]],
    "Google Pixel": [["Pixel 8a",52999,"Tensor G3, 7 years of updates"],["Pixel 8",64999,"Pure Android, AI camera"],["Pixel 9",79999,"Tensor G4, Gemini AI"]],
    "Nothing": [["Nothing Phone (2a)",23999,"Glyph interface, Dimensity 7200 Pro"],["Nothing Phone (2)",39999,"Snapdragon 8+ Gen 1"],["CMF Phone 1",15999,"Swappable back cases, AMOLED"]],
    "POCO": [["POCO X6 Pro 5G",24999,"Dimensity 8300 Ultra, 67W"],["POCO F6",29999,"Snapdragon 8s Gen 3, 90W"],["POCO M6 Pro 5G",11999,"Snapdragon 4 Gen 2, 5G"]],
    "HONOR": [["HONOR 200 5G",34999,"Studio Harcourt portrait camera"],["HONOR 200 Pro",57999,"Flagship camera, 100W"],["HONOR X9b",25999,"Anti-drop curved display"]],
    "Infinix": [["Infinix GT 20 Pro",21999,"Dimensity 8200, gaming"],["Infinix Zero 30 5G",23999,"108MP camera, curved AMOLED"],["Infinix Note 40X 5G",12999,"Dimensity 6300, 120Hz"]],
    "Tecno": [["Tecno Pova 6 Pro",19999,"108MP camera, 70W charging"],["Tecno Camon 30",21999,"50MP OIS camera"],["Tecno Spark 20 Pro+",15999,"Curved AMOLED, 108MP"]],
    "Nokia": [["Nokia G42 5G",12999,"Repairable design, 3-year updates"],["Nokia 105 Classic",1299,"Reliable feature phone"],["Nokia 110 4G",2199,"4G keypad phone, long battery"]]
  };

  const CATALOG = [];
  let idCounter = 1;
  Object.keys(BRANDS).forEach(function (brand) {
    BRANDS[brand].forEach(function (m) {
      CATALOG.push({
        id: idCounter++, name: m[0], category: brand, price: m[1],
        detail: "From ₹" + m[1].toLocaleString("en-IN"),
        image: svgImg(m[0], brand), description: m[2]
      });
    });
  });

  const CATEGORIES = Object.keys(BRANDS);
  let activeCategory = "All";

  function showSection(id) {
    document.querySelectorAll(".section").forEach(function (s) { s.classList.remove("active"); });
    document.getElementById(id).classList.add("active");
    document.querySelectorAll(".nav-btn").forEach(function (b) { b.classList.toggle("active", b.dataset.target === id); });
    window.scrollTo({ top: 0, behavior: "smooth" });
    if (id === "about") runCounters();
  }

  function renderTabs() {
    const wrap = document.getElementById("filterTabs");
    wrap.innerHTML = "";
    ["All"].concat(CATEGORIES).forEach(function (cat) {
      const b = document.createElement("button");
      b.textContent = cat;
      b.className = "tab whitespace-nowrap px-4 py-2 rounded-full border border-line text-sm font-medium text-gray-300 hover:border-brand transition" + (cat === activeCategory ? " active" : "");
      b.onclick = function () { activeCategory = cat; renderTabs(); renderCatalog(); };
      wrap.appendChild(b);
    });
  }

  function renderCatalog() {
    const grid = document.getElementById("catalogGrid");
    const items = activeCategory === "All" ? CATALOG : CATALOG.filter(function (i) { return i.category === activeCategory; });
    grid.innerHTML = "";
    document.getElementById("emptyMsg").classList.toggle("hidden", items.length > 0);
    items.forEach(function (item) {
      const card = document.createElement("div");
      card.className = "bg-panel border border-line rounded-2xl overflow-hidden hover:border-brand/60 transition flex flex-col";
      card.innerHTML =
        '<img src="' + item.image + '" alt="' + item.name + '" loading="lazy" class="w-full h-32 sm:h-40 object-cover" onerror="imgFallback(this)">' +
        '<div class="p-3 sm:p-4 flex flex-col flex-1">' +
          '<span class="text-[11px] uppercase tracking-wider text-brand font-semibold">' + item.category + '</span>' +
          '<h3 class="font-head font-semibold mt-1 leading-snug">' + item.name + '</h3>' +
          '<p class="text-xs text-gray-400 mt-1 flex-1">' + item.description + '</p>' +
          '<p class="font-semibold text-brand mt-2">' + item.detail + '</p>' +
          '<button class="mt-3 w-full bg-brand/10 hover:bg-brand hover:text-ink text-brand border border-brand/40 rounded-lg py-2 text-sm font-semibold transition" onclick="enquire(' + item.id + ')">Enquire Now</button>' +
        '</div>';
      grid.appendChild(card);
    });
  }

  function renderChips() {
    const wrap = document.getElementById("brandChips");
    CATEGORIES.forEach(function (c) {
      const b = document.createElement("button");
      b.textContent = c;
      b.className = "px-4 py-2 rounded-full bg-panel border border-line text-sm hover:border-brand hover:text-brand transition";
      b.onclick = function () { activeCategory = c; renderTabs(); renderCatalog(); showSection("catalog"); };
      wrap.appendChild(b);
    });
  }

  function populateBrands() {
    const sel = document.getElementById("fBrand");
    sel.innerHTML = '<option value="">Select brand</option>';
    CATEGORIES.forEach(function (c) {
      const o = document.createElement("option"); o.value = c; o.textContent = c; sel.appendChild(o);
    });
    sel.addEventListener("change", populateModels);
    populateModels();
  }

  function populateModels() {
    const brand = document.getElementById("fBrand").value;
    const sel = document.getElementById("fModel");
    if (!brand) { sel.innerHTML = '<option value="">Select a brand first</option>'; return; }
    sel.innerHTML = '<option value="">Select model</option>';
    CATALOG.filter(function (i) { return i.category === brand; }).forEach(function (i) {
      const o = document.createElement("option"); o.value = i.name; o.textContent = i.name + " (" + i.detail + ")"; sel.appendChild(o);
    });
    const other = document.createElement("option"); other.value = "Other / Not sure"; other.textContent = "Other / Not sure"; sel.appendChild(other);
  }

  function enquire(id) {
    const item = CATALOG.find(function (i) { return i.id === id; });
    showSection("booking");
    document.getElementById("fBrand").value = item.category;
    populateModels();
    document.getElementById("fModel").value = item.name;
  }

  function submitForm() {
    const v = function (id) { return document.getElementById(id).value.trim(); };
    const name = v("fName"), phone = v("fPhone"), type = v("fType"), brand = v("fBrand"),
          model = v("fModel"), budget = v("fBudget"), date = v("fDate"), msg = v("fMsg");
    const err = document.getElementById("formError");
    let problem = "";
    if (!name) problem = "Please enter your name.";
    else if (!/^[0-9+\s-]{10,15}$/.test(phone)) problem = "Please enter a valid mobile number.";
    else if (!brand) problem = "Please select a brand.";
    else if (!model) problem = "Please select a model.";
    if (problem) { err.textContent = problem; err.classList.remove("hidden"); return; }
    err.classList.add("hidden");
    const text = [
      "*New Enquiry – Smart Phone Zone*", "",
      "Name: " + name, "Mobile: " + phone, "Request: " + type,
      "Brand: " + brand, "Model: " + model, "Budget: " + budget,
      "Preferred Visit Date: " + (date || "Not specified"), "Message: " + (msg || "-")
    ].join("\n");
    const url = "https://wa.me/" + SHOP_PHONE + "?text=" + encodeURIComponent(text);
    const w = window.open(url, "_blank");
    if (!w) { window.location.href = url; }
  }

  let countersRan = false;
  function runCounters() {
    if (countersRan) return;
    countersRan = true;
    document.querySelectorAll(".counter").forEach(function (el) {
      const to = parseInt(el.dataset.to, 10), start = performance.now(), dur = 1400;
      function tick(now) {
        const p = Math.min((now - start) / dur, 1);
        el.textContent = Math.floor(to * (1 - Math.pow(1 - p, 3))).toLocaleString("en-IN");
        if (p < 1) requestAnimationFrame(tick);
      }
      requestAnimationFrame(tick);
    });
  }

  document.getElementById("heroImg").src = svgImg("SMART PHONE ZONE", "Latest smartphones, best prices");
  document.getElementById("aboutImg").src = svgImg("SMART PHONE ZONE", "Your trusted mobile store");
  document.getElementById("yr").textContent = new Date().getFullYear();
  document.getElementById("fDate").min = new Date().toISOString().split("T")[0];
  renderTabs(); renderCatalog(); renderChips(); populateBrands(); showSection("home");
</script>
</body>
</html>
