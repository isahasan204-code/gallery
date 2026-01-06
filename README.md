<section class="ehs-gallery"> 

  <div class="ehs-gallery-wrap"> 

    <h2>Photo Gallery</h2> 

    <p class="ehs-gallery-intro">Take a look at our portfolio to see the precision and care we bring to every project.</p> 

    <div class="ehs-gallery-grid" id="ehsGalleryGrid"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1505691938895-1758d7feb511?w=900&amp;auto=format&amp;fit=crop" alt="Photo 1"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1503387762-592deb58ef4e?w=900&amp;auto=format&amp;fit=crop" alt="Photo 2"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1570129477492-45c003edd2be?w=900&amp;auto=format&amp;fit=crop" alt="Photo 3"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1523413651479-597eb2da0ad6?w=900&amp;auto=format&amp;fit=crop" alt="Photo 4"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1560185008-5bf9f2849488?w=900&amp;auto=format&amp;fit=crop" alt="Photo 5"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1595526114035-0d45ed16cfbf?w=900&amp;auto=format&amp;fit=crop" alt="Photo 6"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1523755231516-e43fd2e8dca5?w=900&amp;auto=format&amp;fit=crop" alt="Photo 7"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1527030280862-64139fba04ca?w=900&amp;auto=format&amp;fit=crop" alt="Photo 8"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1502005229762-cf1b2da7c5d6?w=900&amp;auto=format&amp;fit=crop" alt="Photo 9"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1484154218962-a197022b5858?w=900&amp;auto=format&amp;fit=crop" alt="Photo 10"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1501183638710-841dd1904471?w=900&amp;auto=format&amp;fit=crop" alt="Photo 11"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1505693416388-ac5ce068fe85?w=900&amp;auto=format&amp;fit=crop" alt="Photo 12"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1501045661006-fcebe0257c3f?w=900&amp;auto=format&amp;fit=crop" alt="Photo 13"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1519710164239-da123dc03ef4?w=900&amp;auto=format&amp;fit=crop" alt="Photo 14"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1507089947368-19c1da9775ae?w=900&amp;auto=format&amp;fit=crop" alt="Photo 15"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1522708323590-d24dbb6b0267?w=900&amp;auto=format&amp;fit=crop" alt="Photo 16"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1494526585095-c41746248156?w=900&amp;auto=format&amp;fit=crop" alt="Photo 17"> 

      <img class="ehs-thumb" src="https://images.unsplash.com/photo-1493809842364-78817add7ffb?w=900&amp;auto=format&amp;fit=crop" alt="Photo 18"> 

    </div> 

  </div> 

</section> 

  

<div class="ehs-lightbox" id="ehsLightbox"> 

  <button class="ehs-lb-close" id="ehsLbClose">✕</button> 

  <button class="ehs-lb-arrow ehs-lb-prev" id="ehsLbPrev">‹</button> 

  <figure class="ehs-lb-figure"><img id="ehsLbImg" src=""></figure> 

  <button class="ehs-lb-arrow ehs-lb-next" id="ehsLbNext">›</button> 

  <div class="ehs-lb-counter" id="ehsLbCounter"></div> 

</div> 

  

