<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>착한언니복덕방 | 신촌·이대 부동산</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300;400;500;700&family=Noto+Serif+KR:wght@400;700&display=swap" rel="stylesheet">
<style>
*{box-sizing:border-box;margin:0;padding:0}
:root{--pink:#E8185A;--pink-soft:#FFF0F5;--pink-mid:#FFD6E5;--text:#1a1a1a;--muted:#888}
body{font-family:'Noto Sans KR',sans-serif;background:#fff;color:var(--text)}
.header{background:white;border-bottom:.5px solid #f0e0e8;padding:0 1.5rem;height:52px;display:flex;align-items:center;justify-content:space-between;position:sticky;top:0;z-index:10}
.logo{font-size:15px;font-weight:700;color:var(--pink)}
.lang-toggle{display:flex;background:var(--pink);border-radius:20px;overflow:hidden}
.lang-toggle button{padding:5px 14px;border:none;background:transparent;cursor:pointer;font-size:11px;font-weight:600;font-family:'Noto Sans KR',sans-serif;color:rgba(255,255,255,0.6)}
.lang-toggle button.active{background:white;color:var(--pink);border-radius:20px;margin:2px}
.hero{background:linear-gradient(160deg,#FFF0F5 0%,#FFE4EE 40%,#FFF8FB 100%);padding:72px 24px 56px;text-align:center}
.hero-tag{display:inline-block;background:white;color:var(--pink);padding:5px 16px;border-radius:20px;font-size:12px;font-weight:500;border:1px solid var(--pink-mid);margin-bottom:20px}
.hero h1{font-family:'Noto Serif KR',serif;font-size:clamp(26px,6vw,44px);font-weight:700;line-height:1.3;margin-bottom:8px}
.hero h1 em{color:var(--pink);font-style:normal}
.hero p{font-size:14px;color:#666;line-height:1.8;max-width:400px;margin:0 auto 28px}
.hero-btns{display:flex;gap:10px;justify-content:center;flex-wrap:wrap}
.btn-pink{padding:12px 24px;border-radius:10px;border:none;background:var(--pink);color:white;font-weight:600;font-size:13px;font-family:'Noto Sans KR',sans-serif;text-decoration:none;display:inline-flex;align-items:center;gap:6px}
.btn-ghost{padding:12px 24px;border-radius:10px;border:1.5px solid var(--pink);color:var(--pink);font-weight:500;font-size:13px;background:white;text-decoration:none;display:inline-flex;align-items:center;gap:6px}
section{padding:52px 24px}
.container{max-width:800px;margin:0 auto}
.sec-title{font-family:'Noto Serif KR',serif;font-size:clamp(20px,3.5vw,28px);font-weight:700;text-align:center;margin-bottom:8px}
.sec-sub{text-align:center;color:var(--muted);font-size:13px;margin-bottom:32px}
.sec-title em{color:var(--pink);font-style:normal}
.highlight-box{background:var(--pink);border-radius:18px;padding:32px 24px;text-align:center;max-width:560px;margin:0 auto}
.highlight-box h2{font-size:clamp(17px,3vw,23px);font-weight:700;color:white;line-height:1.6;margin-bottom:6px}
.highlight-box h2 strong{background:rgba(255,255,255,0.2);padding:2px 10px;border-radius:6px}
.highlight-box p{font-size:12px;color:rgba(255,255,255,0.75);margin-top:8px}
.feat-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(170px,1fr));gap:12px}
.feat-card{background:white;border-radius:14px;padding:22px 16px;text-align:center;border:.5px solid #f5e0e8}
.feat-icon{font-size:28px;margin-bottom:10px}
.feat-card h3{font-size:14px;font-weight:600;margin-bottom:6px}
.feat-card p{font-size:12px;color:var(--muted);line-height:1.6}
.team-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(150px,1fr));gap:12px}
.team-card{border-radius:14px;padding:22px 14px;text-align:center;border:.5px solid #f5e0e8;background:white}
.avatar{width:68px;height:68px;border-radius:50%;background:linear-gradient(135deg,var(--pink),#ff6b9d);color:white;display:flex;align-items:center;justify-content:center;font-size:18px;font-weight:700;margin:0 auto 10px}
.team-card h3{font-size:14px;font-weight:600;margin-bottom:3px}
.team-card p{font-size:11px;color:var(--muted)}
.offices-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:16px}
.office-card{background:white;border-radius:14px;padding:22px;border:.5px solid #f5e0e8;border-top:3px solid var(--pink)}
.office-card h3{font-size:15px;font-weight:600;margin-bottom:14px;color:var(--pink)}
.oinfo{display:flex;flex-direction:column;gap:8px}
.orow{display:flex;gap:8px;font-size:12px;align-items:flex-start;color:#444}
.orow .oi{color:var(--pink);flex-shrink:0}
.call-btn{display:inline-flex;align-items:center;gap:6px;background:var(--pink);color:white;padding:9px 18px;border-radius:8px;font-size:13px;font-weight:700;text-decoration:none;margin-top:14px}
.links-row{display:flex;gap:12px;justify-content:center;flex-wrap:wrap}
.link-card{display:flex;align-items:center;gap:10px;padding:14px 24px;border-radius:12px;text-decoration:none;font-weight:600;font-size:14px;min-width:200px;justify-content:center}
.link-blog{background:#03C75A;color:white}
.link-yt{background:#FF0000;color:white}
.footer{background:#1a1a1a;color:rgba(255,255,255,0.5);padding:32px 24px;text-align:center;font-size:11px;line-height:2.2}
.footer strong{color:rgba(255,255,255,0.85)}
.en{display:none}
@media(max-width:480px){.hero{padding:64px 16px 48px}section{padding:40px 16px}.offices-grid{grid-template-columns:1fr}}
</style>
</head>
<body>
<header class="header">
  <div class="logo">착한언니복덕방</div>
  <div class="lang-toggle">
    <button class="active" onclick="setLang('ko')">KO</button>
    <button onclick="setLang('en')">EN</button>
  </div>
</header>
<div class="hero">
  <div class="hero-tag ko">신촌 · 이대 상권 전문 부동산</div>
  <div class="hero-tag en">Sinchon &amp; Ewha Real Estate Specialists</div>
  <h1 class="ko">당신의 공간을<br><em>찾아드립니다</em></h1>
  <h1 class="en">We Find<br><em>Your Perfect Space</em></h1>
  <p class="ko">신촌과 이대 상권을 누벼온<br>착한언니복덕방이 함께합니다</p>
  <p class="en">Kind Sister Realtors — your trusted partner<br>in Sinchon &amp; Ewha</p>
  <div class="hero-btns">
    <a href="tel:0236344080" class="btn-pink">📞 <span class="ko">전화 상담</span><span class="en">Call Now</span></a>
    <a href="https://blog.naver.com/ellarang" target="_blank" class="btn-ghost">N <span class="ko">블로그</span><span class="en">Blog</span></a>
    <a href="https://www.youtube.com/@착한언니복덕방" target="_blank" class="btn-ghost">▶ <span class="ko">유튜브</span><span class="en">YouTube</span></a>
  </div>
</div>
<section style="background:#fff5f8;padding:44px 24px">
  <div class="container">
    <div class="highlight-box">
      <h2 class="ko">착한언니복덕방에는<br><strong>"중개보조원"이 없습니다!</strong></h2>
      <h2 class="en">No unlicensed assistants.<br><strong>Only certified professionals.</strong></h2>
      <p class="ko">모든 중개업무는 자격증을 보유한 국가공인중개사가 직접 진행합니다</p>
      <p class="en">Every transaction is handled by nationally certified real estate agents</p>
    </div>
  </div>
</section>
<section style="background:white">
  <div class="container">
    <h2 class="sec-title ko">왜 <em>착한언니복덕방</em>인가요?</h2>
    <h2 class="sec-title en">Why <em>Kind Sister</em> Realtors?</h2>
    <p class="sec-sub ko">신촌·이대 지역 전문가가 직접 도와드립니다</p>
    <p class="sec-sub en">Local experts who know every corner of Sinchon &amp; Ewha</p>
    <div class="feat-grid">
      <div class="feat-card"><div class="feat-icon">🏆</div><h3 class="ko">전문성</h3><h3 class="en">Expertise</h3><p class="ko">신촌·이대 상권 오피스텔·상가 전문</p><p class="en">Specialists in local commercial &amp; residential</p></div>
      <div class="feat-card"><div class="feat-icon">🤝</div><h3 class="ko">신뢰</h3><h3 class="en">Trust</h3><p class="ko">공인중개사가 처음부터 끝까지</p><p class="en">Certified agents, start to finish</p></div>
      <div class="feat-card"><div class="feat-icon">🌍</div><h3 class="ko">외국인 환영</h3><h3 class="en">Foreigner Friendly</h3><p class="ko">외국인 고객 상담 가능합니다</p><p class="en">Bilingual support available</p></div>
      <div class="feat-card"><div class="feat-icon">🅿️</div><h3 class="ko">무료 주차</h3><h3 class="en">Free Parking</h3><p class="ko">내방 고객 무료 주차 제공</p><p class="en">Complimentary parking for visitors</p></div>
    </div>
  </div>
</section>
<section style="background:#fff5f8">
  <div class="container">
    <h2 class="sec-title ko">공인중개사 소개</h2>
    <h2 class="sec-title en">Our Licensed Agents</h2>
    <p class="sec-sub ko">모든 직원이 국가공인중개사 자격증 보유</p>
    <p class="sec-sub en">All staff hold national real estate certifications</p>
    <div class="team-grid">
      <div class="team-card"><div class="avatar">신혜</div><h3>신혜선</h3><p class="ko">공인중개사</p><p class="en">Certified Agent</p></div>
      <div class="team-card"><div class="avatar">신수</div><h3>신수진</h3><p class="ko">공인중개사</p><p class="en">Certified Agent</p></div>
      <div class="team-card"><div class="avatar">신경</div><h3>신수경</h3><p class="ko">공인중개사</p><p class="en">Certified Agent</p></div>
      <div class="team-card"><div class="avatar">윤미</div><h3>윤미현</h3><p class="ko">공인중개사</p><p class="en">Certified Agent</p></div>
    </div>
  </div>
</section>
<section style="background:white">
  <div class="container">
    <h2 class="sec-title ko">오시는 길</h2>
    <h2 class="sec-title en">Find Us</h2>
    <p class="sec-sub ko">두 곳 모두 이대역 근처에 있어요</p>
    <p class="sec-sub en">Both offices are near Ewha Station (Line 2)</p>
    <div class="offices-grid">
      <div class="office-card">
        <h3 class="ko">신촌자이엘라 부동산</h3>
        <h3 class="en">Sinchon Xi Ella Office</h3>
        <div class="oinfo">
          <div class="orow"><span class="oi">📍</span><span class="ko">서울 서대문구 대현동 104-36, B101호 (신촌자이엘라)</span><span class="en">104-36 Daehyeon-dong, Seodaemun-gu, B101</span></div>
          <div class="orow"><span class="oi">🚇</span><span class="ko">이대역 1번출구 도보 3분</span><span class="en">3 min walk from Ewha Station, Exit 1</span></div>
          <div class="orow"><span class="oi">🅿️</span><span class="ko">무료주차 — 경비 호출 후 방문 등록</span><span class="en">Free parking — call security on arrival</span></div>
        </div>
        <a href="tel:0236344080" class="call-btn">📞 02-364-4080</a>
      </div>
      <div class="office-card">
        <h3 class="ko">마포그랑자이 부동산</h3>
        <h3 class="en">Mapo Granj Xi Office</h3>
        <div class="oinfo">
          <div class="orow"><span class="oi">📍</span><span class="ko">서울 마포구 대흥로 175 마포그랑자이 상가4동 104호</span><span class="en">175 Daeheung-ro, Mapo-gu, Granj Xi 4-104</span></div>
          <div class="orow"><span class="oi">🚇</span><span class="ko">이대역 6번출구 도보 5분</span><span class="en">5 min walk from Ewha Station, Exit 6</span></div>
          <div class="orow"><span class="oi">🅿️</span><span class="ko">무료주차 — 게이트1 정문 주차장</span><span class="en">Free parking — Gate 1 entrance</span></div>
        </div>
        <a href="tel:0270733434" class="call-btn">📞 02-707-3434</a>
      </div>
    </div>
  </div>
</section>
<section style="background:#fff5f8">
  <div class="container">
    <h2 class="sec-title ko">블로그 &amp; 유튜브</h2>
    <h2 class="sec-title en">Blog &amp; YouTube</h2>
    <p class="sec-sub ko">부동산 정보와 유용한 콘텐츠를 확인하세요</p>
    <p class="sec-sub en">Real estate tips and helpful content</p>
    <div class="links-row">
      <a href="https://blog.naver.com/ellarang" target="_blank" class="link-card link-blog">
        <span style="font-size:20px;font-weight:900">N</span>
        <span class="ko">착한언니복덕방 블로그</span><span class="en">Naver Blog</span>
      </a>
      <a href="https://www.youtube.com/@착한언니복덕방" target="_blank" class="link-card link-yt">
        <span style="font-size:18px">▶</span>
        <span class="ko">착한언니복덕방 유튜브</span><span class="en">YouTube Channel</span>
      </a>
    </div>
  </div>
</section>
<footer class="footer">
  <strong class="ko">착한언니복덕방 | 신촌자이엘라부동산공인중개사사무소</strong>
  <strong class="en">Kind Sister Realtors | Licensed Real Estate Agency</strong><br>
  <span class="ko">대표: 신수경 &nbsp;|&nbsp; 사업자번호: 204-29-31241 &nbsp;|&nbsp; 중개등록번호: 11410-2019-00062</span>
  <span class="en">CEO: Shin Sukyung &nbsp;|&nbsp; Reg: 204-29-31241 &nbsp;|&nbsp; License: 11410-2019-00062</span><br>
  <span>© 2025 착한언니복덕방 · Kind Sister Realtors</span>
</footer>
<script>
function setLang(l){
  document.querySelectorAll('.ko').forEach(el=>el.style.display=l==='en'?'none':'');
  document.querySelectorAll('.en').forEach(el=>el.style.display=l==='en'?'':'none');
  document.querySelectorAll('.lang-toggle button').forEach((b,i)=>b.classList.toggle('active',(l==='ko'&&i===0)||(l==='en'&&i===1)));
}
</script>
</body>
</html>
