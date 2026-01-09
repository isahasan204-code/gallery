<meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Our Projects - Elite Home Services | London, ON</title>

  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700&amp;family=Inter:wght@300;400;500;600;700&amp;display=swap" rel="stylesheet">

  <style>
    *{margin:0;padding:0;box-sizing:border-box}
    :root{
      --background:#faf8f6;
      --foreground:#2d2520;
      --primary:#5D4037;
      --primary-foreground:#faf8f6;
      --accent:#c4784a;
      --muted:#6b5c52;
      --card:#f5f2ef;
      --border:#e8e2dc;
      --radius:16px;
      --shadow:0 14px 40px -14px rgba(45,37,32,0.18);
    }

    body{
      font-family:'Inter',sans-serif;
      background:var(--background);
      color:var(--foreground);
      line-height:1.6;
    }
    h1,h2,h3,h4{font-family:'Playfair Display',serif}
    a{color:inherit}
    .container{max-width:1100px;margin:0 auto;padding:0 16px}

    /* HEADER */
    .header{
      background:var(--primary);
      color:var(--primary-foreground);
      border-bottom:1px solid rgba(255,255,255,0.12);
    }
    .header-wrap{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:12px;
      padding:14px 0;
      flex-wrap:wrap;
    }
    .brand{display:flex;flex-direction:column;gap:2px;min-width:220px}
    .brand h1{font-size:18px;font-weight:700;letter-spacing:.2px;line-height:1.15}
    .brand p{font-size:12.5px;opacity:.85}

    .header-actions{
      display:flex;
      gap:10px;
      flex-wrap:wrap;
      justify-content:flex-end;
    }
    .pill{
      display:inline-flex;
      align-items:center;
      gap:8px;
      text-decoration:none;
      padding:10px 12px;
      border-radius:999px;
      border:1px solid rgba(255,255,255,0.18);
      background:rgba(255,255,255,0.08);
      font-size:13px;
      font-weight:600;
      transition:transform .15s ease, opacity .15s ease;
      white-space:nowrap;
    }
    .pill:hover{opacity:0.9;transform:translateY(-1px)}
    .pill strong{font-weight:700}

    /* HERO */
    .hero{
      position:relative;
      background:
        linear-gradient(to bottom, rgba(45,37,32,0.78), rgba(45,37,32,0.35)),
        url("https://i.pinimg.com/1200x/aa/fa/9e/aafa9ec10f25f76f5403ad4dcd8b3da6.jpg") center/cover no-repeat;
      color:var(--primary-foreground);
    }
    .hero .container{padding:34px 16px 28px}
    .hero-card{
      max-width:720px;
      background:rgba(0,0,0,0.15);
      border:1px solid rgba(255,255,255,0.14);
      border-radius:var(--radius);
      padding:18px;
      box-shadow:0 18px 50px -26px rgba(0,0,0,0.55);
      backdrop-filter: blur(8px);
    }
    .hero h2{font-size:28px;line-height:1.15;margin-bottom:10px;color:#fff}
    .hero p{font-size:15.5px;opacity:.92;margin-bottom:14px;max-width:60ch}
    .hero-cta{display:flex;gap:10px;flex-wrap:wrap;margin-bottom:14px}
    .btn{
      display:inline-flex;
      align-items:center;
      justify-content:center;
      gap:10px;
      padding:12px 16px;
      border-radius:999px;
      text-decoration:none;
      font-weight:700;
      font-size:14px;
      border:1px solid rgba(255,255,255,0.0);
      transition:transform .15s ease, opacity .15s ease;
      white-space:nowrap;
    }
    .btn:hover{transform:translateY(-1px);opacity:0.95}
    .btn-primary{
      background:var(--accent);
      color:#1f140f;
      border:1px solid rgba(255,255,255,0.12);
    }
    .btn-outline{
      background:rgba(255,255,255,0.10);
      color:var(--primary-foreground);
      border:1px solid rgba(255,255,255,0.18);
    }
    .badges{display:flex;flex-wrap:wrap;gap:8px}
    .badge{
      display:inline-flex;
      align-items:center;
      gap:8px;
      padding:8px 12px;
      border-radius:999px;
      background:rgba(255,255,255,0.10);
      border:1px solid rgba(255,255,255,0.16);
      font-size:12.5px;
      font-weight:600;
    }
    .dot{width:8px;height:8px;border-radius:50%;background:var(--accent)}

    /* GALLERY SECTION */
    .ehs-gallery{ 
      padding: 48px 16px; 
      background: var(--card);
      border-top: 1px solid var(--border);
    } 
    .ehs-gallery-wrap{ 
      max-width: 1100px; 
      margin: 0 auto; 
    } 
    .ehs-gallery h2{ 
      margin: 0 0 10px; 
      font-size: 30px;
      text-align: center;
      color: var(--foreground);
    } 
    .ehs-gallery-intro{ 
      margin: 0 0 32px; 
      font-size: 16px; 
      line-height: 1.7;
      text-align: center;
      color: var(--muted);
      max-width: 70ch;
      margin-left: auto;
      margin-right: auto;
    } 
    .ehs-gallery-grid{ 
      display: grid; 
      grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); 
      gap: 14px; 
    } 
    .ehs-thumb{ 
      width: 100%; 
      height: 220px; 
      object-fit: cover; 
      border-radius: 14px; 
      cursor: pointer; 
      border: 1px solid var(--border); 
      transition: transform .2s ease, box-shadow .2s ease; 
      box-shadow: 0 4px 12px rgba(45,37,32,0.1);
    } 
    .ehs-thumb:hover{ 
      transform: scale(1.03); 
      box-shadow: 0 8px 24px rgba(45,37,32,0.15);
    } 

    /* LIGHTBOX */
    .ehs-lightbox{ 
      position: fixed; 
      inset: 0; 
      background: rgba(0,0,0,.90); 
      display: none; 
      align-items: center; 
      justify-content: center; 
      z-index: 99999; 
      padding: 16px; 
    } 
    .ehs-lightbox.is-open{ display: flex; } 
    .ehs-lb-figure{ 
      display: flex;
      align-items: center;
      justify-content: center;
      max-width: 90vw;
      max-height: 90vh;
    }
    .ehs-lb-figure img{ 
      max-width: 100%; 
      max-height: 85vh; 
      border-radius: 16px; 
      box-shadow: 0 12px 40px rgba(0,0,0,.5); 
    } 
    .ehs-lb-close, .ehs-lb-arrow{ 
      position: absolute; 
      background: rgba(255,255,255,.15); 
      color: #fff; 
      border: 0; 
      cursor: pointer; 
      border-radius: 999px; 
      display: flex; 
      align-items: center; 
      justify-content: center;
      transition: background .2s ease;
    }
    .ehs-lb-close:hover, .ehs-lb-arrow:hover{
      background: rgba(255,255,255,.25);
    }
    .ehs-lb-close{ 
      top: 14px; 
      right: 14px; 
      width: 44px; 
      height: 44px; 
      font-size: 22px; 
    } 
    .ehs-lb-arrow{ 
      top: 50%; 
      transform: translateY(-50%); 
      width: 54px; 
      height: 54px; 
      font-size: 38px; 
    } 
    .ehs-lb-prev{ left: 14px; } 
    .ehs-lb-next{ right: 14px; } 
    .ehs-lb-counter{ 
      position: absolute; 
      bottom: 14px; 
      left: 50%; 
      transform: translateX(-50%); 
      color: #fff; 
      background: rgba(255,255,255,.12); 
      padding: 8px 14px; 
      border-radius: 999px; 
      font-size: 14px;
      font-weight: 600;
    }

    /* CTA */
    .cta{
      background:linear-gradient(180deg, var(--card), #fff);
      border-top:1px solid var(--border);
      padding:34px 16px;
      text-align:center;
    }
    .cta h2{font-size:24px;margin-bottom:8px}
    .cta p{
      color:var(--muted);
      font-size:15px;
      max-width:70ch;
      margin:0 auto 16px;
    }
    .ehs-cta-actions{
      display:flex;
      gap:10px;
      justify-content:center;
      flex-wrap:wrap;
      margin-top:12px;
    }

    /* RESPONSIVE */
    @media (min-width: 640px){
      .container{padding:0 20px}
      .hero .container{padding:44px 20px 34px}
      .hero h2{font-size:34px}
      .ehs-gallery-grid{ 
        grid-template-columns: repeat(3, 1fr); 
      }
    }
    @media (min-width: 980px){
      .hero .container{padding:68px 24px 48px}
      .hero-card{padding:22px}
      .hero h2{font-size:44px}
      .hero p{font-size:16.5px}
      .ehs-gallery-grid{ 
        grid-template-columns: repeat(4, 1fr); 
      }
    }
    html{scroll-behavior:smooth}
  </style>




  <!-- HEADER -->
  <header class="header">
    <div class="container">
      <div class="header-wrap">
        <div class="brand">
          <h1>Elite Home Services</h1>
          <p>Professional Home Improvement • London, ON</p>
        </div>

        <div class="header-actions">
          <a class="pill" href="tel:+15196972361">📞 <strong>(519) 697-2361</strong></a>
          <a class="pill" href="mailto:contact@elitehomeservices.ca">✉️ <strong>contact@elitehomeservices.ca</strong></a>
        </div>
      </div>
    </div>
  </header>

  <!-- HERO -->
  <section class="hero">
    <div class="container">
      <div class="hero-card">
        <h2>Our Completed Projects</h2>
        <p>
          Take a look at our portfolio to see the precision, care, and quality craftsmanship we bring to every project.
          From painting and flooring to custom décor and installations — we deliver results you'll be proud of.
        </p>

        <div class="hero-cta">
          <a class="btn btn-primary" href="tel:+15196972361">Get Your Free Quote</a>
          <a class="btn btn-outline" href="mailto:contact@elitehomeservices.ca">Email Us</a>
        </div>

        <div class="badges">
          <span class="badge"><span class="dot"></span> Professional Finishing</span>
          <span class="badge"><span class="dot"></span> Attention to Detail</span>
          <span class="badge"><span class="dot"></span> Quality Results</span>
        </div>
      </div>
    </div>
  </section>

  <!-- GALLERY -->
  <section class="ehs-gallery"> 
    <div class="ehs-gallery-wrap"> 
      <h2>Our Work Gallery</h2> 
      <p class="ehs-gallery-intro">Browse through our completed projects showcasing painting, wall repair, flooring, fencing, custom décor, and more. Click any image to view full size.</p> 

      <div class="ehs-gallery-grid" id="ehsGalleryGrid"> 
        <!-- YOUR REAL PROJECT PHOTOS FIRST -->
        <img class="ehs-thumb" src="https://i.imgur.com/vACI71h.jpg" alt="Elite Home Services Project">
     <img class="ehs-thumb" src="https://i.imgur.com/DbcGfaJ.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/lv0ujtj.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/CXCd8eT.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/dXaLZLM.jpg" alt="Elite Home Services Project">
       <img class="ehs-thumb" src="https://i.imgur.com/4aNT8Ys.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/7RI0eGq.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/QYVAKN8.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/CioeDzk.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/xh6tk88.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/TQlCajJ.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/aXFZvQy.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/c3AgXnD.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/73CepFp.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/j469SAj.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/5cSfbYe.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/Je1J53l.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/giBt4kf.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/0SZC5Gn.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/uAiTWDu.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/zn6n0w4.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/csWfuLT.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/VgAufOS.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/SDuSppc.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/TAaXbVo.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/NWCy9Cy.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/AyJ3AqL.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/C4Fnvi9.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/LQCkpqB.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/oHATeTl.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/Qq3Fhm4.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/t1WcZ9n.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/001qShl.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/bibfL4U.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/VFzu7Wm.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/tAvNkHE.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/avu4hjo.jpg" alt="Elite Home Services Project">
        <img class="ehs-thumb" src="https://i.imgur.com/MahBWti.jpg" alt="Elite Home Services Project">

        <!-- Pinterest Placeholder Images LAST -->
        <img class="ehs-thumb" src="https://i.pinimg.com/1200x/30/52/5d/30525dad8f1b4da0ed38c44ed999d458.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/736x/ca/b3/23/cab323a621c0469982f4f2c448ff737a.jpg" alt="Home Project">
        <img class="ehs-thumb" src="https://i.pinimg.com/1200x/eb/4a/68/eb4a68d6f83b033d70bc01a4bf792a98.jpg" alt="Home Project">
        <img class="ehs-thumb" src="https://i.pinimg.com/736x/49/2e/a6/492ea68084095a27c9a6110198ed6fef.jpg" alt="Home Project">
        <img class="ehs-thumb" src="https://i.pinimg.com/736x/02/b9/c5/02b9c5ca5ec6c5bc2fa994185f33d536.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/736x/42/28/c5/4228c55f45c598e441713bf4b4202780.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/736x/6b/5a/e8/6b5ae8ddbe509e39d43e20b9abb3d044.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/736x/55/fb/7b/55fb7bf83dd92fc0e43fbaa1a6795ac3.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/736x/3d/3d/ef/3d3defd93e239c0447efef6095d0863d.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/736x/0a/27/42/0a27424c216871b6e2273e35462cf876.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/1200x/71/a7/e5/71a7e5c9efab13548b5da13c20329e08.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/1200x/df/e6/c0/dfe6c01f83fe30a21cb4fd207605a76a.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/1200x/1d/95/35/1d953551c9dc8eba7806a1bc2efb3bc5.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/736x/ec/4f/2c/ec4f2c0506e1227df1deaa6f51872719.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/1200x/04/d1/cd/04d1cde7775cbd265826384451a535fd.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/736x/28/3b/d9/283bd9483aef910b00b482f729420f23.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/1200x/85/d1/7a/85d17a275962c9628107f3b35b93e850.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/736x/fd/17/21/fd172103fa8b8c1ba840ab5818e3ae9a.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/736x/53/f7/45/53f745ec8be773bca7b1d9d0047c5bbc.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/736x/83/a7/47/83a747cc100509318ac5eaf80fb1399d.jpg" alt="Home Project"> 
        <img class="ehs-thumb" src="https://i.pinimg.com/1200x/57/5d/e1/575de1eed160baf017bc6bd84ae6e1e8.jpg" alt="Home Project"> 
      </div> 
    </div> 
  </section> 

  <!-- LIGHTBOX -->
  <div class="ehs-lightbox" id="ehsLightbox"> 
    <button class="ehs-lb-close" id="ehsLbClose">✕</button> 
    <button class="ehs-lb-arrow ehs-lb-prev" id="ehsLbPrev">‹</button> 
    <figure class="ehs-lb-figure"><img id="ehsLbImg" src="" alt="Project Image"></figure> 
    <button class="ehs-lb-arrow ehs-lb-next" id="ehsLbNext">›</button> 
    <div class="ehs-lb-counter" id="ehsLbCounter"></div> 
  </div>

  <!-- CTA -->
  <section class="cta">
    <div class="container">
      <h2>Ready to Start Your Project?</h2>
      <p>
        Contact us today for a free estimate. We focus on quality workmanship, transparent pricing, and customer satisfaction.
      </p>
      <div class="ehs-cta-actions">
        <a class="btn btn-primary" href="tel:+15196972361">Call Now</a>
        <a class="btn btn-primary" href="mailto:contact@elitehomeservices.ca">Email Us</a>
        <a class="btn btn-primary" href="https://wa.me/15198518887">WhatsApp</a>
      </div>
    </div>
  </section>

  <script> 
  (function(){ 
    const grid = document.getElementById('ehsGalleryGrid'); 
    const thumbs = Array.from(grid.querySelectorAll('.ehs-thumb')); 
    const lb = document.getElementById('ehsLightbox'); 
    const lbImg = document.getElementById('ehsLbImg'); 
    const lbCounter = document.getElementById('ehsLbCounter'); 
    let index = 0; 
    
    function openLightbox(i){ 
      index = i; 
      lb.classList.add('is-open'); 
      render(); 
    } 
    
    function render(){ 
      lbImg.src = thumbs[index].src; 
      lbCounter.textContent = (index + 1) + ' / ' + thumbs.length; 
    } 
    
    thumbs.forEach((img, i) => img.onclick = () => openLightbox(i)); 
    document.getElementById('ehsLbClose').onclick = () => lb.classList.remove('is-open'); 
    document.getElementById('ehsLbPrev').onclick = () => { 
      index = (index - 1 + thumbs.length) % thumbs.length; 
      render(); 
    }; 
    document.getElementById('ehsLbNext').onclick = () => { 
      index = (index + 1) % thumbs.length; 
      render(); 
    }; 
    lb.onclick = (e) => { 
      if(e.target === lb) lb.classList.remove('is-open'); 
    }; 
    
    // Keyboard navigation
    document.addEventListener('keydown', (e) => {
      if(!lb.classList.contains('is-open')) return;
      if(e.key === 'Escape') lb.classList.remove('is-open');
      if(e.key === 'ArrowLeft') { index = (index - 1 + thumbs.length) % thumbs.length; render(); }
      if(e.key === 'ArrowRight') { index = (index + 1) % thumbs.length; render(); }
    });
  })(); 
  </script










  

our projects Footer




<meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elite Home Services Footer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
        }
    </style>



    <section class="py-12 bg-gradient-to-br from-amber-900 to-amber-950 text-white">
        <div class="container max-w-4xl mx-auto px-4 text-center">
            <h2 class="text-2xl md:text-3xl font-bold mb-3">Looking for Reliable Home Services?</h2>
            <p class="text-md opacity-90 mb-8 max-w-2xl mx-auto">
                Contact us today for a free estimate. We focus on quality workmanship, transparent pricing, and customer satisfaction.
            </p>
            
            <div class="flex flex-row justify-center items-center gap-2 md:gap-4 mb-16">
                <a href="tel:+15196972361" class="flex items-center gap-2 bg-white/10 hover:bg-white/20 border border-white/20 rounded-full px-3 py-2 transition-all duration-300 hover:scale-105 text-xs md:text-sm">
                    <span class="w-6 h-6 rounded-full bg-green-500 flex items-center justify-center flex-shrink-0">
                        <svg class="h-3 w-3 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path>
                        </svg>
                    </span>
                    <span class="font-bold">Call Now</span>
                </a>

                <a href="mailto:contact@elitehomeservices.ca" class="flex items-center gap-2 bg-white/10 hover:bg-white/20 border border-white/20 rounded-full px-3 py-2 transition-all duration-300 hover:scale-105 text-xs md:text-sm">
                    <span class="w-6 h-6 rounded-full bg-amber-600 flex items-center justify-center flex-shrink-0">
                        <svg class="h-3 w-3 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path>
                        </svg>
                    </span>
                    <span class="font-bold">Email Us</span>
                </a>

                <a href="https://wa.me/15198518887" class="flex items-center gap-2 bg-white/10 hover:bg-white/20 border border-white/20 rounded-full px-3 py-2 transition-all duration-300 hover:scale-105 text-xs md:text-sm">
                    <span class="w-6 h-6 rounded-full bg-emerald-500 flex items-center justify-center flex-shrink-0">
                        <svg class="h-3 w-3 text-white" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.890-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"></path>
                        </svg>
                    </span>
                    <span class="font-bold">WhatsApp</span>
                </a>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-left border-t border-white/10 pt-12">
                
                <div class="bg-white/5 backdrop-blur-sm border border-white/10 rounded-2xl p-6">
                    <div class="text-xl font-bold mb-3" style="font-family: 'Playfair Display', serif;">Elite Home Services</div>
                    <p class="opacity-80 text-xs leading-relaxed mb-4">
                        Professional home improvement based in London, Ontario. We pride ourselves on clean finishing and reliable scheduling.
                    </p>
                    <div class="flex flex-wrap gap-2 mb-4">
                        <span class="text-[10px] font-bold px-2 py-1 rounded-full bg-white/10 border border-white/20">Clean Finishing</span>
                        <span class="text-[10px] font-bold px-2 py-1 rounded-full bg-white/10 border border-white/20">Reliable Scheduling</span>
                        <span class="text-[10px] font-bold px-2 py-1 rounded-full bg-white/10 border border-white/20">Quality Results</span>
                    </div>
                </div>

                <div class="bg-white/5 backdrop-blur-sm border border-white/10 rounded-2xl p-6">
                    <h4 class="text-sm font-bold mb-4 pb-2 border-b border-amber-500 inline-block">Navigation</h4>
                    <div class="grid grid-cols-2 gap-4">
                        <ul class="space-y-2 text-xs opacity-80">
                            <li><a href="/" class="hover:underline">Home</a></li>
                            <li><a href="/services/" class="hover:underline">Services</a></li>
                            <li><a href="/Our Projects/" class="hover:underline">Our Projects</a></li>
                        </ul>
                        <ul class="space-y-2 text-xs opacity-80">
                            <li><a href="/about/" class="hover:underline">About Us</a></li>
                            <li><a href="/faqs/" class="hover:underline">FAQs</a></li>
                            <li><a href="/customer-reviews/" class="hover:underline">Reviews</a></li>
                            <li><a href="/contact/" class="hover:underline">Contact</a></li>
                        </ul>
                    </div>
                </div>

                <div class="bg-white/5 backdrop-blur-sm border border-white/10 rounded-2xl p-6">
                    <h4 class="text-sm font-bold mb-4 pb-2 border-b border-amber-500 inline-block">Our Team</h4>
                    
                    <div class="space-y-2">
                        <div class="flex justify-between items-center bg-black/20 p-2 rounded-lg border border-white/5">
                            <span class="text-xs font-bold">Isa Hasan</span>
                            <a href="tel:+15196972361" class="text-[11px] opacity-90 hover:text-amber-400 font-mono">(519) 697-2361</a>
                        </div>
                        <div class="flex justify-between items-center bg-black/20 p-2 rounded-lg border border-white/5">
                            <span class="text-xs font-bold">Musa Hasan</span>
                            <a href="tel:+12265040348" class="text-[11px] opacity-90 hover:text-amber-400 font-mono">(226) 504-0348</a>
                        </div>
                        <div class="flex justify-between items-center bg-black/20 p-2 rounded-lg border border-white/5">
                            <span class="text-xs font-bold">Abdul Alali</span>
                            <a href="tel:+12264486508" class="text-[11px] opacity-90 hover:text-amber-400 font-mono">(226) 448-6508</a>
                        </div>
                    </div>

                    <div class="mt-4 pt-4 border-t border-white/10 flex flex-col gap-2">
                        <div class="flex gap-2 items-center text-[11px] opacity-70">
                            <span>📍</span> 1157 Oakcrossing Rd, London, ON
                        </div>
                        <div class="flex gap-2 items-center text-[11px] opacity-70">
                            <span>✉️</span> contact@elitehomeservices.ca
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="mt-12 text-center text-[10px] opacity-40">
                © 2026 Elite Home Services. Serving Ontario with Excellence.
            </div>
        </div>
    </section>
