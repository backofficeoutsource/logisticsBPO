<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Accounts Payable Outsourcing | Infinity IPS</title>
<link href="https://fonts.googleapis.com/css2?family=Source+Serif+4:ital,wght@0,400;0,600;0,700;1,400&family=Source+Sans+3:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  html { scroll-behavior: smooth; }

  body {
    background-color: #0a0e1a !important;
    color: #e8edf8 !important;
    font-family: 'Source Sans 3', Arial, sans-serif;
    font-weight: 400;
    line-height: 1.75;
    overflow-x: hidden;
  }

  /* ─── HERO ─── */
  .ap-hero {
    position: relative;
    min-height: 70vh;
    display: flex;
    align-items: center;
    padding: 80px 5% 70px;
    overflow: hidden;
    background-color: #0a0e1a;
  }

  .ap-hero-bg {
    position: absolute;
    inset: 0;
    background-image: url('https://images.unsplash.com/photo-1554224311-beee460ae6ba?w=1600');
    background-size: cover;
    background-position: center;
    filter: brightness(0.12) saturate(0.5);
    z-index: 0;
  }

  .ap-hero-overlay {
    position: absolute;
    inset: 0;
    background: linear-gradient(160deg, rgba(10,14,26,0.92) 0%, rgba(10,14,26,0.65) 60%, rgba(10,14,26,0.97) 100%);
    z-index: 1;
  }

  .ap-hero-content {
    position: relative;
    z-index: 2;
    max-width: 1100px;
    margin: 0 auto;
    width: 100%;
  }

  .ap-hero-label {
    display: inline-block;
    font-size: 0.72rem;
    font-weight: 600;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: #00c8ee;
    margin-bottom: 1.25rem;
    padding-bottom: 0.5rem;
    border-bottom: 1px solid rgba(0,200,238,0.3);
  }

  .ap-hero h1 {
    font-family: 'Source Serif 4', Georgia, serif;
    font-size: clamp(2rem, 4.5vw, 3.6rem);
    font-weight: 700;
    line-height: 1.15;
    margin-bottom: 1.25rem;
    color: #e8edf8;
  }

  .ap-hero-sub {
    font-size: 1.05rem;
    color: #7a8ba8;
    max-width: 650px;
    line-height: 1.8;
    font-weight: 300;
  }

  /* ─── STATS BAR ─── */
  .ap-stats {
    background-color: #141c30;
    border-top: 1px solid rgba(100,140,180,0.15);
    border-bottom: 1px solid rgba(100,140,180,0.15);
    padding: 1.75rem 5%;
  }

  .ap-stats-inner {
    max-width: 1100px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1rem;
    text-align: center;
  }

  .ap-stat {
    padding: 0.5rem;
    border-right: 1px solid rgba(100,140,180,0.15);
  }
  .ap-stat:last-child { border-right: none; }

  .ap-stat-num {
    font-family: 'Source Serif 4', Georgia, serif;
    font-size: 1.9rem;
    font-weight: 700;
    color: #00aacc;
    line-height: 1;
    margin-bottom: 0.3rem;
  }

  .ap-stat-label {
    font-size: 0.74rem;
    color: #7a8ba8;
    text-transform: uppercase;
    letter-spacing: 0.07em;
  }

  /* ─── SHARED SECTION STYLES ─── */
  .ap-section {
    padding: 80px 5%;
    background-color: #0a0e1a;
  }

  .ap-section-alt {
    padding: 80px 5%;
    background-color: #0f1525;
    border-top: 1px solid rgba(100,140,180,0.12);
    border-bottom: 1px solid rgba(100,140,180,0.12);
  }

  .ap-inner {
    max-width: 1100px;
    margin: 0 auto;
  }

  .ap-label {
    display: block;
    font-size: 0.7rem;
    font-weight: 600;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: #00aacc;
    margin-bottom: 0.75rem;
  }

  .ap-title {
    font-family: 'Source Serif 4', Georgia, serif;
    font-size: clamp(1.6rem, 3vw, 2.4rem);
    font-weight: 700;
    line-height: 1.2;
    margin-bottom: 1.25rem;
    color: #e8edf8;
  }

  .ap-lead {
    font-size: 1rem;
    color: #9aaabf;
    max-width: 720px;
    line-height: 1.85;
    font-weight: 300;
    margin-bottom: 2rem;
  }

  /* ─── INLINE LINKS ─── */
  .ap-link {
    color: #00c8ee;
    text-decoration: underline;
    text-decoration-color: rgba(0,200,238,0.4);
    text-underline-offset: 3px;
    transition: color 0.2s;
  }
  .ap-link:hover { color: #ffffff; }

  /* ─── INTRO TEXT ─── */
  .ap-intro p {
    color: #9aaabf;
    margin-bottom: 1.1rem;
    font-size: 0.97rem;
    line-height: 1.85;
  }
  .ap-intro p strong { color: #e8edf8; font-weight: 500; }

  /* ─── BENEFITS LIST ─── */
  .ap-benefits-list {
    list-style: none;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 0.65rem;
    margin: 1.5rem 0 2rem;
  }

  .ap-benefits-list li {
    display: flex;
    align-items: flex-start;
    gap: 0.75rem;
    padding: 0.85rem 1rem;
    background-color: rgba(0,170,204,0.06);
    border: 1px solid rgba(0,170,204,0.15);
    font-size: 0.88rem;
    color: #9aaabf;
    line-height: 1.5;
    transition: background-color 0.2s;
  }
  .ap-benefits-list li:hover { background-color: rgba(0,170,204,0.1); }
  .ap-benefits-list li::before {
    content: '✓';
    color: #00aacc;
    font-weight: 700;
    font-size: 1rem;
    flex-shrink: 0;
  }

  /* ─── PROCESS GRID ─── */
  .ap-process-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1.5rem;
    margin-top: 2.5rem;
  }

  .ap-process-card {
    background-color: #111827;
    border: 1px solid rgba(100,140,180,0.15);
    border-left: 3px solid #00aacc;
    padding: 1.75rem;
    transition: border-left-color 0.25s, transform 0.25s;
  }
  .ap-process-card:hover {
    border-left-color: #00c8ee;
    transform: translateX(3px);
  }

  .ap-process-num {
    display: inline-block;
    width: 32px;
    height: 32px;
    background-color: rgba(0,170,204,0.1);
    border: 1px solid rgba(0,170,204,0.25);
    border-radius: 50%;
    text-align: center;
    line-height: 32px;
    font-size: 0.8rem;
    font-weight: 700;
    color: #00aacc;
    margin-bottom: 0.85rem;
  }

  .ap-process-card h3 {
    font-size: 1rem;
    font-weight: 600;
    color: #e8edf8;
    margin-bottom: 0.65rem;
  }

  .ap-process-card p {
    font-size: 0.88rem;
    color: #7a8ba8;
    line-height: 1.75;
  }

  /* ─── AUTOMATION FEATURES ─── */
  .ap-automation-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.25rem;
    margin-top: 2.5rem;
  }

  .ap-auto-card {
    background-color: #111827;
    border: 1px solid rgba(100,140,180,0.15);
    padding: 1.5rem;
    text-align: center;
    transition: border-color 0.25s, transform 0.25s;
  }
  .ap-auto-card:hover {
    border-color: rgba(0,170,204,0.3);
    transform: translateY(-3px);
  }

  .ap-auto-icon {
    font-size: 2rem;
    margin-bottom: 0.75rem;
    display: block;
  }

  .ap-auto-card h4 {
    font-size: 0.88rem;
    font-weight: 600;
    color: #e8edf8;
    margin-bottom: 0.4rem;
  }

  .ap-auto-card p {
    font-size: 0.8rem;
    color: #7a8ba8;
    line-height: 1.6;
  }

  /* ─── SPLIT LAYOUT ─── */
  .ap-split {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 4rem;
    align-items: start;
    margin-top: 2.5rem;
  }

  .ap-split-text p {
    color: #9aaabf;
    margin-bottom: 1.1rem;
    font-size: 0.95rem;
    line-height: 1.85;
  }
  .ap-split-text p strong { color: #e8edf8; font-weight: 500; }

  .ap-split-list {
    list-style: none;
    display: flex;
    flex-direction: column;
    gap: 0.55rem;
  }

  .ap-split-list li {
    display: flex;
    align-items: flex-start;
    gap: 0.65rem;
    font-size: 0.88rem;
    color: #7a8ba8;
    line-height: 1.5;
  }
  .ap-split-list li::before {
    content: '›';
    color: #00aacc;
    font-weight: 700;
    font-size: 1rem;
    flex-shrink: 0;
  }

  /* ─── INDUSTRIES GRID ─── */
  .ap-industries-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 0.85rem;
    margin-top: 2rem;
  }

  .ap-industry-tag {
    background-color: #111827;
    border: 1px solid rgba(100,140,180,0.15);
    padding: 0.75rem 1rem;
    text-align: center;
    font-size: 0.85rem;
    font-weight: 500;
    color: #9aaabf;
    transition: background-color 0.2s, border-color 0.2s;
  }
  .ap-industry-tag:hover {
    background-color: rgba(0,170,204,0.08);
    border-color: rgba(0,170,204,0.25);
    color: #00c8ee;
  }

  /* ─── WHY CHOOSE CARDS ─── */
  .ap-why-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1rem;
    margin-top: 2rem;
  }

  .ap-why-card {
    background-color: #111827;
    border: 1px solid rgba(100,140,180,0.15);
    padding: 1.25rem;
    display: flex;
    align-items: flex-start;
    gap: 0.85rem;
    transition: border-color 0.2s;
  }
  .ap-why-card:hover { border-color: rgba(0,170,204,0.25); }

  .ap-why-icon {
    font-size: 1.3rem;
    flex-shrink: 0;
    margin-top: 0.1rem;
  }

  .ap-why-card h4 {
    font-size: 0.88rem;
    font-weight: 600;
    color: #e8edf8;
    line-height: 1.4;
  }

  /* ─── CTA ─── */
  .ap-cta {
    background-color: #141c30;
    border-top: 1px solid rgba(100,140,180,0.15);
    text-align: center;
    padding: 90px 5%;
  }
  .ap-cta-inner { max-width: 680px; margin: 0 auto; }
  .ap-cta .ap-title { margin-bottom: 1rem; }
  .ap-cta .ap-lead { margin: 0 auto 2.25rem; text-align: center; max-width: 580px; }

  .ap-btn {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    background-color: #c8001a;
    color: #ffffff;
    padding: 0.85rem 2.25rem;
    font-weight: 600;
    font-size: 0.9rem;
    letter-spacing: 0.04em;
    text-decoration: none;
    transition: background-color 0.22s, transform 0.22s;
  }
  .ap-btn:hover { background-color: #e8001a; transform: translateY(-2px); color: #fff; }

  /* ─── FOOTER ─── */
  .ap-footer {
    background-color: #060810;
    border-top: 1px solid rgba(100,140,180,0.12);
    padding: 2rem 5%;
    text-align: center;
  }
  .ap-footer p { font-size: 0.78rem; color: #5a6a85; }
  .ap-footer a { color: #00aacc; text-decoration: none; }

  /* ─── REVEAL ANIMATION ─── */
  .ap-reveal {
    opacity: 0;
    transform: translateY(20px);
    transition: opacity 0.55s ease, transform 0.55s ease;
  }
  .ap-reveal.visible { opacity: 1; transform: translateY(0); }

  /* ─── RESPONSIVE ─── */
  @media (max-width: 1024px) {
    .ap-automation-grid { grid-template-columns: repeat(2, 1fr); }
  }
  @media (max-width: 768px) {
    .ap-split,
    .ap-process-grid { grid-template-columns: 1fr; gap: 2rem; }
    .ap-automation-grid,
    .ap-industries-grid { grid-template-columns: repeat(2, 1fr); }
    .ap-benefits-list { grid-template-columns: 1fr; }
    .ap-why-grid { grid-template-columns: 1fr; }
    .ap-stats-inner { grid-template-columns: repeat(2, 1fr); }
    .ap-stat:nth-child(2) { border-right: none; }
    .ap-stat { border-bottom: 1px solid rgba(100,140,180,0.15); padding-bottom: 1rem; }
    .ap-stat:nth-child(3), .ap-stat:nth-child(4) { border-bottom: none; }
    .ap-section, .ap-section-alt { padding: 60px 5%; }
  }
  @media (max-width: 480px) {
    .ap-automation-grid,
    .ap-industries-grid { grid-template-columns: 1fr; }
    .ap-hero { min-height: 60vh; }
  }
</style>
</head>
<body>

<!-- HERO -->
<div class="ap-hero">
  <div class="ap-hero-bg"></div>
  <div class="ap-hero-overlay"></div>
  <div class="ap-hero-content">
    <span class="ap-hero-label">Infinity IPS — Finance Outsourcing Services</span>
    <h1>Accounts Payable Outsourcing</h1>
    <p class="ap-hero-sub">Streamline vendor payments, reduce processing costs, and improve financial accuracy with specialized AP outsourcing designed for logistics and transportation companies.</p>
  </div>
</div>

<!-- STATS -->
<div class="ap-stats">
  <div class="ap-stats-inner">
    <div class="ap-stat">
      <div class="ap-stat-num">60%</div>
      <div class="ap-stat-label">Cost Reduction</div>
    </div>
    <div class="ap-stat">
      <div class="ap-stat-num">3x</div>
      <div class="ap-stat-label">Faster Processing</div>
    </div>
    <div class="ap-stat">
      <div class="ap-stat-num">99.8%</div>
      <div class="ap-stat-label">Invoice Accuracy</div>
    </div>
    <div class="ap-stat">
      <div class="ap-stat-num">100%</div>
      <div class="ap-stat-label">Audit Ready</div>
    </div>
  </div>
</div>

<!-- INTRO -->
<div class="ap-section">
  <div class="ap-inner">
    <span class="ap-label">Why Accounts Payable Outsourcing</span>
    <h2 class="ap-title">Strategic AP Management for Growing Businesses</h2>
    <div class="ap-intro ap-reveal">
      <p>In today's fast-paced financial environment, <strong>Accounts Payable Outsourcing has become a strategic solution</strong> for businesses looking to improve accuracy, reduce processing costs, and streamline vendor payments. Managing high invoice volumes manually often leads to delays, duplicate payments, and compliance risks. Therefore, companies are increasingly turning to specialized AP outsourcing partners to modernize their finance operations.</p>
      <p>At Infinity IPS, our <a href="https://infinity-logisticsbackoffice.com/services/accounts-payable/" class="ap-link">Accounts Payable</a> Outsourcing services combine industry expertise, automation tools, and structured workflows to help logistics and transportation companies maintain accurate, timely, and fully compliant payment processes. As a result, your internal finance team can focus on strategic financial planning instead of repetitive transactional tasks.</p>
    </div>
  </div>
</div>

<!-- WHY IT MATTERS -->
<div class="ap-section-alt">
  <div class="ap-inner">
    <span class="ap-label">Benefits & Impact</span>
    <h2 class="ap-title">Why Accounts Payable Outsourcing Matters</h2>
    <p class="ap-lead ap-reveal">Handling accounts payable internally can be resource-intensive. Moreover, growing businesses often struggle with invoice backlogs, vendor disputes, and inconsistent approval cycles. By outsourcing AP functions, companies gain access to trained specialists, standardized processes, and scalable support.</p>
    <p class="ap-lead ap-reveal">Our <a href="https://infinity-logisticsbackoffice.com/services/accounts-payable/" class="ap-link">Accounts Payable</a> solutions help organizations achieve measurable improvements:</p>
    <ul class="ap-benefits-list ap-reveal">
      <li>Reduce manual data entry errors</li>
      <li>Accelerate invoice processing cycles</li>
      <li>Improve vendor payment accuracy</li>
      <li>Strengthen financial controls</li>
      <li>Enhance cash flow visibility</li>
      <li>Lower operational overhead</li>
    </ul>
    <p class="ap-lead ap-reveal" style="margin-top:1.5rem;">Consequently, businesses experience smoother financial operations and stronger supplier relationships.</p>
  </div>
</div>

<!-- PROCESS MANAGEMENT -->
<div class="ap-section">
  <div class="ap-inner">
    <span class="ap-label">End-to-End Process Management</span>
    <h2 class="ap-title">Comprehensive AP Workflow Support</h2>
    <p class="ap-lead ap-reveal">Infinity IPS delivers comprehensive accounts payable outsourcing support tailored to logistics-driven businesses. Our structured workflow ensures every invoice moves through validation, approval, and payment efficiently.</p>
    <div class="ap-process-grid">
      <div class="ap-process-card ap-reveal">
        <span class="ap-process-num">1</span>
        <h3>Invoice Capture & Data Entry</h3>
        <p>Our team captures invoice data from multiple sources including email, EDI, and scanned documents. Additionally, we validate key fields such as vendor details, PO numbers, and charge codes to ensure accuracy from the start.</p>
      </div>
      <div class="ap-process-card ap-reveal">
        <span class="ap-process-num">2</span>
        <h3>2-Way and 3-Way Matching</h3>
        <p>We perform detailed matching between invoices, purchase orders, and goods receipts. As a result, discrepancies are identified early, which prevents overpayments and billing disputes.</p>
      </div>
      <div class="ap-process-card ap-reveal">
        <span class="ap-process-num">3</span>
        <h3>Vendor Management & Query Resolution</h3>
        <p>Our specialists handle vendor communications, resolve invoice exceptions, and maintain updated supplier records. This significantly reduces the workload on your internal finance team.</p>
      </div>
      <div class="ap-process-card ap-reveal">
        <span class="ap-process-num">4</span>
        <h3>Payment Processing & Reconciliation</h3>
        <p>We support payment scheduling, remittance processing, and account reconciliation. Consequently, your organization maintains timely payments and accurate financial records.</p>
      </div>
    </div>
  </div>
</div>

<!-- AUTOMATION -->
<div class="ap-section-alt">
  <div class="ap-inner">
    <span class="ap-label">Automation-Driven Efficiency</span>
    <h2 class="ap-title">AI-Powered AP Processing</h2>
    <p class="ap-lead ap-reveal">Modern accounts payable outsourcing services go beyond manual processing. Therefore, Infinity IPS integrates AI, OCR, and workflow automation into AP operations. Because of automation, businesses achieve higher processing speed while maintaining strong financial governance.</p>
    <div class="ap-automation-grid">
      <div class="ap-auto-card ap-reveal">
        <span class="ap-auto-icon">⚡</span>
        <h4>Faster Invoice Data Extraction</h4>
        <p>OCR technology captures invoice fields instantly</p>
      </div>
      <div class="ap-auto-card ap-reveal">
        <span class="ap-auto-icon">🤖</span>
        <h4>Reduced Human Intervention</h4>
        <p>Automated workflows minimize manual touchpoints</p>
      </div>
      <div class="ap-auto-card ap-reveal">
        <span class="ap-auto-icon">🔍</span>
        <h4>Improved Duplicate Detection</h4>
        <p>AI flags duplicate invoices before processing</p>
      </div>
      <div class="ap-auto-card ap-reveal">
        <span class="ap-auto-icon">✓</span>
        <h4>Real-Time Approval Workflows</h4>
        <p>Dynamic routing ensures timely approvals</p>
      </div>
      <div class="ap-auto-card ap-reveal">
        <span class="ap-auto-icon">📋</span>
        <h4>Enhanced Audit Trails</h4>
        <p>Complete digital records for compliance</p>
      </div>
      <div class="ap-auto-card ap-reveal">
        <span class="ap-auto-icon">📊</span>
        <h4>Advanced Analytics</h4>
        <p>Real-time dashboards for AP insights</p>
      </div>
    </div>
  </div>
</div>

<!-- COST & SCALABILITY -->
<div class="ap-section">
  <div class="ap-inner">
    <span class="ap-label">Cost Reduction & Scalability</span>
    <h2 class="ap-title">Flexible AP Support That Scales</h2>
    <div class="ap-split">
      <div class="ap-split-text ap-reveal">
        <p>One of the biggest advantages of accounts payable outsourcing is <strong>operational flexibility.</strong> Instead of hiring and training in-house staff, companies can scale AP support based on invoice volume.</p>
        <p>Additionally, outsourcing helps businesses reduce operational burden while maintaining consistent quality throughout seasonal fluctuations and business growth cycles.</p>
        <p>To explore more benefits, read <a href="https://infinity-logisticsbackoffice.com/the-advantages-of-outsourcing-accounts-payable/" class="ap-link">the advantages of outsourcing accounts payable</a>.</p>
      </div>
      <div class="ap-reveal">
        <ul class="ap-split-list">
          <li>Lower overhead and staffing costs</li>
          <li>Eliminate technology investment burden</li>
          <li>Improve turnaround time significantly</li>
          <li>Support seasonal volume spikes easily</li>
          <li>Maintain consistent processing quality</li>
          <li>Access specialized finance expertise</li>
          <li>Reduce training and onboarding time</li>
          <li>Gain flexible capacity management</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<!-- INDUSTRIES -->
<div class="ap-section-alt">
  <div class="ap-inner">
    <span class="ap-label">Industries We Support</span>
    <h2 class="ap-title">Specialized for Logistics Operations</h2>
    <p class="ap-lead ap-reveal">Our accounts payable outsourcing solutions are specifically designed for logistics-focused organizations. Because each sector has unique billing and documentation requirements, our workflows are customized to match your operational environment.</p>
    <div class="ap-industries-grid ap-reveal">
      <div class="ap-industry-tag">🚛 Freight Forwarders</div>
      <div class="ap-industry-tag">🏭 3PL Providers</div>
      <div class="ap-industry-tag">🚐 Trucking Companies</div>
      <div class="ap-industry-tag">🚢 NVOCC Operators</div>
      <div class="ap-industry-tag">💳 Freight Payment Firms</div>
      <div class="ap-industry-tag">📦 Custom House Brokers</div>
    </div>
  </div>
</div>

<!-- WHY CHOOSE -->
<div class="ap-section">
  <div class="ap-inner">
    <span class="ap-label">Why Choose Infinity IPS</span>
    <h2 class="ap-title">Logistics Domain Expertise + Finance Automation</h2>
    <p class="ap-lead ap-reveal">Infinity IPS combines logistics domain expertise with advanced finance automation to deliver reliable AP outsourcing services. Furthermore, our structured quality controls, secure data handling, and scalable delivery model ensure consistent performance.</p>
    <div class="ap-why-grid">
      <div class="ap-why-card ap-reveal">
        <span class="ap-why-icon">📈</span>
        <h4>Higher Invoice Accuracy</h4>
      </div>
      <div class="ap-why-card ap-reveal">
        <span class="ap-why-icon">⏱️</span>
        <h4>Faster Payment Cycles</h4>
      </div>
      <div class="ap-why-card ap-reveal">
        <span class="ap-why-icon">🤝</span>
        <h4>Stronger Vendor Relationships</h4>
      </div>
      <div class="ap-why-card ap-reveal">
        <span class="ap-why-icon">👁️</span>
        <h4>Improved Financial Visibility</h4>
      </div>
      <div class="ap-why-card ap-reveal">
        <span class="ap-why-icon">🛡️</span>
        <h4>Reduced Operational Risk</h4>
      </div>
      <div class="ap-why-card ap-reveal">
        <span class="ap-why-icon">📊</span>
        <h4>Real-Time Reporting & Analytics</h4>
      </div>
    </div>
  </div>
</div>

<!-- CTA -->
<div class="ap-cta">
  <div class="ap-cta-inner">
    <span class="ap-label" style="display:block; text-align:center; margin-bottom:0.75rem;">Get Started</span>
    <h2 class="ap-title">Ready to Streamline Your AP Operations?</h2>
    <p class="ap-lead">As invoice volumes grow and financial processes become more complex, outsourcing accounts payable becomes a smart strategic move. Infinity IPS helps logistics companies modernize AP workflows, improve control, and scale efficiently—without increasing internal workload.</p>
    <a href="https://infinity-logisticsbackoffice.com/contact-us/" class="ap-btn">Contact Us Today →</a>
  </div>
</div>

<!-- FOOTER -->
<div class="ap-footer">
  <p>© 2026 <a href="https://infinity-logisticsbackoffice.com">Infinity IPS</a> — Your Logistics Back Office Partner. All rights reserved.</p>
</div>

<script>
  const reveals = document.querySelectorAll('.ap-reveal');
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible');
        observer.unobserve(entry.target);
      }
    });
  }, { threshold: 0.08, rootMargin: '0px 0px -30px 0px' });
  reveals.forEach(el => observer.observe(el));
</script>
</body>
</html>
