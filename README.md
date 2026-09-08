<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>بازار الأصالة | تحف وهدايا وإكسسوارات</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@500;700;800&family=Tajawal:wght@400;500;700&display=swap" rel="stylesheet">
<style>
  :root{
    --bg: #1a140f;
    --bg-card: #241b13;
    --bg-card-2: #2c2117;
    --gold: #c79a3d;
    --gold-light: #e0b95c;
    --teal: #2c6b5f;
    --text: #f3e9d6;
    --text-muted: #b3a184;
    --line: #3a2e20;
    --whatsapp: #3aa373;
  }
  *{ box-sizing:border-box; margin:0; padding:0; }
  html{ scroll-behavior:smooth; }
  body{
    background:
      radial-gradient(circle at 15% 0%, rgba(199,154,61,0.08), transparent 40%),
      radial-gradient(circle at 85% 20%, rgba(44,107,95,0.10), transparent 45%),
      var(--bg);
    color:var(--text);
    font-family:'Tajawal', sans-serif;
    line-height:1.6;
    padding-bottom:90px;
  }
  h1,h2,h3{ font-family:'Cairo', sans-serif; }
  a{ color:inherit; text-decoration:none; }
  img{ max-width:100%; display:block; }
  .container{ max-width:520px; margin:0 auto; padding:0 16px; }

  header.site-header{
    position:relative;
    padding:38px 16px 30px;
    text-align:center;
    background:
      linear-gradient(180deg, rgba(26,20,15,0.2), var(--bg) 90%),
      repeating-linear-gradient(135deg, rgba(199,154,61,0.06) 0 2px, transparent 2px 22px);
    border-bottom:1px solid var(--line);
  }
  .brand-mark{
    width:56px; height:56px;
    margin:0 auto 14px;
    border:1.5px solid var(--gold);
    border-radius:50%;
    display:flex; align-items:center; justify-content:center;
    font-size:24px;
    color:var(--gold-light);
    background:rgba(199,154,61,0.06);
  }
  header.site-header h1{
    font-size:26px;
    font-weight:800;
    color:var(--gold-light);
    letter-spacing:0.5px;
  }
  header.site-header p.tagline{
    margin-top:8px;
    color:var(--text-muted);
    font-size:14px;
  }

  nav.categories{
    display:flex;
    gap:10px;
    overflow-x:auto;
    padding:14px 16px;
    background:var(--bg);
    position:sticky;
    top:0;
    z-index:20;
    border-bottom:1px solid var(--line);
    -ms-overflow-style:none;
    scrollbar-width:none;
  }
  nav.categories::-webkit-scrollbar{ display:none; }
  nav.categories a{
    flex:0 0 auto;
    padding:8px 18px;
    border:1px solid var(--line);
    border-radius:20px;
    font-size:13.5px;
    font-weight:700;
    color:var(--text-muted);
    background:var(--bg-card);
    white-space:nowrap;
    transition:border-color .2s, color .2s;
  }
  nav.categories a:active,
  nav.categories a:focus-visible{
    border-color:var(--gold);
    color:var(--gold-light);
  }

  section.category{
    padding:30px 16px 8px;
    scroll-margin-top:64px;
  }
  .category-heading{
    display:flex;
    align-items:baseline;
    gap:10px;
    margin-bottom:4px;
  }
  .category-heading h2{
    font-size:20px;
    font-weight:800;
    color:var(--text);
  }
  .category-heading span.count{
    font-size:12.5px;
    color:var(--text-muted);
  }
  .category-underline{
    width:38px;
    height:3px;
    background:var(--gold);
    border-radius:3px;
    margin:8px 0 18px;
  }
  .product-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:14px;
  }

  .product-card{
    background:var(--bg-card);
    border:1px solid var(--line);
    border-radius:14px;
    overflow:hidden;
    display:flex;
    flex-direction:column;
  }
  .product-image{
    aspect-ratio:1/1;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:34px;
    background:
      radial-gradient(circle at 30% 20%, rgba(224,185,92,0.18), transparent 55%),
      var(--bg-card-2);
    border-bottom:1px solid var(--line);
    color:var(--gold-light);
  }
  .product-image img{ width:100%; height:100%; object-fit:cover; }
  .product-info{
    padding:12px 12px 14px;
    display:flex;
    flex-direction:column;
    gap:6px;
    flex:1;
  }
  .product-info h3{
    font-size:14.5px;
    font-weight:700;
    color:var(--text);
  }
  .product-price{
    font-size:14px;
    font-weight:800;
    color:var(--gold-light);
    font-family:'Cairo', sans-serif;
  }
  .product-order-btn{
    margin-top:auto;
    display:flex;
    align-items:center;
    justify-content:center;
    gap:6px;
    padding:8px 6px;
    border-radius:8px;
    background:rgba(58,163,115,0.12);
    border:1px solid rgba(58,163,115,0.4);
    color:#7fd6ac;
    font-size:12.5px;
    font-weight:700;
  }
  .product-order-btn svg{ width:14px; height:14px; flex:0 0 auto; }

  .section-divider{
    max-width:520px;
    margin:26px auto 0;
    padding:0 16px;
  }
  .section-divider .line{
    height:1px;
    background:linear-gradient(90deg, transparent, var(--line), transparent);
  }

  section.about{
    padding:34px 16px 10px;
    text-align:center;
  }
  section.about h2{
    font-size:18px;
    color:var(--gold-light);
    margin-bottom:16px;
  }
  .about-points{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:10px;
  }
  .about-points div{
    background:var(--bg-card);
    border:1px solid var(--line);
    border-radius:12px;
    padding:14px 6px;
    font-size:12px;
    color:var(--text-muted);
  }
  .about-points span{
    display:block;
    font-size:20px;
    margin-bottom:6px;
  }

  footer{
    margin-top:34px;
    padding:26px 16px 10px;
    text-align:center;
    color:var(--text-muted);
    font-size:12.5px;
    border-top:1px solid var(--line);
  }
  footer strong{ color:var(--gold-light); }

  .whatsapp-float{
    position:fixed;
    bottom:18px;
    left:50%;
    transform:translateX(-50%);
    width:calc(100% - 32px);
    max-width:488px;
    display:flex;
    align-items:center;
    justify-content:center;
    gap:10px;
    padding:14px 20px;
    background:var(--whatsapp);
    color:#0d1f16;
    font-family:'Cairo', sans-serif;
    font-weight:700;
    font-size:15px;
    border-radius:14px;
    box-shadow:0 10px 24px rgba(0,0,0,0.4);
    z-index:30;
  }
  .whatsapp-float svg{ width:20px; height:20px; flex:0 0 auto; }

  @media (prefers-reduced-motion: reduce){
    html{ scroll-behavior:auto; }
  }
