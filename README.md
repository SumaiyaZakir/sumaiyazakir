<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Sumaiya Zakir | Geospatial &amp; Environmental Researcher</title>
  
  <!-- Standard Academic & Professional Google Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Plus+Jakarta+Sans:wght@600;700;800&display=swap" rel="stylesheet">

  <!-- ========================================================================== -->
  <!--                              CSS STYLES                                    -->
  <!-- ========================================================================== -->
  <style>
    :root {
      --bg-main: #f8fafc;
      --bg-card: #ffffff;
      --border-color: #e2e8f0;
      --border-hover: #cbd5e1;
      --primary: #0f4c5c;
      --primary-accent: #0284c7;
      --primary-light: #f0f9ff;
      --accent-emerald: #059669;
      --accent-emerald-light: #ecfdf5;
      --text-dark: #0f172a;
      --text-body: #334155;
      --text-muted: #64748b;
      --max-width: 1140px;
      --shadow-sm: 0 1px 3px rgba(0, 0, 0, 0.05);
      --shadow-md: 0 4px 12px -2px rgba(0, 0, 0, 0.06);
      --radius-sm: 6px;
      --radius-md: 10px;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
      background-color: var(--bg-main);
      color: var(--text-body);
      line-height: 1.65;
    }

    h1, h2, h3, h4, .brand-font {
      font-family: 'Plus Jakarta Sans', sans-serif;
      color: var(--text-dark);
    }

    a {
      color: var(--primary-accent);
      text-decoration: none;
      transition: all 0.2s ease;
    }

    a:hover {
      color: var(--primary);
    }

    /* Top Navigation Bar */
    header {
      position: sticky;
      top: 0;
      width: 100%;
      background: rgba(255, 255, 255, 0.96);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid var(--border-color);
      z-index: 1000;
    }

    nav {
      max-width: var(--max-width);
      margin: 0 auto;
      padding: 1.1rem 1.75rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 1rem;
    }

    .nav-brand {
      font-size: 1.15rem;
      font-weight: 700;
      color: var(--primary);
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }

    .nav-brand:hover {
      color: var(--primary-accent);
    }

    .nav-links {
      display: flex;
      list-style: none;
      gap: 1.3rem;
      align-items: center;
      flex-wrap: wrap;
    }

    .nav-links a {
      font-size: 0.9rem;
      font-weight: 500;
      color: var(--text-muted);
    }

    .nav-links a:hover {
      color: var(--primary);
    }

    /* Main Container & Sections */
    main {
      max-width: var(--max-width);
      margin: 0 auto;
      padding: 0 1.75rem 4rem;
    }

    section {
      padding: 4.5rem 0 2.5rem;
      border-bottom: 1px solid var(--border-color);
    }

    section:last-of-type {
      border-bottom: none;
    }

    .section-header {
      margin-bottom: 2rem;
    }

    .section-tag {
      text-transform: uppercase;
      font-size: 0.75rem;
      font-weight: 700;
      letter-spacing: 0.08em;
      color: var(--primary-accent);
      margin-bottom: 0.35rem;
      display: block;
    }

    .section-title {
      font-size: 1.85rem;
      font-weight: 700;
      letter-spacing: -0.02em;
    }

    /* Hero Section */
    #home {
      padding: 4.5rem 0 3rem;
    }

    .hero-grid {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 3.5rem;
      flex-wrap: wrap-reverse;
    }

    .hero-content {
      flex: 1 1 560px;
    }

    .role-badge {
      display: inline-block;
      padding: 0.35rem 0.85rem;
      background-color: var(--primary-light);
      border: 1px solid #bae6fd;
      border-radius: 9999px;
      font-size: 0.85rem;
      font-weight: 600;
      color: var(--primary);
      margin-bottom: 1.25rem;
    }

    .hero-name {
      font-size: 2.8rem;
      font-weight: 800;
      letter-spacing: -0.025em;
      line-height: 1.2;
      margin-bottom: 0.5rem;
    }

    .hero-subtitle {
      font-size: 1.25rem;
      font-weight: 600;
      color: var(--primary-accent);
      margin-bottom: 1.25rem;
    }

    .hero-desc {
      font-size: 1.05rem;
      color: var(--text-body);
      line-height: 1.7;
      margin-bottom: 1.5rem;
    }

    /* Research Interests Box */
    .research-interest-box {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-left: 4px solid var(--primary-accent);
      border-radius: var(--radius-sm);
      padding: 1.15rem 1.35rem;
      margin-bottom: 1.75rem;
      box-shadow: var(--shadow-sm);
    }

    .research-interest-title {
      font-size: 0.88rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.05em;
      color: var(--primary);
      margin-bottom: 0.75rem;
      display: flex;
      align-items: center;
      gap: 0.4rem;
    }

    .interest-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
    }

    .interest-tag {
      background: #f1f5f9;
      color: #1e293b;
      border: 1px solid #e2e8f0;
      padding: 0.35rem 0.75rem;
      border-radius: 6px;
      font-size: 0.84rem;
      font-weight: 500;
      transition: all 0.2s ease;
    }

    .interest-tag:hover {
      background: var(--primary-light);
      border-color: #bae6fd;
      color: var(--primary-accent);
    }

    /* Action Buttons */
    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 0.85rem;
      align-items: center;
      margin-bottom: 1.75rem;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.7rem 1.4rem;
      font-size: 0.92rem;
      font-weight: 600;
      border-radius: var(--radius-sm);
      cursor: pointer;
      transition: all 0.2s ease;
    }

    .btn-primary {
      background-color: var(--primary);
      color: #ffffff;
      border: 1px solid var(--primary);
    }

    .btn-primary:hover {
      background-color: #0b3742;
      color: #ffffff;
      transform: translateY(-1px);
    }

    .btn-secondary {
      background-color: #ffffff;
      color: var(--text-dark);
      border: 1px solid var(--border-color);
    }

    .btn-secondary:hover {
      border-color: var(--primary-accent);
      color: var(--primary-accent);
      transform: translateY(-1px);
    }

    /* Hero Socials */
    .hero-socials {
      display: flex;
      gap: 1.5rem;
      align-items: center;
      flex-wrap: wrap;
    }

    .social-link {
      display: inline-flex;
      align-items: center;
      gap: 0.35rem;
      font-size: 0.9rem;
      font-weight: 600;
      color: var(--text-muted);
    }

    .social-link:hover {
      color: var(--primary-accent);
    }

    /* Profile Photo Area */
    .hero-photo-container {
      flex: 0 0 260px;
      display: flex;
      justify-content: center;
    }

    .photo-frame {
      width: 250px;
      height: 250px;
      border-radius: var(--radius-md);
      border: 2px solid var(--border-color);
      box-shadow: var(--shadow-md);
      overflow: hidden;
      background-color: #e2e8f0;
    }

    .photo-frame img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block;
    }

    /* Education & Awards Grid */
    .education-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      gap: 1.5rem;
      margin-bottom: 2rem;
    }

    .edu-card {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-md);
      overflow: hidden;
      box-shadow: var(--shadow-sm);
      display: flex;
      flex-direction: column;
      padding: 1.5rem;
      transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
    }

    .edu-card:hover {
      transform: translateY(-3px);
      box-shadow: var(--shadow-md);
      border-color: var(--border-hover);
    }

    .edu-year {
      font-size: 0.82rem;
      font-weight: 700;
      color: var(--primary-accent);
      margin-bottom: 0.35rem;
    }

    .edu-degree {
      font-size: 1.15rem;
      font-weight: 700;
      color: var(--text-dark);
      line-height: 1.35;
      margin-bottom: 0.35rem;
    }

    .edu-institution {
      font-size: 0.95rem;
      color: var(--text-muted);
      margin-bottom: 1.15rem;
      font-weight: 500;
    }

    .edu-details {
      margin-top: auto;
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
    }

    .edu-badge {
      font-size: 0.82rem;
      padding: 0.3rem 0.65rem;
      border-radius: 4px;
      background: #f1f5f9;
      color: #334155;
      border: 1px solid #e2e8f0;
      font-weight: 500;
    }

    .edu-badge-result {
      background: var(--accent-emerald-light);
      border-color: #a7f3d0;
      color: #065f46;
    }

    /* Awards Strip */
    .award-card {
      background: #f0fdf4;
      border: 1px solid #bbf7d0;
      border-left: 4px solid var(--accent-emerald);
      border-radius: var(--radius-md);
      padding: 1.25rem 1.5rem;
      margin-top: 1rem;
    }

    .award-title {
      font-size: 0.95rem;
      font-weight: 700;
      color: #065f46;
      margin-bottom: 0.5rem;
      display: flex;
      align-items: center;
      gap: 0.4rem;
    }

    .award-list {
      list-style-type: none;
      display: flex;
      flex-direction: column;
      gap: 0.45rem;
    }

    .award-list li {
      font-size: 0.92rem;
      color: #1e293b;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }

    /* General Cards & Grid System */
    .card {
      background: var(--bg-card);
      border: 1px solid var(--border-color);
      border-radius: var(--radius-md);
      padding: 1.6rem;
      margin-bottom: 1.25rem;
      box-shadow: var(--shadow-sm);
      transition: border-color 0.2s ease, box-shadow 0.2s ease;
    }

    .card:hover {
      border-color: var(--border-hover);
      box-shadow: var(--shadow-md);
    }

    .grid-2 {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      gap: 1.25rem;
    }

    .grid-3 {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1.25rem;
    }

    .card-meta {
      font-size: 0.82rem;
      font-weight: 600;
      color: var(--primary-accent);
      margin-bottom: 0.4rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 0.5rem;
    }

    .card-badge {
      display: inline-block;
      padding: 0.2rem 0.55rem;
      font-size: 0.75rem;
      font-weight: 700;
      border-radius: 4px;
      background: #eff6ff;
      color: #1d4ed8;
      border: 1px solid #bfdbfe;
    }

    .card-badge.accepted {
      background: #ecfdf5;
      color: #047857;
      border-color: #a7f3d0;
    }

    .card-title {
      font-size: 1.15rem;
      font-weight: 700;
      margin-bottom: 0.65rem;
      line-height: 1.4;
    }

    .card-text {
      color: var(--text-body);
      font-size: 0.94rem;
      line-height: 1.65;
      margin-bottom: 0.75rem;
    }

    .card-list {
      padding-left: 1.2rem;
      font-size: 0.92rem;
      color: var(--text-body);
      display: flex;
      flex-direction: column;
      gap: 0.4rem;
    }

    /* Skills Badges */
    .skill-category-title {
      font-size: 1.05rem;
      font-weight: 700;
      color: var(--primary);
      margin-bottom: 0.85rem;
      display: flex;
      align-items: center;
      gap: 0.4rem;
    }

    .skill-pills {
      display: flex;
      flex-wrap: wrap;
      gap: 0.45rem;
    }

    .skill-pill {
      background: #f8fafc;
      border: 1px solid var(--border-color);
      padding: 0.35rem 0.7rem;
      border-radius: 6px;
      font-size: 0.85rem;
      font-weight: 500;
      color: #334155;
    }

    /* Contact Details */
    .contact-row {
      display: flex;
      align-items: flex-start;
      gap: 1rem;
      margin-bottom: 1.25rem;
    }

    .contact-row:last-child {
      margin-bottom: 0;
    }

    .contact-icon {
      width: 40px;
      height: 40px;
      border-radius: var(--radius-sm);
      background-color: var(--primary-light);
      color: var(--primary);
      display: flex;
      align-items: center;
      justify-content: center;
      flex-shrink: 0;
    }

    .contact-label {
      font-size: 0.78rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.05em;
      color: var(--text-muted);
    }

    .contact-value {
      font-size: 0.95rem;
      font-weight: 600;
      color: var(--text-dark);
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 2.5rem 1.5rem;
      border-top: 1px solid var(--border-color);
      color: var(--text-muted);
      font-size: 0.88rem;
      background-color: #ffffff;
    }

    @media (max-width: 768px) {
      .hero-name {
        font-size: 2.2rem;
      }
      .hero-photo-container {
        margin: 0 auto;
      }
      .nav-links {
        gap: 0.85rem;
      }
    }
  </style>
</head>
<body>

  <!-- ========================================================================== -->
  <!--                            TOP NAVIGATION BAR                              -->
  <!-- ========================================================================== -->
  <header>
    <nav>
      <a href="#home" class="nav-brand">
        Sumaiya Zakir
      </a>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">Education</a></li>
        <li><a href="#publications">Publications</a></li>
        <li><a href="#research-projects">Research &amp; Dissertations</a></li>
        <li><a href="#experience">Experience</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main>

    <!-- ========================================================================== -->
    <!--                          SECTION 1: HOME (HERO)                            -->
    <!-- ========================================================================== -->
    <section id="home">
      <div class="hero-grid">
        <div class="hero-content">
          <div class="role-badge">Geospatial &bull; Climate Resilience &bull; Remote Sensing</div>
          
          <h1 class="hero-name">Sumaiya Zakir</h1>
          <h2 class="hero-subtitle">Geospatial Analyst &amp; Environmental Researcher</h2>

          <p class="hero-desc">
            Specializing in geospatial analysis, satellite remote sensing, ecological modeling, and machine learning for climate resilience and environmental management. Experienced in master plan preparation, spatiotemporal ecological dynamics, and air quality assessment using Google Earth Engine and ArcGIS Pro.
          </p>

          <!-- Research Interests Box -->
          <div class="research-interest-box">
            <div class="research-interest-title">
              <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M19.428 15.428a2 2 0 00-1.022-.547l-2.387-.477a6 6 0 00-3.86.517l-.318.158a6 6 0 01-3.86.517L6.05 15.21a2 2 0 00-1.806.547M8 4h8l-1 1v5.172a2 2 0 00.586 1.414l5 5c1.26 1.26.367 3.414-1.415 3.414H4.828c-1.782 0-2.674-2.154-1.414-3.414l5-5A2 2 0 009 10.172V5L8 4z"/></svg>
              <span>Research Interests</span>
            </div>
            <div class="interest-tags">
              <span class="interest-tag">Climate &amp; Disaster Resilience</span>
              <span class="interest-tag">Spatial Analysis &amp; Environmental Modelling</span>
              <span class="interest-tag">Urban Environmental Management</span>
              <span class="interest-tag">Biodiversity &amp; Nature Conservation</span>
              <span class="interest-tag">Satellite Remote Sensing</span>
              <span class="interest-tag">Geospatial Machine Learning</span>
            </div>
          </div>

          <!-- Action Buttons -->
          <div class="hero-actions">
            <a href="https://drive.google.com" target="_blank" class="btn btn-primary">
              <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M12 10v6m0 0l-3-3m3 3l3-3m2 8H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"/></svg>
              <span>Download CV</span>
            </a>
            <a href="#publications" class="btn btn-secondary">Publications</a>
            <a href="#contact" class="btn btn-secondary">Contact Me</a>
          </div>

          <!-- Active Social & Profile Links -->
          <div class="hero-socials">
            <a href="https://linkedin.com" target="_blank" rel="noopener noreferrer" class="social-link">
              <svg width="16" height="16" fill="currentColor" viewBox="0 0 24 24"><path d="M19 3a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h14m-.5 15.5v-5.3a3.26 3.26 0 0 0-3.26-3.26c-.85 0-1.84.52-2.28 1.3v-1.11h-2.79v8.37h2.79v-4.93c0-.77.62-1.4 1.39-1.4a1.4 1.4 0 0 1 1.4 1.4v4.93h2.75M6.46 10.9v8.37H9.2V10.9H6.46M7.83 6.45a1.65 1.65 0 0 0-1.66 1.66 1.66 1.66 0 0 0 1.66 1.65 1.65 1.65 0 0 0 1.65-1.65c0-.92-.74-1.66-1.65-1.66Z"/></svg>
              <span>LinkedIn</span>
            </a>
            <a href="mailto:your-email@gmail.com" class="social-link">
              <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/></svg>
              <span>Gmail</span>
            </a>
            <a href="#contact" class="social-link">
              <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/><path stroke-linecap="round" stroke-linejoin="round" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/></svg>
              <span>Dhaka, Bangladesh</span>
            </a>
          </div>
        </div>

        <!-- Profile Photo Area -->
        <div class="hero-photo-container">
          <div class="photo-frame">
            <img 
              src="profile.jpg" 
              alt="Sumaiya Zakir" 
              onerror="this.onerror=null; this.src='data:image/svg+xml;utf8,<svg xmlns=\'http://www.w3.org/2000/svg\' width=\'250\' height=\'250\' viewBox=\'0 0 250 250\'><rect fill=\'%23e2e8f0\' width=\'250\' height=\'250\'/><text fill=\'%230f4c5c\' font-family=\'sans-serif\' font-size=\'15\' font-weight=\'700\' x=\'50%25\' y=\'50%25\' text-anchor=\'middle\' dominant-baseline=\'middle\'>Sumaiya Zakir</text></svg>';" 
            />
          </div>
        </div>
      </div>
    </section>

    <!-- ========================================================================== -->
    <!--                   SECTION 2: ABOUT (EDUCATION & AWARDS)                    -->
    <!-- ========================================================================== -->
    <section id="about">
      <div class="section-header">
        <span class="section-tag">Academic Background</span>
        <h2 class="section-title">Education &amp; Honors</h2>
      </div>

      <div class="education-grid">
        <!-- 1. Master of Science -->
        <div class="edu-card">
          <div class="edu-year">Nov 2022 &ndash; March 2024</div>
          <h3 class="edu-degree">Master of Science in Geography and Environment</h3>
          <p class="edu-institution">Jahangirnagar University, Bangladesh</p>
          <div class="edu-details">
            <div class="edu-badge edu-badge-result">
              <span>Result:</span> <strong>CGPA 3.78 / 4.00</strong>
            </div>
            <div class="edu-badge">
              <span>Specialization:</span> Spatial Analysis &amp; Environmental Modeling
            </div>
          </div>
        </div>

        <!-- 2. Bachelor of Science -->
        <div class="edu-card">
          <div class="edu-year">March 2017 &ndash; Feb 2023</div>
          <h3 class="edu-degree">Bachelor of Science in Geography and Environment</h3>
          <p class="edu-institution">Jahangirnagar University, Bangladesh</p>
          <div class="edu-details">
            <div class="edu-badge edu-badge-result">
              <span>Result:</span> <strong>CGPA 3.51 / 4.00</strong>
            </div>
            <div class="edu-badge">
              <span>Focus:</span> Environmental Remote Sensing &amp; GIS
            </div>
          </div>
        </div>
      </div>

      <!-- Academic Honors & Awards -->
      <div class="award-card">
        <div class="award-title">
          <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 12l2 2 4-4M7.835 4.697a3.42 3.42 0 001.946-.806 3.42 3.42 0 014.438 0 3.42 3.42 0 001.946.806 3.42 3.42 0 013.138 3.138 3.42 3.42 0 00.806 1.946 3.42 3.42 0 010 4.438 3.42 3.42 0 00-.806 1.946 3.42 3.42 0 01-3.138 3.138 3.42 3.42 0 00-1.946.806 3.42 3.42 0 01-4.438 0 3.42 3.42 0 00-1.946-.806 3.42 3.42 0 01-3.138-3.138 3.42 3.42 0 00-.806-1.946 3.42 3.42 0 010-4.438 3.42 3.42 0 00.806-1.946 3.42 3.42 0 013.138-3.138z"/></svg>
          <span>Honors &amp; Awards</span>
        </div>
        <ul class="award-list">
          <li><strong>National Science and Technology (NST) Research Fellowship</strong> &ndash; Ministry of Science and Technology, Bangladesh</li>
          <li><strong>The Duke of Edinburgh's International Award (Direct Gold)</strong> &ndash; Recognized for leadership, community service, and environmental expeditions</li>
        </ul>
      </div>
    </section>

    <!-- ========================================================================== -->
    <!--                         SECTION 3: PUBLICATIONS                            -->
    <!-- ========================================================================== -->
    <section id="publications">
      <div class="section-header">
        <span class="section-tag">Peer-Reviewed Research</span>
        <h2 class="section-title">Publications &amp; Manuscripts</h2>
      </div>
      <div class="grid-2">
        <!-- Publication 1 -->
        <div class="card">
          <div class="card-meta">
            <span>Environmental Sciences Europe (Q1 Journal)</span>
            <span class="card-badge accepted">1st Author &bull; Accepted</span>
          </div>
          <h3 class="card-title">Spatiotemporal land use changes shaping biodiversity dynamics in southeastern regions of Bangladesh: A multi-scale geospatial and ecological analysis</h3>
          <ul class="card-list">
            <li>Applied multi-temporal Landsat classification with MOLUSCE CA-ANN modeling to simulate and predict LULC shifts through 2050.</li>
            <li>Integrated FRAGSTATS fragmentation metrics, InVEST habitat-quality modeling, and species-richness overlays to evaluate biodiversity risk.</li>
          </ul>
        </div>

        <!-- Publication 2 -->
        <div class="card">
          <div class="card-meta">
            <span>Springer Nature (Book Chapter, Scopus Indexed)</span>
            <span class="card-badge accepted">Co-Author &bull; In Press</span>
          </div>
          <h3 class="card-title">Spatiotemporal Assessment of Cyclone-Induced Canopy Loss and Regeneration Dynamics in the Bangladesh Sundarbans</h3>
          <ul class="card-list">
            <li>Evaluated multi-temporal Landsat imagery across 5km cyclone corridors to quantify canopy loss and mangrove vegetation recovery trajectories.</li>
            <li>Applied Kruskal-Wallis and Dunn's post-hoc tests, demonstrating EVI as the most sensitive disturbance and recovery indicator.</li>
          </ul>
        </div>

        <!-- Publication 3 -->
        <div class="card" style="grid-column: 1 / -1;">
          <div class="card-meta">
            <span>Target Q1 Journal</span>
            <span class="card-badge">Co-Author &bull; In Preparation</span>
          </div>
          <h3 class="card-title">Machine Learning-driven Multifactor Water Quality Indexing for Aquaculture Site Suitability Assessment: A Case Study in Khulna Division, Bangladesh</h3>
          <ul class="card-list">
            <li>Evaluated Machine Learning algorithms modeling satellite covariates with in-situ physicochemical parameters (TDS, EC, pH, SG, Salinity, DO, NO2, NO3) from 100 survey points.</li>
            <li>Constructed an Aquaculture Site Suitability Index combining ML raster predictions, IDW spatial interpolation, and Analytic Hierarchy Process (AHP) weighting.</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- ========================================================================== -->
    <!--            SECTION 4: RESEARCH PROJECTS & DISSERTATIONS                    -->
    <!-- ========================================================================== -->
    <section id="research-projects">
      <div class="section-header">
        <span class="section-tag">Academic Research</span>
        <h2 class="section-title">Dissertations &amp; Conference Presentations</h2>
      </div>
      <div class="grid-3">
        <!-- MSc Thesis -->
        <div class="card">
          <div class="card-meta">Master's Dissertation &bull; GEE</div>
          <h3 class="card-title">Air Quality Index Analysis in Google Earth Engine</h3>
          <p class="card-text">Assessed Pre-, During-, and Post-COVID-19 periods in Dhaka City using JavaScript-based GEE pipelines mapping Sentinel-5P NO2, SO2, and CO concentrations.</p>
        </div>

        <!-- Conference Presentation -->
        <div class="card">
          <div class="card-meta">1st South Asian Climate Conference</div>
          <h3 class="card-title">Time Series Assessment of PM2.5 via Linear Regression</h3>
          <p class="card-text">Modeled PM2.5 trends for Dhaka North City Corporation using IBM SPSS regression and generated spatial variation maps using ArcGIS IDW interpolation.</p>
        </div>

        <!-- BSc Thesis -->
        <div class="card">
          <div class="card-meta">Bachelor's Dissertation &bull; ArcGIS</div>
          <h3 class="card-title">Analysis of Air Pollution in Dhaka City (PM2.5 &amp; PM10)</h3>
          <p class="card-text">Processed monitoring station data using SPSS and ArcGIS to examine annual variations, seasonal trends, weekday-weekend differences, and spatial dispersion.</p>
        </div>
      </div>
    </section>

    <!-- ========================================================================== -->
    <!--                     SECTION 5: PROFESSIONAL EXPERIENCE                     -->
    <!-- ========================================================================== -->
    <section id="experience">
      <div class="section-header">
        <span class="section-tag">Career History</span>
        <h2 class="section-title">Professional Experience</h2>
      </div>
      
      <!-- Experience 1 -->
      <div class="card">
        <div class="card-meta">
          <span>Sheltech Consultancy Pvt. Ltd., Dhaka</span>
          <span>Jan 2024 &ndash; Mar 2026</span>
        </div>
        <h3 class="card-title">Assistant GIS Specialist</h3>
        <p class="card-text">
          Conducted GIS spatial database management, remote sensing, satellite image analysis, mapping, digitization, topographic surveying, and geospatial data processing for the preparation of 20-year master plans across 20 upazilas in Bangladesh.
        </p>
      </div>

      <!-- Experience 2 -->
      <div class="card">
        <div class="card-meta">
          <span>Center for People and Environ (CPE)</span>
          <span>Nov 2022 &ndash; April 2023</span>
        </div>
        <h3 class="card-title">Research Assistant</h3>
        <p class="card-text">
          Executed field research, primary data collection, spatial GIS analysis, systematic literature reviews, technical report writing, and stakeholder consultation for environmental and climate-oriented community projects.
        </p>
      </div>

      <!-- Experience 3 -->
      <div class="card">
        <div class="card-meta">
          <span>British Council</span>
          <span>April 2023 &ndash; Oct 2023</span>
        </div>
        <h3 class="card-title">Invigilator</h3>
        <p class="card-text">
          Supervised high-stakes international examinations, upholding examination integrity, testing regulations, and ensuring rigorous, fair, and compliant assessment protocols.
        </p>
      </div>
    </section>

    <!-- ========================================================================== -->
    <!--                   SECTION 6: SKILLS & COMPETENCIES                         -->
    <!-- ========================================================================== -->
    <section id="skills">
      <div class="section-header">
        <span class="section-tag">Technical Competencies</span>
        <h2 class="section-title">Technical Skills &amp; Workshops</h2>
      </div>
      <div class="grid-3">
        <div class="card">
          <div class="skill-category-title">
            <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 20l-5.447-2.724A1 1 0 013 16.382V5.618a1 1 0 011.447-.894L9 7m0 13l6-3m-6 3V7m6 10l4.553 2.276A1 1 0 0021 18.382V7.618a1 1 0 00-.553-.894L15 4m0 13V4m0 0L9 7"/></svg>
            <span>Geospatial Tools</span>
          </div>
          <div class="skill-pills">
            <span class="skill-pill">ArcGIS</span>
            <span class="skill-pill">ArcGIS Pro</span>
            <span class="skill-pill">QGIS</span>
            <span class="skill-pill">Google Earth Engine (GEE)</span>
            <span class="skill-pill">Remote Sensing</span>
            <span class="skill-pill">Spatial Modeling</span>
          </div>
        </div>

        <div class="card">
          <div class="skill-category-title">
            <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4"/></svg>
            <span>Programming &amp; ML</span>
          </div>
          <div class="skill-pills">
            <span class="skill-pill">Python</span>
            <span class="skill-pill">Machine Learning</span>
            <span class="skill-pill">JavaScript (GEE)</span>
            <span class="skill-pill">MOLUSCE (CA-ANN)</span>
            <span class="skill-pill">FRAGSTATS</span>
            <span class="skill-pill">InVEST Habitat Model</span>
          </div>
        </div>

        <div class="card">
          <div class="skill-category-title">
            <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 17v-2m3 2v-4m3 4v-6m2 10H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"/></svg>
            <span>Data &amp; Analytics</span>
          </div>
          <div class="skill-pills">
            <span class="skill-pill">IBM SPSS Statistics</span>
            <span class="skill-pill">MS Excel &amp; Project</span>
            <span class="skill-pill">Adobe Illustrator</span>
            <span class="skill-pill">MS PowerPoint &amp; Word</span>
            <span class="skill-pill">AHP Analysis</span>
          </div>
        </div>
      </div>

      <!-- Workshops & Engagements -->
      <div class="card" style="margin-top: 1.5rem;">
        <h3 class="card-title">Leadership, Workshops &amp; Training</h3>
        <ul class="card-list">
          <li><strong>Youth Action Track &ndash; BDP2100 Conference:</strong> Engaged for seven months with the Youth Action Track organized by ICCCAD, presenting youth climate perspectives at the Netherlands Embassy conference.</li>
          <li><strong>Disaster Management &amp; Environment Safety Workshop:</strong> Completed intensive training at Dhaka University on disaster preparedness, environmental risk assessment, emergency protocols, and climate hazards.</li>
        </ul>
      </div>
    </section>

    <!-- ========================================================================== -->
    <!--                          SECTION 7: CONTACT ME                             -->
    <!-- ========================================================================== -->
    <section id="contact">
      <div class="section-header">
        <span class="section-tag">Get In Touch</span>
        <h2 class="section-title">Contact &amp; References</h2>
      </div>
      <div class="grid-2">
        <div class="card">
          <h3 class="card-title" style="margin-bottom: 1.25rem;">Contact Information</h3>
          
          <div class="contact-row">
            <div class="contact-icon">
              <svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/></svg>
            </div>
            <div>
              <div class="contact-label">Email</div>
              <div class="contact-value">
                <a href="mailto:your-email@gmail.com">Contact via Email</a>
              </div>
            </div>
          </div>

          <div class="contact-row">
            <div class="contact-icon">
              <svg width="20" height="20" fill="currentColor" viewBox="0 0 24 24"><path d="M19 3a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h14m-.5 15.5v-5.3a3.26 3.26 0 0 0-3.26-3.26c-.85 0-1.84.52-2.28 1.3v-1.11h-2.79v8.37h2.79v-4.93c0-.77.62-1.4 1.39-1.4a1.4 1.4 0 0 1 1.4 1.4v4.93h2.75M6.46 10.9v8.37H9.2V10.9H6.46M7.83 6.45a1.65 1.65 0 0 0-1.66 1.66 1.66 1.66 0 0 0 1.66 1.65 1.65 1.65 0 0 0 1.65-1.65c0-.92-.74-1.66-1.65-1.66Z"/></svg>
            </div>
            <div>
              <div class="contact-label">LinkedIn</div>
              <div class="contact-value">
                <a href="https://linkedin.com" target="_blank" rel="noopener noreferrer">Sumaiya Zakir on LinkedIn</a>
              </div>
            </div>
          </div>

          <div class="contact-row">
            <div class="contact-icon">
              <svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/><path stroke-linecap="round" stroke-linejoin="round" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/></svg>
            </div>
            <div>
              <div class="contact-label">Location</div>
              <div class="contact-value">Dhaka, Bangladesh</div>
            </div>
          </div>
        </div>

        <div class="card">
          <h3 class="card-title" style="margin-bottom: 1.25rem;">Academic References</h3>
          <div style="display: flex; flex-direction: column; gap: 1.25rem;">
            <div>
              <h4 style="font-size: 1rem; color: var(--text-dark);">Dr. Mohammad Nayeem Aziz Ansari</h4>
              <p style="font-size: 0.85rem; color: var(--text-muted);">Professor (Research Supervisor)<br>Dept. of Geography and Environment, Jahangirnagar University</p>
              <a href="mailto:ansari@juniv.edu" style="font-size: 0.88rem; font-weight: 500;">ansari@juniv.edu</a>
            </div>
            <div style="border-top: 1px solid var(--border-color); padding-top: 0.75rem;">
              <h4 style="font-size: 1rem; color: var(--text-dark);">Dr. Ummeh Saika</h4>
              <p style="font-size: 0.85rem; color: var(--text-muted);">Associate Professor (Course Instructor)<br>Dept. of Geography and Environment, Jahangirnagar University</p>
              <a href="mailto:usaikau@geography-juniv.edu.bd" style="font-size: 0.88rem; font-weight: 500;">usaikau@geography-juniv.edu.bd</a>
            </div>
          </div>
        </div>
      </div>
    </section>

  </main>

  <!-- ========================================================================== -->
  <!--                             PAGE FOOTER                                    -->
  <!-- ========================================================================== -->
  <footer>
    <p>&copy; <span id="year"></span> Sumaiya Zakir. All rights reserved.</p>
  </footer>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
