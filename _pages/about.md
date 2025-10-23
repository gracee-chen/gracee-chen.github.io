---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<div id="tab-container">
  <!-- Tab Navigation -->
  <div class="tab-navigation">
    <button class="tab-button active" onclick="showTab('about-me')">About Me</button>
    <button class="tab-button" onclick="showTab('research-experience')">Research Experience</button>
    <button class="tab-button" onclick="showTab('work-experience')">Work Experience</button>
    <button class="tab-button" onclick="showTab('skills')">Skills</button>
  </div>

  <!-- Tab Content -->
  <div id="about-me" class="tab-content active">
    <span class='anchor' id='about-me'></span>
    
    I am an undergraduate student majoring in Mathematics and Computer Science at New York University, and an incoming Master of Science student in Data Science at Harvard University (September 2025). My research interests focus on artificial intelligence, computer vision, and medical image analysis. Currently, I work as a research assistant at the AI4CE Lab at NYU Tandon and the Radiology Research Department at NYU Langone Health, where I contribute to projects in 3D reconstruction, assembly, and medical imaging analysis.

    <h2>🔥 News</h2>
    <ul>
      <li><em>2025.02</em>: &nbsp;🎉🎉 Accepted to Harvard University's Master of Science program in Data Science!</li>
    </ul>

    <h2>📝 Publications</h2>
    <div class='paper-box'>
      <div class='paper-box-image'>
        <div>
          <div class="badge">Arxiv 2025</div>
          <img src='images/GARF.gif' alt="sym" width="100%">
        </div>
      </div>
      <div class='paper-box-text' markdown="1">
        [GARF: Learning Generalizable 3D Reassembly for Real-World Fractures](https://ai4ce.github.io/GARF/)
        <br><br>
        Chen Feng, **Grace Chen**, et al. [**Project**](https://arxiv.org/abs/2504.05400) <strong><span class='show_paper_citations' data='DhtAFkwAAAAJ:ALROH1vI_8AC'></span></strong>
      </div>
    </div>

    <h2>📖 Education</h2>
    <ul>
      <li><em>2025.09 - 2026.12 (incoming)</em>, Master of Science in Data Science, Harvard University</li>
      <li><em>2022.09 - 2025.05</em>, Bachelor of Art in Mathematics and Computer Science, New York University</li>
    </ul>
  </div>

  <div id="research-experience" class="tab-content">
    <span class='anchor' id='research-experience'></span>
    
    <h2>💻 Research Experience</h2>
    
    <h3>AI4CE Lab, NYU Tandon</h3>
    <p><em>2024.08 - Present</em> (supervised by Prof. Chen Feng)</p>
    <ul>
      <li>3D Assembly Project: Contributed to GARF model for generalizable 3D reassembly</li>
      <li>3D Reconstruction Project: Implemented Dust3R geometric 3D vision model for archaeological fragment reconstruction</li>
    </ul>

    <h3>NYU Langone Health, Radiology Research Department</h3>
    <p><em>2024.02 - Present</em> (supervised by Dr. Yiqiu Shen)</p>
    <ul>
      <li>Pancreatic Cancer Project: Processed data for 1200+ patients, used LLMs to analyze radiology reports</li>
      <li>Breast Cancer Project: Conducted statistical analysis on radiology reports using Cohen's Kappa hypothesis test, improved GPT training prompt template for BI-RADS score ratings by 10%</li>
    </ul>

    <h3>Chongqing University of Technology</h3>
    <p><em>2023.11 - Present</em> (supervised by Prof. Dongyang Qiu)</p>
    <ul>
      <li>Implemented machine learning algorithms for financial risk early warning models</li>
      <li>Developed data preprocessing tools, reducing processing time by 15%</li>
    </ul>

    <h3>NYU Savin's Lab</h3>
    <p><em>2023.11 - 2024.05</em> (supervised by Prof. Cristina Savin)</p>
    <ul>
      <li>Conducted research on dimensionality reduction and Gaussian Models for data analysis</li>
    </ul>
  </div>

  <div id="work-experience" class="tab-content">
    <span class='anchor' id='work-experience'></span>
    
    <h2>💼 Professional Experience</h2>
    
    <h3>Guotai Jun'an Securities</h3>
    <p><em>2023.05 - 2023.07</em>, Investment Banking Intern, Shanghai, China</p>
    <ul>
      <li>Developed project proposals focused on market research and financial assessments</li>
      <li>Contributed to 10+ high-profile roadshows for client company offerings (project resulted in successful IPO)</li>
      <li>Produced financial offering-related documents including due diligence and client interviews</li>
    </ul>

    <h2>💬 Teaching Experience</h2>
    
    <h3>Courant Institute of Mathematical Sciences</h3>
    <p><em>2024.02 - Present</em>, Teaching Assistant for Linear Algebra and Calculus III</p>
    <ul>
      <li>Provided one-on-one tutoring and detailed feedback, and graded assignments for classes of 50+ students</li>
    </ul>
  </div>

  <div id="skills" class="tab-content">
    <span class='anchor' id='skills'></span>
    
    <h2>🛠 Skills</h2>
    
    <h3>Technical Proficiency</h3>
    <p>R, Java, Python, C, SPSS Statistics, SQL, CSS, HTML, GIS</p>
    
    <h3>Languages</h3>
    <p>Mandarin Chinese (Native), English (Fluent)</p>
  </div>
</div>

<style>
.tab-navigation {
  display: flex;
  border-bottom: 2px solid #e1e4e8;
  margin-bottom: 2rem;
}

.tab-button {
  background: none;
  border: none;
  padding: 12px 24px;
  cursor: pointer;
  font-size: 16px;
  color: #586069;
  border-bottom: 2px solid transparent;
  transition: all 0.3s ease;
}

.tab-button:hover {
  color: #0366d6;
  background-color: #f6f8fa;
}

.tab-button.active {
  color: #0366d6;
  border-bottom-color: #0366d6;
  font-weight: 600;
}

.tab-content {
  display: none;
  animation: fadeIn 0.3s ease-in;
}

.tab-content.active {
  display: block;
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}

.paper-box {
  display: flex;
  justify-content: left;
  align-items: center;
  flex-direction: row;
  flex-wrap: wrap;
  border-bottom: 1px #efefef solid;
  padding: 2em 0 2em 0;
}

.paper-box-image {
  justify-content: center;
  display: flex;
  width: 100%;
  order: 2;
}

.paper-box-image img {
  max-width: 400px;
  box-shadow: 3px 3px 6px #888;
  object-fit: cover;
}

.paper-box-text {
  max-width: 100%;
  order: 1;
}

@media (min-width: 768px) {
  .paper-box-image {
    justify-content: left;
    min-width: 200px;
    max-width: 40%;
    order: 1;
  }
  
  .paper-box-text {
    justify-content: left;
    padding-left: 2em;
    max-width: 60%;
    order: 2;
  }
}

.badge {
  padding-left: 1rem;
  padding-right: 1rem;
  position: absolute;
  margin-top: .5em;
  margin-left: -.5em;
  color: white;
  background-color: #00369f;
  font-size: .8em;
}
</style>

<script>
function showTab(tabId) {
  // Hide all tab contents
  const contents = document.querySelectorAll('.tab-content');
  contents.forEach(content => {
    content.classList.remove('active');
  });
  
  // Remove active class from all buttons
  const buttons = document.querySelectorAll('.tab-button');
  buttons.forEach(button => {
    button.classList.remove('active');
  });
  
  // Show selected tab content
  document.getElementById(tabId).classList.add('active');
  
  // Add active class to clicked button
  event.target.classList.add('active');
}

// Handle URL hash navigation
window.addEventListener('load', function() {
  const hash = window.location.hash.substring(1);
  if (hash && document.getElementById(hash)) {
    showTab(hash);
  }
});

// Handle browser back/forward buttons
window.addEventListener('hashchange', function() {
  const hash = window.location.hash.substring(1);
  if (hash && document.getElementById(hash)) {
    showTab(hash);
  }
});
</script>
