
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#0b1726">
<title>WORLD EVENTS | رویدادهای جهان</title>

<style>
:root{
 --navy:#0b1726;
 --navy2:#12253b;
 --blue:#167dce;
 --light:#f3f7fc;
 --white:#fff;
 --text:#172b43;
 --muted:#718198;
}
*{box-sizing:border-box}
body{
 margin:0;
 font-family:Tahoma,Arial,sans-serif;
 background:var(--light);
 color:var(--text);
}
a{text-decoration:none;color:inherit}
button,input{font-family:inherit}
.container{width:min(1150px,94%);margin:auto}

/* HEADER */
header{
 background:linear-gradient(120deg,#091522,#142d49);
 color:white;
 padding:17px 0;
}
.header-content{
 display:flex;align-items:center;
 justify-content:space-between;gap:15px;
}
.brand{display:flex;align-items:center;gap:11px}
.logo{
 width:48px;height:48px;border-radius:14px;
 display:grid;place-items:center;
 background:linear-gradient(145deg,#168de8,#07549a);
 font-size:23px;font-weight:bold;
 box-shadow:0 5px 20px #0878c855;
}
.brand h1{font-size:19px;margin:0;letter-spacing:1px}
.brand p{font-size:11px;color:#a9c6e5;margin:6px 0 0}
.header-links{display:flex;gap:17px;font-size:12px;color:#d6e7fa}
.header-links a:hover{color:#52b2ff}

/* NAVIGATION */
nav{
 background:#10233a;color:white;
 border-top:1px solid #ffffff12;
}
.nav-content{
 display:flex;align-items:center;gap:24px;
 overflow-x:auto;white-space:nowrap;
 padding:13px 0;font-size:12px;
}
.nav-content a:hover{color:#53b4ff}
.menu-button{
 display:none;background:none;color:white;
 border:1px solid #49617b;padding:8px 12px;
 border-radius:8px;font-size:19px;
}

/* BREAKING */
.breaking{
 margin:20px auto 0;
 background:#fff;border:1px solid #e1e9f2;
 border-radius:12px;overflow:hidden;
 display:flex;align-items:center;
 box-shadow:0 4px 15px #173b5b0a;
}
.breaking-label{
 background:#147dce;color:white;
 padding:15px;font-size:12px;font-weight:bold;
 white-space:nowrap;
}
.breaking-text{
 padding:12px 15px;font-size:12px;
 color:#344a62;
}

/* HERO */
.hero{
 margin-top:22px;
 display:grid;
 grid-template-columns:1.5fr 1fr;
 gap:17px;
}
.hero-main{
 min-height:300px;
 border-radius:17px;overflow:hidden;
 position:relative;
 background:
 linear-gradient(0deg,#061322eF,transparent 90%),
 linear-gradient(135deg,#155d92,#10243b 65%,#071522);
 color:white;
 display:flex;align-items:end;
 padding:25px;
}
.hero-main:before{
 content:"🌍";position:absolute;
 font-size:125px;opacity:.12;
 top:25px;left:30px;
}
.hero-main h2{font-size:24px;line-height:1.8;margin:10px 0}
.hero-main p{font-size:12px;color:#c9dced;line-height:2}
.tag{
 display:inline-block;
 background:#1686db;color:white;
 padding:6px 11px;border-radius:6px;
 font-size:10px;
}
.hero-side{display:grid;gap:14px}
.hero-small{
 border-radius:15px;padding:20px;
 color:white;display:flex;flex-direction:column;
 justify-content:end;min-height:140px;
 background:linear-gradient(130deg,#174c78,#0d1c30);
}
.hero-small:nth-child(2){
 background:linear-gradient(130deg,#166d9e,#112a42);
}
.hero-small h3{font-size:15px;line-height:1.8;margin:9px 0 0}

/* SECTION */
.section{margin-top:34px}
.section-title{
 display:flex;align-items:center;
 justify-content:space-between;
 margin-bottom:17px;
}
.section-title h2{
 font-size:18px;margin:0;
 border-right:4px solid var(--blue);
 padding-right:11px;
}
.section-title a{font-size:11px;color:var(--blue)}

/* NEWS CARDS */
.news-grid{
 display:grid;
 grid-template-columns:repeat(3,1fr);
 gap:16px;
}
.news-card{
 background:white;border:1px solid #e5ebf2;
 border-radius:14px;overflow:hidden;
 transition:.2s;
}
.news-card:hover{
 transform:translateY(-4px);
 box-shadow:0 10px 25px #173b5b12;
}
.news-image{
 height:165px;
 display:grid;place-items:center;
 font-size:48px;color:white;
 background:linear-gradient(135deg,#1b6595,#0c2036);
}
.news-card:nth-child(3n+2) .news-image{
 background:linear-gradient(135deg,#275e78,#142a43)
}
.news-card:nth-child(3n) .news-image{
 background:linear-gradient(135deg,#246b91,#101d32)
}
.news-body{padding:15px}
.news-category{font-size:10px;color:var(--blue)}
.news-body h3{
 font-size:14px;line-height:2;
 margin:9px 0;color:#152c45;
}
.news-body p{
 font-size:11px;line-height:2;
 color:var(--muted);margin:0 0 12px;
}
.news-time{font-size:10px;color:#98a6b6}

/* CATEGORIES */
.category-grid{
 display:grid;
 grid-template-columns:repeat(5,1fr);
 gap:12px;
}
.category{
 background:white;border:1px solid #e4ebf3;
 padding:18px 8px;border-radius:12px;
 text-align:center;font-size:12px;
 transition:.2s;
}
.category:hover{
 border-color:var(--blue);
 background:#eaf5ff;
}
.category span{display:block;font-size:25px;margin-bottom:10px}

/* NEWSLETTER */
.join{
 margin:38px 0;
 padding:27px;
 border-radius:17px;
 color:white;
 background:linear-gradient(120deg,#0b1b2d,#15538a);
 display:flex;align-items:center;
 justify-content:space-between;gap:15px;
}
.join h2{font-size:19px;margin:0 0 9px}
.join p{font-size:11px;color:#c5d9ed;line-height:2}
.join a{
 background:#1688dc;color:white;
 padding:12px 17px;border-radius:9px;
 font-size:12px;white-space:nowrap;
}

/* FOOTER */
footer{
 background:#091522;color:#dce9f7;
 padding:30px 0 18px;
}
.footer-grid{
 display:grid;grid-template-columns:2fr 1fr 1fr;
 gap:25px;
}
footer h3{font-size:15px;color:#54aef5}
footer p,footer a{
 font-size:11px;color:#a9bdd1;line-height:2.3;
}
.footer-links{display:flex;flex-direction:column}
.copyright{
 border-top:1px solid #ffffff19;
 text-align:center;padding-top:17px;
 margin-top:25px;color:#7890a9;font-size:10px;
}

/* SEARCH */
.search-box{margin-top:22px}
.search-box input{
 width:100%;padding:15px 17px;
 border:1px solid #dce5ef;border-radius:11px;
 outline:none;background:white;font-size:12px;
}
.search-box input:focus{border-color:var(--blue)}
.empty{
 display:none;text-align:center;
 padding:25px;color:var(--muted);font-size:13px;
}
@media(max-width:700px){
 .header-content{flex-wrap:wrap}
 .header-links{display:none}
 .menu-button{display:block}
 nav{display:none}
 nav.open{display:block}
 .nav-content{flex-direction:column;align-items:stretch;gap:0}
 .nav-content a{padding:12px 4px;border-bottom:1px solid #ffffff12}
 .hero{grid-template-columns:1fr}
 .hero-main{min-height:250px}
 .hero-side{grid-template-columns:1fr 1fr}
 .hero-small{min-height:130px;padding:13px}
 .hero-small h3{font-size:12px}
 .news-grid{grid-template-columns:1fr 1fr;gap:10px}
 .news-image{height:120px}
 .news-body{padding:11px}
 .news-body h3{font-size:12px}
 .news-body p{font-size:10px}
 .category-grid{grid-template-columns:repeat(3,1fr);gap:8px}
 .category{font-size:10px;padding:14px 5px}
 .join{flex-direction:column;align-items:flex-start}
 .footer-grid{grid-template-columns:1fr 1fr}
 .footer-grid>div:first-child{grid-column:1/-1}
}
@media(max-width:380px){
 .news-grid{grid-template-columns:1fr}
 .hero-side{grid-template-columns:1fr}
}
</style>
</head>

<body>

<header>
 <div class="container header-content">
  <div class="brand">
   <div class="logo">🌍</div>
   <div>
    <h1>WORLD EVENTS</h1>
    <p>رویدادهای جهان | از جهان باخبر باشید</p>
   </div>
  </div>
  <div class="header-links">
   <a href="https://ble.ir/WORLDEVENTS">کانال رسمی</a>
   <a href="https://ble.ir/WORLDEVENTSCHAT">گروه گفت‌وگو</a>
   <a href="#about">درباره ما</a>
  </div>
  <button class="menu-button" onclick="toggleMenu()">☰</button>
 </div>
</header>

<nav id="navigation">
 <div class="container nav-content">
  <a href="#">صفحه اصلی</a>
  <a href="#latest">آخرین اخبار</a>
  <a href="#categories">اخبار جهان</a>
  <a href="#categories">اقتصاد</a>
  <a href="#categories">علم و دانش</a>
  <a href="#categories">ورزش</a>
  <a href="#categories">فناوری</a>
  <a href="#categories">سیاست و دیپلماسی</a>
  <a href="#categories">روزنامه و مطبوعات</a>
 </div>
</nav>

<main class="container">

 <div class="breaking">
  <div class="breaking-label">⚡ اخبار فوری</div>
  <div class="breaking-text" id="breakingText">
   به بخش اخبار فوری WORLD EVENTS خوش آمدید.
  </div>
 </div>

 <div class="search-box">
  <input id="search" type="search"
   placeholder="🔍 جست‌وجو در میان اخبار..."
   oninput="searchNews()">
 </div>

 <section class="hero">
  <div class="hero-main">
   <div>
    <span class="tag">رسانه خبری WORLD EVENTS</span>
    <h2>پنجره‌ای به تازه‌ترین رویدادهای جهان</h2>
    <p>
     تازه‌ترین اخبار، تحولات بین‌المللی و رویدادهای مهم
     را در WORLD EVENTS دنبال کنید.
    </p>
   </div>
  </div>
  <div class="hero-side">
   <div class="hero-small">
    <span class="tag">اخبار جهان</span>
    <h3>تحولات و رویدادهای بین‌المللی</h3>
   </div>
   <div class="hero-small">
    <span class="tag">فناوری</span>
    <h3>نگاهی به دنیای علم و فناوری</h3>
   </div>
  </div>
 </section>

 <section class="section" id="latest">
  <div class="section-title">
   <h2>آخرین اخبار</h2>
   <a href="#latest">مشاهده همه ←</a>
  </div>

  <div class="news-grid" id="newsGrid">

   <article class="news-card" data-category="جهان">
    <div class="news-image">🌍</div>
    <div class="news-body">
     <span class="news-category">اخبار جهان</span>
     <h3>رویدادهای مهم جهان را دنبال کنید</h3>
     <p>آخرین تحولات بین‌المللی و اتفاقات مهم جهان در این بخش منتشر می‌شود.</p>
     <span class="news-time">WORLD EVENTS</span>
    </div>
   </article>

   <article class="news-card" data-category="فناوری">
    <div class="news-image">💻</div>
    <div class="news-body">
     <span class="news-category">فناوری</span>
     <h3>تازه‌های دنیای فناوری و تکنولوژی</h3>
     <p>با جدیدترین دستاوردهای فناوری و نوآوری‌های علمی آشنا شوید.</p>
     <span class="news-time">WORLD EVENTS</span>
    </div>
   </article>

   <article class="news-card" data-category="اقتصاد">
    <div class="news-image">📊</div>
    <div class="news-body">
     <span class="news-category">اقتصاد</span>
     <h3>نگاهی به تحولات اقتصادی جهان</h3>
     <p>گزارش‌ها و تحلیل‌های اقتصادی در این بخش قرار می‌گیرند.</p>
     <span class="news-time">WORLD EVENTS</span>
    </div>
   </article>

   <article class="news-card" data-category="علم">
    <div class="news-image">🔬</div>
    <div class="news-body">
     <span class="news-category">علم و دانش</span>
     <h3>تازه‌ترین اخبار علمی</h3>
     <p>دستاوردهای علمی و پژوهش‌های جدید را دنبال کنید.</p>
     <span class="news-time">WORLD EVENTS</span>
    </div>
   </article>

   <article class="news-card" data-category="ورزش">
    <div class="news-image">⚽</div>
    <div class="news-body">
     <span class="news-category">ورزش</span>
     <h3>آخرین رویدادهای ورزشی</h3>
     <p>خبرها و اتفاقات دنیای ورزش در این قسمت منتشر می‌شوند.</p>
     <span class="news-time">WORLD EVENTS</span>
    </div>
   </article>

   <article class="news-card" data-category="سیاست">
    <div class="news-image">🏛️</div>
    <div class="news-body">
     <span class="news-category">سیاست و دیپلماسی</span>
     <h3>تحولات سیاسی و روابط بین‌الملل</h3>
     <p>رویدادهای سیاسی و دیپلماتیک جهان را دنبال کنید.</p>
     <span class="news-time">WORLD EVENTS</span>
    </div>
   </article>

  </div>
  <div class="empty" id="empty">خبری با این عبارت پیدا نشد.</div>
 </section>

 <section class="section" id="categories">
  <div class="section-title">
   <h2>دسته‌بندی اخبار</h2>
  </div>
  <div class="category-grid">
   <a class="category" href="#latest"><span>🌍</span>اخبار جهان</a>
   <a class="category" href="#latest"><span>📊</span>اقتصاد</a>
   <a class="category" href="#latest"><span>🔬</span>علم و دانش</a>
   <a class="category" href="#latest"><span>⚽</span>ورزش</a>
   <a class="category" href="#latest"><span>💻</span>فناوری</a>
   <a class="category" href="#latest"><span>🏛️</span>سیاست و دیپلماسی</a>
   <a class="category" href="#latest"><span>🗞️</span>روزنامه و مطبوعات</a>
   <a class="category" href="#latest"><span>⚡</span>اخبار فوری</a>
   <a class="category" href="#latest"><span>🗂️</span>آرشیو خبر</a>
   <a class="category" href="#latest"><span>📰</span>آخرین اخبار</a>
  </div>
 </section>

 <section class="join">
  <div>
   <h2>همراه WORLD EVENTS باشید</h2>
   <p>برای دنبال‌کردن تازه‌ترین اخبار به کانال رسمی ما بپیوندید.</p>
  </div>
  <a href="https://ble.ir/WORLDEVENTS">📢 ورود به کانال رسمی</a>
 </section>

</main>

<footer id="about">
 <div class="container">
  <div class="footer-grid">
   <div>
    <h3>🌍 WORLD EVENTS</h3>
    <p>
     رویدادهای جهان؛ پنجره‌ای به تازه‌ترین اخبار،
     تحولات بین‌المللی و اتفاقات مهم جهان.
    </p>
   </div>
   <div>
    <h3>دسترسی سریع</h3>
    <div class="footer-links">
     <a href="#latest">آخرین اخبار</a>
     <a href="#categories">دسته‌بندی‌ها</a>
     <a href="#about">درباره ما</a>
    </div>
   </div>
   <div>
    <h3>ارتباط با ما</h3>
    <div class="footer-links">
     <a href="https://ble.ir/WORLDEVENTS">کانال رسمی</a>
     <a href="https://ble.ir/WORLDEVENTSCHAT">گروه گفت‌وگو</a>
     <a href="https://ble.ir/MohammadMahdi2037">پشتیبانی</a>
    </div>
   </div>
  </div>
  <div class="copyright">
   © WORLD EVENTS - All Rights Reserved
  </div>
 </div>
</footer>

<script>
function toggleMenu(){
 document.getElementById('navigation').classList.toggle('open');
}

function searchNews(){
 const q=document.getElementById('search').value.trim().toLowerCase();
 const cards=document.querySelectorAll('.news-card');
 let count=0;

 cards.forEach(card=>{
  const match=card.innerText.toLowerCase().includes(q);
  card.style.display=match?'':'none';
  if(match)count++;
 });

 document.getElementById('empty').style.display=
  count===0?'block':'none';
}
</script>

</body>
</html>