<style> 

  .ehs-gallery{ padding: 48px 16px; font-family: Arial, sans-serif; color: #222; } 

  .ehs-gallery-wrap{ max-width: 1100px; margin: 0 auto; } 

  .ehs-gallery h2{ margin: 0 0 10px; font-size: 30px; } 

  .ehs-gallery-intro{ margin: 0 0 22px; font-size: 16px; line-height: 1.7; } 

  .ehs-gallery-grid{ display: grid; grid-template-columns: repeat(3, 1fr); gap: 10px; } 

  .ehs-thumb{ width: 100%; height: 160px; object-fit: cover; border-radius: 12px; cursor: pointer; border: 1px solid #eee; transition: transform .2s ease; } 

  .ehs-thumb:hover{ transform: scale(1.02); } 

  .ehs-lightbox{ position: fixed; inset: 0; background: rgba(0,0,0,.82); display: none; align-items: center; justify-content: center; z-index: 99999; padding: 16px; } 

  .ehs-lightbox.is-open{ display: flex; } 

  .ehs-lb-figure img{ max-width: 100%; max-height: 80vh; border-radius: 14px; box-shadow: 0 8px 30px rgba(0,0,0,.35); } 

  .ehs-lb-close, .ehs-lb-arrow{ position: absolute; background: rgba(255,255,255,.15); color: #fff; border: 0; cursor: pointer; border-radius: 999px; display: flex; align-items: center; justify-content: center; } 

  .ehs-lb-close{ top: 14px; right: 14px; width: 44px; height: 44px; font-size: 22px; } 

  .ehs-lb-arrow{ top: 50%; transform: translateY(-50%); width: 54px; height: 54px; font-size: 38px; } 

  .ehs-lb-prev{ left: 14px; } .ehs-lb-next{ right: 14px; } 

  .ehs-lb-counter{ position: absolute; bottom: 14px; left: 50%; transform: translateX(-50%); color: #fff; background: rgba(255,255,255,.12); padding: 6px 10px; border-radius: 999px; font-size: 14px; } 

</style> 

  

<script> 

(function(){ 

  const grid = document.getElementById('ehsGalleryGrid'); 

  const thumbs = Array.from(grid.querySelectorAll('.ehs-thumb')); 

  const lb = document.getElementById('ehsLightbox'); 

  const lbImg = document.getElementById('ehsLbImg'); 

  const lbCounter = document.getElementById('ehsLbCounter'); 

  let index = 0; 

  function openLightbox(i){ index = i; lb.classList.add('is-open'); render(); } 

  function render(){ 

    lbImg.src = thumbs[index].src; 

    lbCounter.textContent = (index + 1) + ' / ' + thumbs.length; 

  } 

  thumbs.forEach((img, i) => img.onclick = () => openLightbox(i)); 

  document.getElementById('ehsLbClose').onclick = () => lb.classList.remove('is-open'); 

  document.getElementById('ehsLbPrev').onclick = () => { index = (index - 1 + thumbs.length) % thumbs.length; render(); }; 

  document.getElementById('ehsLbNext').onclick = () => { index = (index + 1) % thumbs.length; render(); }; 

  lb.onclick = (e) => { if(e.target === lb) lb.classList.remove('is-open'); }; 

})(); 

</script>










  

Gallery Footer




<!-- ===== CODE 3 (UPDATED): CTA + ONE PREMIUM FOOTER (REPLACES BOTH FOOTERS) ===== -->

<!-- CTA -->
<section class="cta">
  <div class="container">
    <h2>Looking for Reliable Home Services?</h2>
    <p>
      Contact us today for a free estimate. We focus on quality workmanship, transparent pricing, and customer satisfaction.
    </p>
    <div class="ehs-cta-actions">
      <a class="btn btn-primary" href="tel:+15196972361">Call Now</a>
      <a class="btn btn-outline" href="mailto:contact@elitehomeservices.ca">Email Us</a>
      <a class="btn btn-outline" href="https://wa.me/15198518887">WhatsApp</a>
    </div>
  </div>
</section>

<!-- PREMIUM FOOTER -->
<footer class="ehs-footer">
  <div class="container">
    <div class="ehs-footer-top">
      <!-- Brand / About -->
      <div class="ehs-footer-col ehs-footer-brand">
        <div class="ehs-footer-logo">Elite Home Services</div>
        <p class="ehs-footer-desc">
          Professional home improvement based in London, Ontario. We pride ourselves on clean finishing, reliable scheduling,
          and high-quality results for every homeowner.
        </p>

        <div class="ehs-footer-badges" aria-label="highlights">
          <span>Clean Finishing</span>
          <span>Reliable Scheduling</span>
          <span>Quality Results</span>
        </div>

        <div class="ehs-footer-social" aria-label="social links">
          <a class="ehs-social" href="#" aria-label="Facebook" title="Facebook">FB</a>
          <a class="ehs-social" href="#" aria-label="Instagram" title="Instagram">IG</a>
          <a class="ehs-social" href="https://wa.me/15198518887" aria-label="WhatsApp" title="WhatsApp">WA</a>
        </div>
      </div>

      <!-- Navigation -->
      <div class="ehs-footer-col">
        <h4 class="ehs-footer-title">Navigation</h4>

        <div class="ehs-footer-links">
          <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/services/">Services</a></li>
            <li><a href="/projects/">Projects</a></li>
            <li><a href="/gallery/">Gallery</a></li>
          </ul>
          <ul>
            <li><a href="/about/">About Us</a></li>
            <li><a href="/faqs/">FAQs</a></li>
            <li><a href="/customer-reviews/">Reviews</a></li>
            <li><a href="/contact/">Contact</a></li>
          </ul>
        </div>
      </div>

      <!-- Contact -->
      <div class="ehs-footer-col">
        <h4 class="ehs-footer-title">Get In Touch</h4>

        <div class="ehs-footer-contact">
          <div class="ehs-contact-row">
            <span class="ehs-ico">📍</span>
            <div class="ehs-contact-text">1157 Oakcrossing Rd, London, ON N6H 0E9</div>
          </div>

          <div class="ehs-contact-row">
            <span class="ehs-ico">✉️</span>
            <div class="ehs-contact-text">
              <a href="mailto:contact@elitehomeservices.ca">contact@elitehomeservices.ca</a>
            </div>
          </div>

          <div class="ehs-team">
            <div class="ehs-team-card">
              <div class="ehs-team-name">Isa Hasan</div>
              <a class="ehs-team-phone" href="tel:+15196972361">(519) 697-2361</a>
            </div>

            <div class="ehs-team-card">
              <div class="ehs-team-name">Musa Hasan</div>
              <a class="ehs-team-phone" href="tel:+12265040348">(226) 504-0348</a>
            </div>

            <div class="ehs-team-card">
              <div class="ehs-team-name">Abdul Alali</div>
              <a class="ehs-team-phone" href="tel:+12264486508">(226) 448-6508</a>
            </div>
          </div>

          <div class="ehs-footer-mini-cta">
            <a class="ehs-mini-btn" href="/contact/">Request a Quote</a>
            <a class="ehs-mini-btn ehs-mini-btn-outline" href="mailto:contact@elitehomeservices.ca">Send Email</a>
          </div>
        </div>
      </div>
    </div>

    <div class="ehs-footer-bottom">
      <p>© <span id="ehs-year"></span> Elite Home Services. Serving Ontario with Excellence.</p>
    </div>
  </div>
</footer>

<style>
  /* CTA actions layout (keeps your existing CTA look, just improves button wrapping) */
  .ehs-cta-actions{
    display:flex;
    gap:10px;
    justify-content:center;
    flex-wrap:wrap;
    margin-top:12px;
  }

  /* PREMIUM FOOTER - matches your theme variables */
  .ehs-footer{
    background: var(--primary);
    color: var(--primary-foreground);
    border-top: 1px solid rgba(255,255,255,0.14);
    padding: 42px 0 18px;
  }

  .ehs-footer-top{
    display:grid;
    grid-template-columns: 1.15fr 0.9fr 1.2fr;
    gap: 24px;
    align-items:start;
  }

  .ehs-footer-col{
    background: rgba(255,255,255,0.06);
    border: 1px solid rgba(255,255,255,0.10);
    border-radius: 16px;
    padding: 16px;
  }

  .ehs-footer-brand{
    padding: 18px;
  }

  .ehs-footer-logo{
    font-family: 'Playfair Display', serif;
    font-size: 20px;
    font-weight: 700;
    letter-spacing: 0.3px;
    margin-bottom: 8px;
  }

  .ehs-footer-desc{
    opacity: 0.9;
    font-size: 13.5px;
    line-height: 1.7;
    margin-bottom: 14px;
    max-width: 52ch;
  }

  .ehs-footer-title{
    font-family: 'Inter', sans-serif;
    font-size: 14px;
    font-weight: 800;
    letter-spacing: 0.2px;
    margin: 0 0 12px 0;
    position: relative;
    padding-bottom: 10px;
  }

  .ehs-footer-title::after{
    content:"";
    position:absolute;
    left:0;
    bottom:0;
    width:42px;
    height:2px;
    background: var(--accent);
    border-radius: 999px;
  }

  /* badges */
  .ehs-footer-badges{
    display:flex;
    flex-wrap:wrap;
    gap:8px;
    margin-bottom: 12px;
  }
  .ehs-footer-badges span{
    font-size: 12px;
    font-weight: 700;
    padding: 8px 10px;
    border-radius: 999px;
    background: rgba(255,255,255,0.08);
    border: 1px solid rgba(255,255,255,0.12);
    color: var(--primary-foreground);
    opacity: 0.95;
  }

  /* social */
  .ehs-footer-social{
    display:flex;
    gap:10px;
    flex-wrap:wrap;
  }
  .ehs-social{
    width:40px;
    height:40px;
    display:inline-flex;
    align-items:center;
    justify-content:center;
    border-radius: 999px;
    text-decoration:none;
    font-weight: 900;
    font-size: 12px;
    color: var(--primary-foreground);
    background: rgba(255,255,255,0.08);
    border: 1px solid rgba(255,255,255,0.12);
    transition: transform .15s ease, opacity .15s ease, background .15s ease;
  }
  .ehs-social:hover{
    transform: translateY(-1px);
    background: rgba(255,255,255,0.14);
    opacity: 0.95;
  }

  /* footer links */
  .ehs-footer-links{
    display:grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px 18px;
  }

  .ehs-footer ul{ list-style:none; padding:0; margin:0; }
  .ehs-footer li{ margin-bottom: 10px; }

  .ehs-footer a{
    color: var(--primary-foreground);
    text-decoration:none;
    opacity: 0.9;
    font-size: 13.5px;
    font-weight: 600;
  }

  .ehs-footer a:hover{
    opacity: 1;
    text-decoration: underline;
  }

  /* contact rows */
  .ehs-footer-contact{ margin-top: 4px; }
  .ehs-contact-row{
    display:flex;
    gap:10px;
    align-items:flex-start;
    margin-bottom: 12px;
  }
  .ehs-ico{
    width:28px;
    height:28px;
    display:flex;
    align-items:center;
    justify-content:center;
    border-radius: 10px;
    background: rgba(255,255,255,0.08);
    border: 1px solid rgba(255,255,255,0.12);
    flex: 0 0 auto;
  }
  .ehs-contact-text{
    font-size: 13.5px;
    line-height: 1.55;
    opacity: 0.92;
  }

  /* team phones */
  .ehs-team{
    display:grid;
    grid-template-columns: 1fr;
    gap: 10px;
    margin-top: 12px;
  }
  .ehs-team-card{
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:10px;
    padding: 12px 12px;
    border-radius: 12px;
    background: rgba(0,0,0,0.12);
    border: 1px solid rgba(255,255,255,0.10);
  }
  .ehs-team-name{
    font-weight: 800;
    font-size: 13px;
    opacity: 0.95;
  }
  .ehs-team-phone{
    font-weight: 900;
    font-size: 13.5px;
    color: #fff;
    opacity: 0.95;
    white-space: nowrap;
  }

  /* mini CTA buttons inside footer */
  .ehs-footer-mini-cta{
    display:flex;
    gap:10px;
    flex-wrap:wrap;
    margin-top: 14px;
  }
  .ehs-mini-btn{
    display:inline-flex;
    align-items:center;
    justify-content:center;
    padding: 10px 14px;
    border-radius: 999px;
    font-weight: 900;
    font-size: 13px;
    text-decoration:none;
    border: 1px solid rgba(255,255,255,0.18);
    background: var(--accent);
    color: #1f140f;
    transition: transform .15s ease, opacity .15s ease;
  }
  .ehs-mini-btn:hover{ transform: translateY(-1px); opacity: 0.95; }

  .ehs-mini-btn-outline{
    background: rgba(255,255,255,0.08);
    color: var(--primary-foreground);
  }

  /* bottom bar */
  .ehs-footer-bottom{
    border-top: 1px solid rgba(255,255,255,0.14);
    margin-top: 18px;
    padding-top: 14px;
    text-align:center;
    font-size: 12.5px;
    opacity: 0.78;
  }

  /* Responsive */
  @media (max-width: 980px){
    .ehs-footer-top{
      grid-template-columns: 1fr 1fr;
    }
  }
  @media (max-width: 680px){
    .ehs-footer-top{
      grid-template-columns: 1fr;
    }
    .ehs-footer-links{
      grid-template-columns: 1fr 1fr;
    }
    .ehs-team-card{
      flex-direction: column;
      align-items:flex-start;
    }
  }
  @media (max-width: 420px){
    .ehs-footer-links{ grid-template-columns: 1fr; }
  }
</style>

<script>
  // year
  (function(){
    var el = document.getElementById("ehs-year");
    if(el) el.textContent = new Date().getFullYear();
  })();
</script>
 