</style>
</head>
<body>

  <header class="site-header">
    <div class="brand-mark">۞</div>
    <h1>بازار الأصالة</h1>
    <p class="tagline">تحف وهدايا وإكسسوارات مختارة بعناية</p>
  </header>

  <nav class="categories">
    <a href="#antiques">تحف</a>
    <a href="#gifts">هدايا</a>
    <a href="#accessories">إكسسوارات</a>
  </nav>

  <section class="category" id="antiques">
    <div class="container">
      <div class="category-heading">
        <h2>تحف</h2>
        <span class="count">قطع فريدة</span>
      </div>
      <div class="category-underline"></div>
      <div class="product-grid">

        <div class="product-card">
          <div class="product-image"><img src="https://via.placeholder.com/300x300/2c2117/e0b95c?text=%D8%B5%D9%88%D8%B1%D8%A9" alt="إبريق نحاسي مزخرف"></div>
          <div class="product-info">
            <h3>إبريق نحاسي مزخرف</h3>
            <div class="product-price">450 ج.م</div>
            <a class="product-order-btn" target="_blank" href="https://wa.me/201000000000?text=مرحباً%2C%20أريد%20الاستفسار%20عن%20منتج%3A%20إبريق%20نحاسي%20مزخرف">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12c0 1.85.5 3.58 1.36 5.07L2 22l5.05-1.32A9.94 9.94 0 0012 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm0 18c-1.6 0-3.1-.42-4.4-1.16l-.32-.19-3.03.8.8-2.95-.2-.32A7.94 7.94 0 014 12c0-4.41 3.59-8 8-8s8 3.59 8 8-3.59 8-8 8z"/></svg>
              اطلب
            </a>
          </div>
        </div>

        <div class="product-card">
          <div class="product-image"><img src="https://via.placeholder.com/300x300/2c2117/e0b95c?text=%D8%B5%D9%88%D8%B1%D8%A9" alt="فانوس نحاسي يدوي"></div>
          <div class="product-info">
            <h3>فانوس نحاسي يدوي</h3>
            <div class="product-price">320 ج.م</div>
            <a class="product-order-btn" target="_blank" href="https://wa.me/201000000000?text=مرحباً%2C%20أريد%20الاستفسار%20عن%20منتج%3A%20فانوس%20نحاسي%20يدوي">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12c0 1.85.5 3.58 1.36 5.07L2 22l5.05-1.32A9.94 9.94 0 0012 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm0 18c-1.6 0-3.1-.42-4.4-1.16l-.32-.19-3.03.8.8-2.95-.2-.32A7.94 7.94 0 014 12c0-4.41 3.59-8 8-8s8 3.59 8 8-3.59 8-8 8z"/></svg>
              اطلب
            </a>
          </div>
        </div>

        <div class="product-card">
          <div class="product-image"><img src="https://via.placeholder.com/300x300/2c2117/e0b95c?text=%D8%B5%D9%88%D8%B1%D8%A9" alt="مرآة إطار خشبي عتيق"></div>
          <div class="product-info">
            <h3>مرآة إطار خشبي عتيق</h3>
            <div class="product-price">680 ج.م</div>
            <a class="product-order-btn" target="_blank" href="https://wa.me/201000000000?text=مرحباً%2C%20أريد%20الاستفسار%20عن%20منتج%3A%20مرآة%20إطار%20خشبي%20عتيق">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12c0 1.85.5 3.58 1.36 5.07L2 22l5.05-1.32A9.94 9.94 0 0012 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm0 18c-1.6 0-3.1-.42-4.4-1.16l-.32-.19-3.03.8.8-2.95-.2-.32A7.94 7.94 0 014 12c0-4.41 3.59-8 8-8s8 3.59 8 8-3.59 8-8 8z"/></svg>
              اطلب
            </a>
          </div>
        </div>

        <div class="product-card">
          <div class="product-image"><img src="https://via.placeholder.com/300x300/2c2117/e0b95c?text=%D8%B5%D9%88%D8%B1%D8%A9" alt="صندوق خشبي محفور"></div>
          <div class="product-info">
            <h3>صندوق خشبي محفور</h3>
            <div class="product-price">250 ج.م</div>
            <a class="product-order-btn" target="_blank" href="https://wa.me/201000000000?text=مرحباً%2C%20أريد%20الاستفسار%20عن%20منتج%3A%20صندوق%20خشبي%20محفور">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12c0 1.85.5 3.58 1.36 5.07L2 22l5.05-1.32A9.94 9.94 0 0012 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm0 18c-1.6 0-3.1-.42-4.4-1.16l-.32-.19-3.03.8.8-2.95-.2-.32A7.94 7.94 0 014 12c0-4.41 3.59-8 8-8s8 3.59 8 8-3.59 8-8 8z"/></svg>
              اطلب
            </a>
          </div>
        </div>

      </div>
    </div>
  </section>

  <div class="section-divider"><div class="line"></div></div>

  <section class="category" id="gifts">
    <div class="container">
      <div class="category-heading">
        <h2>هدايا</h2>
        <span class="count">لكل المناسبات</span>
      </div>
      <div class="category-underline"></div>
      <div class="product-grid">

        <div class="product-card">
          <div class="product-image"><img src="https://via.placeholder.com/300x300/2c2117/e0b95c?text=%D8%B5%D9%88%D8%B1%D8%A9" alt="طقم هدايا مميز"></div>
          <div class="product-info">
            <h3>طقم هدايا مميز</h3>
            <div class="product-price">380 ج.م</div>
            <a class="product-order-btn" target="_blank" href="https://wa.me/201000000000?text=مرحباً%2C%20أريد%20الاستفسار%20عن%20منتج%3A%20طقم%20هدايا%20مميز">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12c0 1.85.5 3.58 1.36 5.07L2 22l5.05-1.32A9.94 9.94 0 0012 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm0 18c-1.6 0-3.1-.42-4.4-1.16l-.32-.19-3.03.8.8-2.95-.2-.32A7.94 7.94 0 014 12c0-4.41 3.59-8 8-8s8 3.59 8 8-3.59 8-8 8z"/></svg>
              اطلب
            </a>
          </div>
        </div>

        <div class="product-card">
          <div class="product-image"><img src="https://via.placeholder.com/300x300/2c2117/e0b95c?text=%D8%B5%D9%88%D8%B1%D8%A9" alt="لوحة تفريغ خشبية"></div>
          <div class="product-info">
            <h3>لوحة تفريغ خشبية</h3>
            <div class="product-price">290 ج.م</div>
            <a class="product-order-btn" target="_blank" href="https://wa.me/201000000000?text=مرحباً%2C%20أريد%20الاستفسار%20عن%20منتج%3A%20لوحة%20تفريغ%20خشبية">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12c0 1.85.5 3.58 1.36 5.07L2 22l5.05-1.32A9.94 9.94 0 0012 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm0 18c-1.6 0-3.1-.42-4.4-1.16l-.32-.19-3.03.8.8-2.95-.2-.32A7.94 7.94 0 014 12c0-4.41 3.59-8 8-8s8 3.59 8 8-3.59 8-8 8z"/></svg>
              اطلب
            </a>
          </div>
        </div>

        <div class="product-card">
          <div class="product-image"><img src="https://via.placeholder.com/300x300/2c2117/e0b95c?text=%D8%B5%D9%88%D8%B1%D8%A9" alt="وشاح حرير مطرز"></div>
          <div class="product-info">
            <h3>وشاح حرير مطرز</h3>
            <div class="product-price">340 ج.م</div>
            <a class="product-order-btn" target="_blank" href="https://wa.me/201000000000?text=مرحباً%2C%20أريد%20الاستفسار%20عن%20منتج%3A%20وشاح%20حرير%20مطرز">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12c0 1.85.5 3.58 1.36 5.07L2 22l5.05-1.32A9.94 9.94 0 0012 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm0 18c-1.6 0-3.1-.42-4.4-1.16l-.32-.19-3.03.8.8-2.95-.2-.32A7.94 7.94 0 014 12c0-4.41 3.59-8 8-8s8 3.59 8 8-3.59 8-8 8z"/></svg>
              اطلب
            </a>
          </div>
        </div>

        <div class="product-card">
          <div class="product-image"><img src="https://via.placeholder.com/300x300/2c2117/e0b95c?text=%D8%B5%D9%88%D8%B1%D8%A9" alt="سلة هدايا طبيعية"></div>
          <div class="product-info">
            <h3>سلة هدايا طبيعية</h3>
            <div class="product-price">410 ج.م</div>
            <a class="product-order-btn" target="_blank" href="https://wa.me/201000000000?text=مرحباً%2C%20أريد%20الاستفسار%20عن%20منتج%3A%20سلة%20هدايا%20طبيعية">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12c0 1.85.5 3.58 1.36 5.07L2 22l5.05-1.32A9.94 9.94 0 0012 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm0 18c-1.6 0-3.1-.42-4.4-1.16l-.32-.19-3.03.8.8-2.95-.2-.32A7.94 7.94 0 014 12c0-4.41 3.59-8 8-8s8 3.59 8 8-3.59 8-8 8z"/></svg>
              اطلب
            </a>
          </div>
        </div>

      </div>
    </div>
  </section>

  <div class="section-divider"><div class="line"></div></div>

  <section class="category" id="accessories">
    <div class="container">
      <div class="category-heading">
        <h2>إكسسوارات</h2>
        <span class="count">لمسة أناقة</span>
      </div>
      <div class="category-underline"></div>
      <div class="product-grid">

        <div class="product-card">
          <div class="product-image"><img src="https://via.placeholder.com/300x300/2c2117/e0b95c?text=%D8%B5%D9%88%D8%B1%D8%A9" alt="خاتم فضة مرصع"></div>
          <div class="product-info">
            <h3>خاتم فضة مرصع</h3>
            <div class="product-price">220 ج.م</div>
            <a class="product-order-btn" target="_blank" href="https://wa.me/201000000000?text=مرحباً%2C%20أريد%20الاستفسار%20عن%20منتج%3A%20خاتم%20فضة%20مرصع">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12c0 1.85.5 3.58 1.36 5.07L2 22l5.05-1.32A9.94 9.94 0 0012 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm0 18c-1.6 0-3.1-.42-4.4-1.16l-.32-.19-3.03.8.8-2.95-.2-.32A7.94 7.94 0 014 12c0-4.41 3.59-8 8-8s8 3.59 8 8-3.59 8-8 8z"/></svg>
              اطلب
            </a>
          </div>
        </div>

        <div class="product-card">
          <div class="product-image"><img src="https://via.placeholder.com/300x300/2c2117/e0b95c?text=%D8%B5%D9%88%D8%B1%D8%A9" alt="عقد خرز يدوي"></div>
          <div class="product-info">
            <h3>عقد خرز يدوي</h3>
            <div class="product-price">180 ج.م</div>
            <a class="product-order-btn" target="_blank" href="https://wa.me/201000000000?text=مرحباً%2C%20أريد%20الاستفسار%20عن%20منتج%3A%20عقد%20خرز%20يدوي">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12c0 1.85.5 3.58 1.36 5.07L2 22l5.05-1.32A9.94 9.94 0 0012 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm0 18c-1.6 0-3.1-.42-4.4-1.16l-.32-.19-3.03.8.8-2.95-.2-.32A7.94 7.94 0 014 12c0-4.41 3.59-8 8-8s8 3.59 8 8-3.59 8-8 8z"/></svg>
              اطلب
            </a>
          </div>
        </div>

        <div class="product-card">
          <div class="product-image"><img src="https://via.placeholder.com/300x300/2c2117/e0b95c?text=%D8%B5%D9%88%D8%B1%D8%A9" alt="حقيبة جلد طبيعي"></div>
          <div class="product-info">
            <h3>حقيبة جلد طبيعي</h3>
            <div class="product-price">550 ج.م</div>
            <a class="product-order-btn" target="_blank" href="https://wa.me/201000000000?text=مرحباً%2C%20أريد%20الاستفسار%20عن%20منتج%3A%20حقيبة%20جلد%20طبيعي">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12c0 1.85.5 3.58 1.36 5.07L2 22l5.05-1.32A9.94 9.94 0 0012 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm0 18c-1.6 0-3.1-.42-4.4-1.16l-.32-.19-3.03.8.8-2.95-.2-.32A7.94 7.94 0 014 12c0-4.41 3.59-8 8-8s8 3.59 8 8-3.59 8-8 8z"/></svg>
              اطلب
            </a>
          </div>
        </div>

        <div class="product-card">
          <div class="product-image"><img src="https://via.placeholder.com/300x300/2c2117/e0b95c?text=%D8%B5%D9%88%D8%B1%D8%A9" alt="سوار نحاسي منقوش"></div>
          <div class="product-info">
            <h3>سوار نحاسي منقوش</h3>
            <div class="product-price">160 ج.م</div>
            <a class="product-order-btn" target="_blank" href="https://wa.me/201000000000?text=مرحباً%2C%20أريد%20الاستفسار%20عن%20منتج%3A%20سوار%20نحاسي%20منقوش">
              <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12c0 1.85.5 3.58 1.36 5.07L2 22l5.05-1.32A9.94 9.94 0 0012 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm0 18c-1.6 0-3.1-.42-4.4-1.16l-.32-.19-3.03.8.8-2.95-.2-.32A7.94 7.94 0 014 12c0-4.41 3.59-8 8-8s8 3.59 8 8-3.59 8-8 8z"/></svg>
              اطلب
            </a>
          </div>
        </div>

      </div>
    </div>
  </section>

  <section class="about">
    <div class="container">
      <h2>لماذا بازار الأصالة</h2>
      <div class="about-points">
        <div><span>✋</span>صناعة يدوية</div>
        <div><span>🚚</span>توصيل لكل المحافظات</div>
        <div><span>💬</span>رد سريع على واتساب</div>
      </div>
    </div>
  </section>

  <footer>
    <p><strong>بازار الأصالة</strong> — تحف وهدايا وإكسسوارات</p>
    <p style="margin-top:6px;">للاستفسار والطلب تواصل معنا مباشرة عبر واتساب</p>
  </footer>

  <a class="whatsapp-float" target="_blank" href="https://wa.me/201000000000?text=مرحباً%2C%20أريد%20الاستفسار%20عن%20منتجات%20بازار%20الأصالة">
    <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12c0 1.85.5 3.58 1.36 5.07L2 22l5.05-1.32A9.94 9.94 0 0012 22c5.52 0 10-4.48 10-10S17.52 2 12 2zm0 18c-1.6 0-3.1-.42-4.4-1.16l-.32-.19-3.03.8.8-2.95-.2-.32A7.94 7.94 0 014 12c0-4.41 3.59-8 8-8s8 3.59 8 8-3.59 8-8 8z"/></svg>
    التواصل عبر الواتساب
  </a>

</body>
</html>