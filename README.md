
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<meta name="theme-color" content="#0b1726">
<title>WORLD EVENTS | رویدادهای جهان</title>

<style>
:root{
 --navy:#0b1726;
 --navy2:#142b45;
 --blue:#1686df;
 --pale:#eaf3fc;
 --white:#fff;
 --text:#172b42;
 --muted:#78899c;
}

*{box-sizing:border-box}

body{
 margin:0;
 background:#f3f6fa;
 color:var(--text);
 font-family:Tahoma,Arial,sans-serif;
}

a{text-decoration:none;color:inherit}
button,input{font:inherit}
.container{width:min(1160px,94%);margin:auto}

/* TOP HEADER */

.topbar{
 background:#071321;
 color:#b9cbe0;
 font-size:11px;
 padding:9px 0;
}

.topbar .container{
 display:flex;
 justify-content:space-between;
 gap:10px;
}

.topbar a:hover{color:white}

header{
 background:linear-gradient(110deg,#0b1726,#173a5b);
 color:white;
 padding:19px 0;
}

.header{
 display:flex;
 align-items:center;
 justify-content:space-between;
 gap:15px;
}

.brand{
 display:flex;
 align-items:center;
 gap:13px;
}

.logo{
 width:54px;
 height:54px;
 border-radius:15px;
 background:linear-gradient(145deg,#168fe8,#07508e);
 display:grid;
 place-items:center;
 font-size:29px;
 box-shadow:0 5px 20px #1686df40;
}

.brand h1{
 font-size:21px;
 letter-spacing:1px;
 margin:0;
}

.brand p{
 font-size:11px;
 color:#b8d0e9;
 margin:7px 0 0;
}

.header-actions{
 display:flex;
 gap:9px;
}

.header-actions a{
 border:1px solid #66809c66;
 border-radius:8px;
 padding:10px 13px;
 font-size:11px;
}

.header-actions a:hover{
 background:#ffffff18;
}

/* NAV */

nav{
 background:#10243a;
 color:#fff;
}

.nav{
 display:flex;
 align-items:center;
 gap:25px;
 overflow-x:auto;
 white-space:nowrap;
}

.nav a{
 font-size:12px;
 padding:15px 0;
 border-bottom:2px solid transparent;
}

.nav a:hover{
 color:#62baff;
 border-color:#1686df;
}

.menu-btn{
 display:none;
 background:transparent;
 color:white;
 border:1px solid #71869b;
 border-radius:8px;
 padding:8px 12px;
 font-size:19px;
}

/* BREAKING */

.breaking{
 margin:20px auto 0;
 display:flex;
 align-items:center;
 background:white;
 border:1px solid #e3eaf1;
 border-radius:10px;
 overflow:hidden;
}

.breaking-label{
 background:#087acb;
 color:white;
 padding:14px 17px;
 font-size:12px;
 font-weight:bold;
 white-space:nowrap;
}

.breaking-content{
 padding:12px 16px;
 font-size:12px;
 color:#42566b;
 overflow:hidden;
 white-space:nowrap;
}

/* TELEGRAM STYLE SEARCH */

.search{
 margin:17px 0;
 display:flex;
 align-items:center;
 gap:10px;
 background:white;
 border:1px solid #dce5ef;
 border-radius:30px;
 padding:0 17px;
 height:49px;
 transition:.2s;
 box-shadow:0 2px 8px #0b172608;
}

.search:focus-within{
 border-color:var(--blue);
 box-shadow:0 0 0 3px #1686df18;
}

.search-icon{
 width:20px;
 height:20px;
 flex-shrink:0;
 color:#8b9bad;
 display:flex;
 align-items:center;
 justify-content:center;
}

.search-icon svg{
 width:19px;
 height:19px;
 stroke:currentColor;
}

.search input{
 flex:1;
 min-width:0;
 border:0;
 outline:none;
 background:transparent;
 padding:12px 0;
 font-size:13px;
 color:#172b42;
}

.search input::placeholder{
 color:#8b9bad;
}

/* Hide default browser search clear button */

.search input::-webkit-search-cancel-button{
 -webkit-appearance:none;
 appearance:none;
}

.search button{
 display:none;
 border:0;
 background:transparent;
 color:#8294a7;
 font-size:23px;
 cursor:pointer;
 padding:3px;
 width:30px;
 height:30px;
 border-radius:50%;
 align-items:center;
 justify-content:center;
}

.search button.show{
 display:flex;
}

.search button:hover{
 background:#edf3f8;
 color:#1686df;
}

/* HERO */

.hero{
 display:grid;
 grid-template-columns:1.7fr 1fr;
 gap:16px;
 margin-top:18px;
}

.hero-main{
 min-height:350px;
 position:relative;
 overflow:hidden;
 border-radius:15px;
 background:
 linear-gradient(0deg,#071321f5 0%,#07132135 85%),
 url("https://images.unsplash.com/photo-1451187580459-43490279c0fa?w=1200") center/cover;
 display:flex;
 align-items:end;
 color:white;
}

.hero-content{
 padding:28px;
 position:relative;
 z-index:1;
}

.tag{
 display:inline-block;
 background:#1686df;
 color:white;
 padding:7px 12px;
 border-radius:5px;
 font-size:10px;
}

.hero h2{
 font-size:25px;
 line-height:1.9;
 margin:15px 0 8px;
}

.hero p{
 font-size:12px;
 color:#d1deeb;
 line-height:2;
}

.read{
 display:inline-block;
 margin-top:8px;
 background:#1686df;
 padding:10px 15px;
 border-radius:7px;
 font-size:11px;
}

.hero-side{
 display:grid;
 gap:15px;
}

.side-card{
 min-height:167px;
 border-radius:14px;
 color:white;
 display:flex;
 align-items:end;
 padding:19px;
 background:
 linear-gradient(0deg,#071321eF,transparent),
 url("https://images.unsplash.com/photo-1526304640581-d334cdbbf45e?w=800") center/cover;
}

.side-card:nth-child(2){
 background:
 linear-gradient(0deg,#071321ed,transparent),
 url("https://images.unsplash.com/photo-1518770660439-4636190af475?w=800") center/cover;
}

.side-card h3{
 font-size:14px;
 line-height:1.9;
 margin:9px 0 0;
}

/* SECTION */

.section{
 margin-top:35px;
}

.section-head{
 display:flex;
 align-items:center;
 justify-content:space-between;
 margin-bottom:17px;
}

.section-head h2{
 font-size:18px;
 margin:0;
 border-right:4px solid var(--blue);
 padding-right:12px;
}

.section-head a{
 font-size:11px;
 color:#167dca;
}

/* NEWS */

.news-grid{
 display:grid;
 grid-template-columns:repeat(3,1fr);
 gap:17px;
}

.news-card{
 background:white;
 border:1px solid #e4eaf0;
 border-radius:12px;
 overflow:hidden;
 transition:.2s;
}

.news-card:hover{
 transform:translateY(-4px);
 box-shadow:0 9px 25px #17334d15;
}

.news-img{
 height:180px;
 overflow:hidden;
 background:#dce8f4;
}

.news-img img{
 width:100%;
 height:100%;
 object-fit:cover;
 transition:.3s;
}

.news-card:hover .news-img img{
 transform:scale(1.04);
}

.news-info{
 padding:15px;
}

.news-cat{
 font-size:10px;
 color:#1686df;
 font-weight:bold;
}

.news-info h3{
 font-size:14px;
 line-height:1.9;
 margin:10px 0;
}

.news-info p{
 font-size:11px;
 line-height:2;
 color:var(--muted);
 margin:0 0 14px;
}

.news-meta{
 border-top:1px solid #edf1f5;
 padding-top:11px;
 color:#9aa8b7;
 font-size:10px;
}

.empty{
 display:none;
 padding:25px;
 text-align:center;
 color:var(--muted);
 font-size:13px;
}

/* CATEGORIES */

.categories{
 display:grid;
 grid-template-columns:repeat(5,1fr);
 gap:12px;
}

.category{
 background:white;
 border:1px solid #e3eaf1;
 border-radius:11px;
 padding:17px 8px;
 text-align:center;
 font-size:11px;
 transition:.2s;
}

.category:hover{
 border-color:var(--blue);
 background:#eaf5ff;
 color:#087acb;
}

.category span{
 display:block;
 font-size:25px;
 margin-bottom:10px;
}

/* CHANNEL */

.channel{
 margin:40px 0;
 background:linear-gradient(110deg,#0b1726,#164e7c);
 color:white;
 border-radius:15px;
 padding:27px;
 display:flex;
 align-items:center;
 justify-content:space-between;
 gap:15px;
}

.channel h2{
 font-size:18px;
 margin:0 0 10px;
}

.channel p{
 font-size:11px;
 color:#c5d8ea;
 line-height:2;
}

.channel a{
 background:#1686df;
 padding:12px 17px;
 border-radius:8px;
 font-size:12px;
 white-space:nowrap;
}

/* FOOTER */

footer{
 background:#091522;
 color:white;
 padding:35px 0 17px;
}

.footer-grid{
 display:grid;
 grid-template-columns:2fr 1fr 1fr;
 gap:25px;
}

footer h3{
 font-size:14px;
 color:#55b2ff;
}

footer p,footer a{
 font-size:11px;
 color:#afc0d2;
 line-height:2.4;
}

.footer-links{
 display:flex;
 flex-direction:column;
}

.copyright{
 border-top:1px solid #ffffff1b;
 text-align:center;
 padding-top:17px;
 margin-top:25px;
 color:#8094a8;
 font-size:10px;
}

/* MOBILE */

@media(max-width:700px){

 .topbar .container{
  font-size:9px;
 }

 .header{
  flex-wrap:wrap;
 }

 .brand h1{
  font-size:17px;
 }

 .logo{
  width:47px;
  height:47px;
 }

 .header-actions{
  display:none;
 }

 .menu-btn{
  display:block;
 }

 nav{
  display:none;
 }

 nav.open{
  display:block;
 }

 .nav{
  display:flex;
  flex-direction:column;
  align-items:stretch;
  gap:0;
 }

 .nav a{
  padding:13px 4px;
  border-bottom:1px solid #ffffff16;
 }

 .hero{
  grid-template-columns:1fr;
 }

 .hero-main{
  min-height:300px;
 }

 .hero h2{
  font-size:21px;
 }

 .hero-side{
  grid-template-columns:1fr 1fr;
 }

 .side-card{
  min-height:140px;
  padding:13px;
 }

 .side-card h3{
  font-size:12px;
 }

 .news-grid{
  grid-template-columns:1fr 1fr;
  gap:10px;
 }

 .news-img{
  height:125px;
 }

 .news-info{
  padding:10px;
 }

 .news-info h3{
  font-size:12px;
 }

 .news-info p{
  font-size:10px;
 }

 .categories{
  grid-template-columns:repeat(3,1fr);
  gap:8px;
 }

 .category{
  font-size:10px;
  padding:13px 4px;
 }

 .channel{
  flex-direction:column;
  align-items:flex-start;
 }

 .footer-grid{
  grid-template-columns:1fr 1fr;
 }

 .footer-grid>div:first-child{
  grid-column:1/-1;
 }

}

@media(max-width:380px){

 .news-grid{
  grid-template-columns:1fr;
 }

 .hero-side{
  grid-template-columns:1fr;
 }

}
</style>
</head>

<body>

<div class="topbar">
 <div class="container">
  <span>🌍 رسانه خبری رویدادهای جهان</span>
  <span>WORLD EVENTS | اخبار جهان</span>
 </div>
</div>

<header>
 <div class="container header">

  <div class="brand">
   <div class="logo">🌍</div>

   <div>
    <h1>WORLD EVENTS</h1>
    <p>رویدادهای جهان | از جهان باخبر باشید</p>
   </div>
  </div>

  <div class="header-actions">
   <a href="https://ble.ir/WORLDEVENTS">کانال رسمی</a>
   <a href="https://ble.ir/WORLDEVENTSCHAT">گروه گفت‌وگو</a>
  </div>

  <button class="menu-btn" onclick="toggleMenu()">☰</button>

 </div>
</header>

<nav id="nav">
 <div class="container nav">
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

 <!-- BREAKING NEWS -->

 <div class="breaking">
  <div class="breaking-label">⚡ اخبار فوری</div>

  <div class="breaking-content" id="breakingText">
   آخرین رویدادهای مهم جهان را در WORLD EVENTS دنبال کنید.
  </div>
 </div>

 <!-- TELEGRAM SEARCH -->

 <div class="search">

  <span class="search-icon">
   <svg viewBox="0 0 24 24" fill="none"
    stroke-width="2" stroke-linecap="round">
    <circle cx="11" cy="11" r="7"></circle>
    <path d="m20 20-4-4"></path>
   </svg>
  </span>

  <input
   id="search"
   type="search"
   placeholder="جستجو در اخبار..."
   autocomplete="off"
   oninput="searchNews();toggleClearButton()"
  >

  <button
   id="clearSearch"
   type="button"
   onclick="clearSearch()"
   aria-label="پاک کردن جستجو"
  >×</button>

 </div>

 <!-- HERO -->

 <section class="hero">

  <div class="hero-main">
   <div class="hero-content">

    <span class="tag">رسانه خبری WORLD EVENTS</span>

    <h2>پنجره‌ای به تازه‌ترین رویدادهای جهان</h2>

    <p>
     تازه‌ترین اخبار، تحولات بین‌المللی و رویدادهای مهم جهان را دنبال کنید.
    </p>

    <a class="read" href="#latest">
     مشاهده آخرین اخبار ←
    </a>

   </div>
  </div>

  <div class="hero-side">

   <div class="side-card">
    <div>
     <span class="tag">اخبار جهان</span>
     <h3>تحولات و رویدادهای بین‌المللی</h3>
    </div>
   </div>

   <div class="side-card">
    <div>
     <span class="tag">فناوری</span>
     <h3>نگاهی به دنیای علم و فناوری</h3>
    </div>
   </div>

  </div>

 </section>

 <!-- LATEST NEWS -->

 <section class="section" id="latest">

  <div class="section-head">
   <h2>آخرین اخبار</h2>
   <a href="#latest">مشاهده همه ←</a>
  </div>

  <div class="news-grid" id="newsGrid">

   <article class="news-card">
    <div class="news-img">
     <img src="https://images.unsplash.com/photo-1529107386315-e1a2ed48a620?w=700" alt="اخبار جهان">
    </div>

    <div class="news-info">
     <span class="news-cat">اخبار جهان</span>
     <h3>تحولات و رویدادهای بین‌المللی</h3>
     <p>آخرین اتفاقات و تحولات مهم جهان را در این بخش دنبال کنید.</p>
     <div class="news-meta">WORLD EVENTS</div>
    </div>
   </article>

   <article class="news-card">
    <div class="news-img">
     <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?w=700" alt="اقتصاد">
    </div>

    <div class="news-info">
     <span class="news-cat">اقتصاد</span>
     <h3>تحولات اقتصادی و بازارهای جهانی</h3>
     <p>گزارش‌ها و رویدادهای مهم اقتصادی را دنبال کنید.</p>
     <div class="news-meta">WORLD EVENTS</div>
    </div>
   </article>

   <article class="news-card">
    <div class="news-img">
     <img src="https://images.unsplash.com/photo-1518770660439-4636190af475?w=700" alt="فناوری">
    </div>

    <div class="news-info">
     <span class="news-cat">فناوری</span>
     <h3>تازه‌های دنیای فناوری</h3>
     <p>با فناوری‌های جدید و نوآوری‌های علمی آشنا شوید.</p>
     <div class="news-meta">WORLD EVENTS</div>
    </div>
   </article>

   <article class="news-card">
    <div class="news-img">
     <img src="https://images.unsplash.com/photo-1532094349884-543bc11b234d?w=700" alt="علم">
    </div>

    <div class="news-info">
     <span class="news-cat">علم و دانش</span>
     <h3>دستاوردهای علمی و پژوهشی</h3>
     <p>تازه‌ترین اخبار علمی و پژوهش‌های جدید جهان.</p>
     <div class="news-meta">WORLD EVENTS</div>
    </div>
   </article>

   <article class="news-card">
    <div class="news-img">
     <img src="https://images.unsplash.com/photo-1461896836934-ffe607ba8211?w=700" alt="ورزش">
    </div>

    <div class="news-info">
     <span class="news-cat">ورزش</span>
     <h3>رویدادهای مهم ورزشی</h3>
     <p>خبرها و اتفاقات دنیای ورزش را دنبال کنید.</p>
     <div class="news-meta">WORLD EVENTS</div>
    </div>
   </article>

   <article class="news-card">
    <div class="news-img">
     <img src="https://images.unsplash.com/photo-1497366754035-f200968a6e72?w=700" alt="سیاست">
    </div>

    <div class="news-info">
     <span class="news-cat">سیاست و دیپلماسی</span>
     <h3>روابط بین‌الملل و تحولات سیاسی</h3>
     <p>گزارش رویدادهای سیاسی و دیپلماتیک جهان.</p>
     <div class="news-meta">WORLD EVENTS</div>
    </div>
   </article>

  </div>

  <div class="empty" id="empty">
   خبری پیدا نشد.
  </div>

 </section>

 <!-- CATEGORIES -->

 <section class="section" id="categories">

  <div class="section-head">
   <h2>دسته‌بندی اخبار</h2>
  </div>

  <div class="categories">

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

 <!-- CHANNEL -->

 <section class="channel">

  <div>
   <h2>همراه WORLD EVENTS باشید</h2>
   <p>برای دنبال‌کردن تازه‌ترین اخبار به کانال رسمی ما بپیوندید.</p>
  </div>

  <a href="https://ble.ir/WORLDEVENTS">
   📢 عضویت در کانال رسمی
  </a>

 </section>

</main>

<!-- FOOTER -->

<footer id="about">

 <div class="container">

  <div class="footer-grid">

   <div>
    <h3>🌍 WORLD EVENTS</h3>
    <p>
     رویدادهای جهان؛ پنجره‌ای به تازه‌ترین اخبار و تحولات بین‌المللی.
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

/* MOBILE MENU */

function toggleMenu(){
 document.getElementById('nav').classList.toggle('open');
}

/* SEARCH NEWS */

function searchNews(){

 const input=document.getElementById('search');
 const query=input.value.trim().toLowerCase();

 const cards=document.querySelectorAll('.news-card');

 let found=0;

 cards.forEach(card=>{

  const text=card.innerText.toLowerCase();
  const match=text.includes(query);

  card.style.display=match?'':'none';

  if(match){
   found++;
  }

 });

 document.getElementById('empty').style.display=
  found===0?'block':'none';

}

/* SHOW / HIDE CLEAR BUTTON */

function toggleClearButton(){

 const input=document.getElementById('search');
 const clear=document.getElementById('clearSearch');

 clear.classList.toggle('show',input.value.length>0);

}

/* CLEAR SEARCH */

function clearSearch(){

 const input=document.getElementById('search');

 input.value='';

 searchNews();
 toggleClearButton();

 input.focus();

}

/* ENTER KEY */

document.getElementById('search').addEventListener('keydown',function(event){

 if(event.key==='Enter'){
  searchNews();
  this.blur();
 }

});

</script>

</body>
</html>
