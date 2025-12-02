# <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1"/>
  <title>RUDEO — Ruvuma Development Organization</title>
  <meta name="description" content="RUDEO empowers communities across Tanzania through health, education, youth & women empowerment, environment, legal aid, and disaster preparedness."/>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Poppins:wght@600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --magenta:#C0176B; --purple:#6B2CA6; --green:#2EA75B; --blue:#1E78D6; --orange:#F28A1C; --red:#E64848;
      --ink:#222; --muted:#666; --bg:#fff;
    }
    *{box-sizing:border-box}
    body{margin:0; font-family:Inter,system-ui,Segoe UI,Roboto,Arial,sans-serif; color:var(--ink); background:var(--bg)}
    a{color:var(--magenta); text-decoration:none}
    .topbar{background:var(--magenta); color:#fff; padding:6px 16px; display:flex; flex-wrap:wrap; gap:12px; justify-content:center; font-size:14px}
    .topbar b{font-weight:700}
    header{border-bottom:1px solid #eee; background:linear-gradient(180deg,#fff 0%,#fff 60%,#f9f0f6 100%)}
    .nav{max-width:1100px; margin:0 auto; display:flex; align-items:center; justify-content:space-between; padding:14px 20px}
    .brand{display:flex; align-items:center; gap:12px}
    .logo{
      width:60px; height:60px; border-radius:50%; position:relative; overflow:hidden;
      background:conic-gradient(from 160deg,var(--green) 0 30%, var(--magenta) 30% 100%);
    }
    .logo::before{
      content:""; position:absolute; inset:12px;
      background:
        radial-gradient(circle at 50% 25%, var(--orange) 6px, transparent 7px),
        radial-gradient(circle at 22% 72%, var(--red) 6px, transparent 7px),
        radial-gradient(circle at 78% 72%, var(--blue) 6px, transparent 7px);
      border-radius:50%;
    }
    .site-title{font-family:Poppins,Inter,sans-serif; font-weight:700}
    .site-title span{color:var(--magenta)}
    .menu a{color:#333; font-weight:600; margin-left:16px; padding:8px 10px; border-radius:8px}
    .menu a.cta{background:var(--magenta); color:#fff}
    .lang-toggle{display:flex; gap:8px; align-items:center}
    .lang-btn{border:1px solid #ddd; background:#fff; color:#333; padding:6px 10px; border-radius:8px; font-weight:600; cursor:pointer}
    .lang-btn.active{border-color:var(--magenta); color:#fff; background:var(--magenta)}
    .hero{max-width:1100px; margin:20px auto 26px; padding:0 20px; text-align:center}
    .hero h1{font-family:Poppins,Inter,sans-serif; font-size:32px; margin:8px 0 12px}
    .hero p{color:var(--muted); max-width:800px; margin:0 auto 16px}
    .cta-row{display:flex; gap:12px; justify-content:center; flex-wrap:wrap}
    .btn{border:0; border-radius:10px; padding:12px 18px; font-weight:700; cursor:pointer}
    .btn.primary{background:var(--magenta); color:#fff}
    .btn.outline{background:#fff; color:var(--magenta); border:2px solid var(--magenta)}
    .focus-grid{max-width:1100px; margin:20px auto; padding:0 20px; display:grid; grid-template-columns:repeat(4,1fr); gap:12px}
    .focus-card{border-radius:12px; color:#fff; padding:18px 16px; font-weight:700; text-align:center}
    .focus-card.green{background:var(--green)} .focus-card.magenta{background:var(--magenta)}
    .focus-card.blue{background:var(--blue)} .focus-card.orange{background:var(--orange)}
    section{padding:30px 20px}
    .wrap{max-width:1100px; margin:0 auto}
    h2{font-family:Poppins,Inter,sans-serif; font-size:26px; margin:0 0 12px}
    .two-col{display:grid; grid-template-columns:1.1fr 1fr; gap:24px}
    .card{background:#fff; border:1px solid #eee; border-radius:12px; padding:18px}
    .list{margin:0; padding-left:18px} .list li{margin:6px 0}
    .pill{display:inline-block; padding:6px 10px; border-radius:999px; background:#f5f5f5; margin:4px 6px 0 0; font-size:13px; color:#444; border:1px solid #eee}
    .values{display:flex; flex-wrap:wrap; gap:8px}
    .impact{display:grid; grid-template-columns:repeat(3,1fr); gap:16px}
    .contact{background:#fafafa; border-top:1px solid #eee; border-bottom:1px solid #eee}
    .contact-grid{display:grid; grid-template-columns:1fr 1fr; gap:18px}
    .footer{background:var(--magenta); color:#fff; text-align:center; padding:18px 20px}
    .footer small{display:block; opacity:0.9}
    @media(max-width:900px){.focus-grid{grid-template-columns:repeat(2,1fr)} .two-col{grid-template-columns:1fr} .impact{grid-template-columns:1fr 1fr} .contact-grid{grid-template-columns:1fr}}
    @media(max-width:520px){.menu{display:none} .hero h1{font-size:26px} .focus-grid{grid-template-columns:1fr} .impact{grid-template-columns:1fr}}
    /* bilingual content visibility */
    [data-lang="sw"] .en{display:none} [data-lang="en"] .sw{display:none}
  </style>
</head>
<body data-lang="en">
  <!-- Top contact bar -->
  <div class="topbar">
    <span><b>P.O.BOX:</b> 175</span>
    <span><b>Mobile:</b> +255 625 348 941</span>
    <span><b>Email:</b> rude24organization@yahoo.com</span>
    <span><b>Office:</b> Manzense Street, Misufini Ward, Songea Municipal, Ruvuma</span>
  </div>

  <!-- Header / Navigation -->
  <header>
    <div class="nav">
      <div class="brand">
        <div class="logo" aria-hidden="true"></div>
        <div class="site-title">
          <div><span>RUVUMA</span> DEVELOPMENT ORGANIZATION</div>
          <small style="color:#555" class="en">Empowering Communities, Transforming Lives</small>
          <small style="color:#555" class="sw">Kuimarisha Jamii, Kubadilisha Maisha</small>
        </div>
      </div>
      <nav class="menu" aria-label="Primary">
        <a href="#about" class="en">About us</a>
        <a href="#about" class="sw">Kuhusu sisi</a>
        <a href="#objectives" class="en">Objectives</a>
        <a href="#objectives" class="sw">Malengo</a>
        <a href="#programs" class="en">Programs</a>
        <a href="#programs" class="sw">Mitungo</a>
        <a href="#services" class="en">Services</a>
        <a href="#services" class="sw">Huduma</a>
        <a href="#policies" class="en">Policies</a>
        <a href="#policies" class="sw">Sera</a>
        <a href="#contact" class="cta en">Contact</a>
        <a href="#contact" class="cta sw">Wasiliana</a>
      </nav>
      <div class="lang-toggle" aria-label="Language toggle">
        <button class="lang-btn active" data-setlang="en">English</button>
        <button class="lang-btn" data-setlang="sw">Kiswahili</button>
      </div>
    </div>

    <!-- Hero -->
    <div class="hero">
      <h1 class="en">Empowering communities across Tanzania through health, education, and opportunity</h1>
      <h1 class="sw">Kuimarisha jamii Tanzania kupitia afya, elimu, na fursa</h1>
      <p class="en">RUDEO is a registered Non-Governmental Organization (Certificate No. 00NGO/R/6053, founded in 2024) operating nationally to support marginalized groups including children, people with disabilities, orphans, widows, and vulnerable youth.</p>
      <p class="sw">RUDEO ni Asasi Isiyo ya Kiserikali (Cheti No. 00NGO/R/6053, iliyoanzishwa 2024) inayofanya kazi kitaifa kusaidia makundi hatarishi wakiwemo watoto, watu wenye ulemavu, yatima, wajane, na vijana.</p>
      <div class="cta-row">
        <a class="btn primary en" href="#get-involved">Join us</a>
        <a class="btn primary sw" href="#get-involved">Jiunge nasi</a>
        <a class="btn outline en" href="#contact">Partner with us</a>
        <a class="btn outline sw" href="#contact">Shirikiana nasi</a>
      </div>
    </div>

    <!-- Focus areas quick links -->
    <div class="focus-grid">
      <a class="focus-card green en" href="#programs">Health</a>
      <a class="focus-card green sw" href="#programs">Afya</a>
      <a class="focus-card magenta en" href="#programs">Education</a>
      <a class="focus-card magenta sw" href="#programs">Elimu</a>
      <a class="focus-card blue en" href="#programs">Youth empowerment</a>
      <a class="focus-card blue sw" href="#programs">Uwezeshaji wa vijana</a>
      <a class="focus-card orange en" href="#programs">Environment</a>
      <a class="focus-card orange sw" href="#programs">Mazingira</a>
    </div>
  </header>

  <!-- About -->
  <section id="about">
    <div class="wrap two-col">
      <div class="card">
        <h2 class="en">About RUDEO</h2>
        <h2 class="sw">Kuhusu RUDEO</h2>
        <p class="en">Ruvuma Development Organization (RUDEO) was established in 2024 and registered under the NGOs Act No.24 of 2002 (amended 2005 and 2019). The head office is based in Songea Municipal, Ruvuma region, and operations extend nationally through partnerships with local and international entities.</p>
        <p class="sw">Ruvuma Development Organization (RUDEO) ilianzishwa mwaka 2024 na kusajiliwa chini ya Sheria ya Mashirika Yasiyo ya Kiserikali Na.24 ya 2002 (marekebisho ya 2005 & 2019). Makao makuu yapo Songea Manispaa, Mkoa wa Ruvuma, na shughuli zake ni za kitaifa kupitia ushirikiano wa ndani na kimataifa.</p>
        <p class="en"><b>Vision:</b> A healthy community aware of good governance, free from violence and discrimination, economically stable, and environmentally sound.</p>
        <p class="sw"><b>Maono:</b> Jamii yenye afya, inayotambua utawala bora, huru dhidi ya ukatili na ubaguzi, imara kiuchumi na yenye kuheshimu mazingira.</p>
        <p class="en"><b>Mission:</b> Empower communities with better health, good governance, entrepreneurship skills, environmental and climate protection, anti-discrimination awareness, and rights education through outreach, service delivery, and participation.</p>
        <p class="sw"><b>Missioni:</b> Kuwawezesha jamii kupitia afya bora, utawala bora, ujuzi wa ujasiriamali, ulinzi wa mazingira na tabianchi, kuelimisha dhidi ya ubaguzi, na haki kupitia uhamasishaji, utoaji huduma, na ushiriki.</p>
      </div>
      <div class="card">
        <h2 class="en">Thematic areas</h2>
        <h2 class="sw">Maeneo ya kipaumbele</h2>
        <div>
          <span class="pill en">Health</span> <span class="pill sw">Afya</span>
          <span class="pill en">Education</span> <span class="pill sw">Elimu</span>
          <span class="pill en">Communicable & Non-communicable diseases</span> <span class="pill sw">Magonjwa ya kuambukiza & yasiyo ya kuambukiza</span>
          <span class="pill en">Economic strengthening</span> <span class="pill sw">Kuimarisha uchumi</span>
          <span class="pill en">Women empowerment</span> <span class="pill sw">Uwezeshaji wa wanawake</span>
          <span class="pill en">Youth empowerment</span> <span class="pill sw">Uwezeshaji wa vijana</span>
          <span class="pill en">WASH & Environment</span> <span class="pill sw">WASH & Mazingira</span>
          <span class="pill en">Free legal aid & education</span> <span class="pill sw">Msaada wa kisheria na elimu</span>
          <span class="pill en">Emergency response & preparedness</span> <span class="pill sw">Mwitikio wa dharura & utayari</span>
          <span class="pill en">Human rights & democracy</span> <span class="pill sw">Haki za binadamu & demokrasia</span>
        </div>
      </div>
    </div>
  </section>

  <!-- Objectives -->
  <section id="objectives">
    <div class="wrap two-col">
      <div class="card">
        <h2 class="en">Objectives</h2>
        <h2 class="sw">Malengo</h2>
        <ul class="list en">
          <li>Improve health services for disabled children and control pandemic/epidemic diseases.</li>
          <li>Raise awareness on gender equality and discrimination.</li>
          <li>Empower disabled people and youth with vocational skills and economic opportunities.</li>
          <li>Enhance environmental care and management.</li>
          <li>Increase awareness on global disasters, floods, and droughts.</li>
        </ul>
        <ul class="list sw">
          <li>Kuboresha huduma za afya kwa watoto wenye ulemavu na kudhibiti magonjwa ya milipuko.</li>
          <li>Kuongeza uelewa kuhusu usawa wa kijinsia na kupinga ubaguzi.</li>
          <li>Kuwawezesha watu wenye ulemavu na vijana kwa ujuzi wa ufundi na fursa za kiuchumi.</li>
          <li>Kuboresha utunzaji na usimamizi wa mazingira.</li>
          <li>Kuongeza uelewa kuhusu majanga ya dunia, mafuriko na ukame.</li>
        </ul>
      </div>
      <div class="card">
        <h2 class="en">Values</h2>
        <h2 class="sw">Misingi ya maadili</h2>
        <div class="values">
          <span class="pill en">Honesty</span><span class="pill sw">Ukweli</span>
          <span class="pill en">Transparency</span><span class="pill sw">Uwazi</span>
          <span class="pill en">Accountability</span><span class="pill sw">Uwajibikaji</span>
          <span class="pill en">Teamwork & Partnership</span><span class="pill sw">Ushirikiano & Kufanya kazi kwa pamoja</span>
          <span class="pill en">Sustainability</span><span class="pill sw">Uendelevu</span>
          <span class="pill en">Value for money</span><span class="pill sw">Thamani ya fedha</span>
          <span class="pill en">Networking</span><span class="pill sw">Mtandao wa ushirikiano</span>
          <span class="pill en">Mutual respect & care</span><span class="pill sw">Heshima na kujali</span>
        </div>
      </div>
    </div>
  </section>

  <!-- Programs & Services -->
  <section id="programs">
    <div class="wrap">
      <h2 class="en">Programs</h2>
      <h2 class="sw">Mitungo</h2>
      <div class="two-col">
        <div class="card">
          <ul class="list en">
            <li>Health and HIV education and support.</li>
            <li>School clubs for legal aid education and child support.</li>
            <li>Essay and drawing competitions (Primary, Secondary, Colleges, Universities).</li>
            <li>Capacity building and entrepreneurship training.</li>
            <li>Micro-credit scheme support and startup capital.</li>
            <li>Income Generating Activities (IGA) groups formation and support.</li>
            <li>Lobbying and advocacy for human rights.</li>
            <li>Environmental protection and climate action campaigns.</li>
            <li>Community development initiatives.</li>
            <li>Free legal aid services.</li>
          </ul>
          <ul class="list sw">
            <li>Elimu na uhamasishaji wa Afya na VVU.</li>
            <li>Vilabu vya shule kwa elimu ya msaada wa kisheria na ulinzi wa watoto.</li>
            <li>Shindano la insha na uchoraji (Msingi, Sekondari, Vyuo, Vyuo Vikuu).</li>
            <li>Kujenga uwezo na mafunzo ya ujasiriamali.</li>
            <li>Msaada wa mikopo midogo na mtaji wa kuanzisha.</li>
            <li>Uundaji na uimarishaji wa vikundi vya IGA.</li>
            <li>Ushawishi na utetezi wa haki za binadamu.</li>
            <li>Kampeni za ulinzi wa mazingira na tabianchi.</li>
            <li>Miradi ya maendeleo ya jamii.</li>
            <li>Huduma za msaada wa kisheria bila malipo.</li>
          </ul>
        </div>
        <div class="card" id="services">
          <h2 class="en">Services offered</h2>
          <h2 class="sw">Huduma zinazotolewa</h2>
          <ul class="list en">
            <li>Community health support to cancer patients, OVC/MVC, and youth.</li>
            <li>Improving water supply, environment conservation, and tree planting at water sources.</li>
            <li>Scholastic materials and school fees support to most vulnerable children and persons with disabilities.</li>
            <li>Basic needs support to marginalized groups, including medical fund disbursement via iCHF.</li>
            <li>Legal aid, elder care education, HIV/AIDS and malaria education for the community.</li>
            <li>Entrepreneurship skills training for IGA groups and startup capital support.</li>
            <li>School clubs running essay, practical, and drawing competitions.</li>
          </ul>
          <ul class="list sw">
            <li>Msaada wa afya ya jamii kwa wagonjwa wa saratani, OVC/MVC, na vijana.</li>
            <li>Kuboresha upatikanaji wa maji, uhifadhi wa mazingira, na upandaji miti katika vyanzo vya maji.</li>
            <li>Vifaa vya masomo na ada za shule kwa watoto walio hatarini na watu wenye ulemavu.</li>
            <li>Msaada wa mahitaji ya msingi kwa makundi yaliyo pembezoni, ikiwemo fedha za matibabu kupitia iCHF.</li>
            <li>Msaada wa kisheria, elimu ya utunzaji wa wazee, elimu ya VVU/UKIMWI na malaria.</li>
            <li>Mafunzo ya ujuzi wa ujasiriamali kwa vikundi vya IGA na msaada wa mtaji.</li>
            <li>Vilabu vya shule vinaendesha mashindano ya insha, vitendo, na uchoraji.</li>
          </ul>
        </div>
      </div>

      <div class="impact" style="margin-top:16px">
        <div class="card">
          <h3 class="en">Operational reach</h3>
          <h3 class="sw">Ufikikaji wa shughuli</h3>
          <p class="en">Rural and urban areas across Tanzania, with partnerships at grassroots and national levels.</p>
          <p class="sw">Maeneo ya vijijini na mijini kote Tanzania, kwa ushirikiano wa ngazi ya jamii na kitaifa.</p>
        </div>
        <div class="card">
          <h3 class="en">Human resources</h3>
          <h3 class="sw">Rasilimali watu</h3>
          <p class="en">10 staff: CEO, Program Manager, Health Officer, Project Accountant, Project Officer, IT Officer, Data Clerk, Office Attendant, and 2 Volunteers.</p>
          <p class="sw">Wafanyakazi 10: CEO, Meneja wa Programu, Afisa Afya, Mhasibu wa Mradi, Afisa Mradi, Afisa TEHAMA, Karani wa Takwimu, Mhudumu wa Ofisi, na Wajitolea 2.</p>
          <p class="en">500+ community volunteers: CHWs, ESL volunteers, CCWs, HBC, Paralegals, PSWs.</p>
          <p class="sw">Wajitolea 500+: Wahudumu wa Afya ya Jamii (CHW), ESL, CCW, HBC, Paralegal, na PSW.</p>
        </div>
        <div class="card">
          <h3 class="en">Policies & governance</h3>
          <h3 class="sw">Sera & utawala</h3>
          <p class="en">Human Resource Manual, Financial Manual, Disability Policy, Procurement Policy, Fraud Policy, HIV/AIDS Policy, Child Protection and Safeguarding Policies.</p>
          <p class="sw">Mwongozo wa Rasilimali Watu, Mwongozo wa Fedha, Sera ya Ulemavu, Ununuzi, Udhibiti Udanganyifu, Sera ya VVU/UKIMWI, Ulinzi na Usalama wa Mtoto.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Funding & Partners -->
  <section id="funding">
    <div class="wrap two-col">
      <div class="card">
        <h2 class="en">Sources of funding</h2>
        <h2 class="sw">Vyanzo vya fedha</h2>
        <ul class="list en">
          <li>Banks and Social Security institutions.</li>
          <li>District Councils and Government grants/subsidies.</li>
          <li>Membership entry and annual fees.</li>
          <li>Business contributions and charitable donations.</li>
          <li>Private companies and other donors.</li>
          <li>Income Generating Activities (IGA) by RUDEO.</li>
        </ul>
        <ul class="list sw">
          <li>Benki na taasisi za Hifadhi ya Jamii.</li>
          <li>Halmashauri za Wilaya na ruzuku/msaada wa Serikali.</li>
          <li>Michango ya uanachama (kujiunga na ada za mwaka).</li>
          <li>Michango ya wafanyabiashara na misaada ya taasisi.</li>
          <li>Makampuni binafsi na wafadhili wengine.</li>
          <li>Shughuli za kujipatia kipato (IGA) za RUDEO.</li>
        </ul>
      </div>
      <div class="card">
        <h2 class="en">Partnership approach</h2>
        <h2 class="sw">Mtazamo wa ushirikiano</h2>
        <p class="en">RUDEO partners with local individuals, entities, and international organizations to solve community challenges and deliver sustainable impact.</p>
        <p class="sw">RUDEO hushirikiana na watu wa ndani, taasisi, na mashirika ya kimataifa kutatua changamoto za jamii na kuleta matokeo endelevu.</p>
      </div>
    </div>
  </section>

  <!-- Get involved -->
  <section id="get-involved" class="contact">
    <div class="wrap">
      <h2 class="en">Get involved</h2>
      <h2 class="sw">Shiriki nasi</h2>
      <div class="contact-grid">
        <div class="card">
          <h3 class="en">Volunteer</h3>
          <h3 class="sw">Jitolee</h3>
          <p class="en">Join our 500+ volunteer network across Tanzania to support health education, school clubs, environmental action, and legal aid.</p>
          <p class="sw">Jiunge na mtandao wa wajitolea 500+ nchini kote kusaidia elimu ya afya, vilabu vya shule, ulinzi wa mazingira, na msaada wa kisheria.</p>
          <p><a href="#contact" class="btn outline en">Sign up</a><a href="#contact" class="btn outline sw">Jisajili</a></p>
        </div>
        <div class="card">
          <h3 class="en">Partner & donate</h3>
          <h3 class="sw">Shirikiana & changia</h3>
          <p class="en">Support RUDEO’s programs through funding, in-kind support, or strategic partnerships with institutions and businesses.</p>
          <p class="sw">Shirikiana na RUDEO kupitia ufadhili, msaada wa vifaa, au ushirikiano wa kimkakati na taasisi na biashara.</p>
          <p><a href="#contact" class="btn primary en">Contact RUDEO</a><a href="#contact" class="btn primary sw">Wasiliana na RUDEO</a></p>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <div class="wrap two-col">
      <div class="card">
        <h2 class="en">Contact us</h2>
        <h2 class="sw">Wasiliana nasi</h2>
        <p><b class="en">Address:</b><b class="sw">Anwani:</b> Manzense Street, Misufini Ward, Songea Municipal, Ruvuma</p>
        <p><b>P.O.BOX:</b> 175</p>
        <p><b class="en">Mobile:</b><b class="sw">Simu:</b> +255 625 348 941</p>
        <p><b>Email:</b> rude24organization@yahoo.com</p>
        <p class="en"><b>Registration:</b> 00NGO/R/6053 (NGOs Act No.24, amended 2005 & 2019)</p>
        <p class="sw"><b>Usajili:</b> 00NGO/R/6053 (Sheria ya NGOs No.24, marekebisho 2005 & 2019)</p>
      </div>
      <div class="card">
        <h2 class="en">Send a message</h2>
        <h2 class="sw">Tuma ujumbe</h2>
        <form action="#" method="post">
          <label class="en">Full name</label><label class="sw">Jina kamili</label>
          <input type="text" name="name" placeholder="Your name / Jina lako" style="width:100%;padding:10px;border:1px solid #ddd;border-radius:8px;margin:6px 0 10px;">
          <label class="en">Email</label><label class="sw">Barua pepe</label>
          <input type="email" name="email" placeholder="you@example.com" style="width:100%;padding:10px;border:1px solid #ddd;border-radius:8px;margin:6px 0 10px;">
          <label class="en">Message</label><label class="sw">Ujumbe</label>
          <textarea name="message" rows="4" placeholder="How would you like to collaborate? / Ungependa kushirikiana vipi?" style="width:100%;padding:10px;border:1px solid #ddd;border-radius:8px;margin:6px 0 12px;"></textarea>
          <button class="btn primary en" type="submit">Send</button>
          <button class="btn primary sw" type="submit">Tuma</button>
        </form>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <div class="wrap">
      <strong class="en">RUDEO — Empowering Communities, Transforming Lives</strong>
      <strong class="sw">RUDEO — Kuimarisha Jamii, Kubadilisha Maisha</strong>
      <small>© 2025 Ruvuma Development Organization. All rights reserved.</small>
    </div>
  </footer>

  <script>
    // Simple language toggle without external libraries
    const root = document.body;
    const btns = document.querySelectorAll('.lang-btn');
    btns.forEach(b=>{
      b.addEventListener('click', ()=>{
        btns.forEach(x=>x.classList.remove('active'));
        b.classList.add('active');
        const lang = b.getAttribute('data-setlang');
        root.setAttribute('data-lang', lang);
      });
    });
  </script>
</body>
</html>
