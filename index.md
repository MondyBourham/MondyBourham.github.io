---
layout: default
title: Mondy Ayman | QA & Automation Engineer
---

<div class="hero" style="text-align: center; margin: 3rem 0;">
  <h1>Mondy Ayman Ramdan Bourham</h1>
  <p style="font-size: 1.2rem; color: #64748b;">
    🎓 Computer Science Graduate (2024) | 🧪 QA & Automation Engineer | 🚀 CI/CD Advocate
  </p>
  <p>📍 Cairo, Egypt | ✉️ <a href="mailto:bourham2018@gmail.com">bourham2018@gmail.com</a></p>
</div>

## About Me
I’m passionate about ensuring software quality and reliability through **Manual and Automation Testing**. My strength lies in bridging development and QA — building robust test frameworks and integrating them into **CI/CD pipelines** to accelerate delivery without sacrificing quality.

---

## 💼 Work Experience
<div class="section">
{% for exp in site.data.experience %}
  <div class="item card">
    <h3>{{ exp.role }}</h3>
    <div class="meta"><strong>{{ exp.company }}</strong> • {{ exp.period }} • {{ exp.location }}</div>
    <ul>
      {% for bullet in exp.bullets %}
        <li>{{ bullet }}</li>
      {% endfor %}
    </ul>
  </div>
{% endfor %}
</div>

## 🛠️ Technical Skills
<div class="section">
<div class="skills-grid" style="display: grid; grid-template-columns: repeat(auto-fill, minmax(240px, 1fr)); gap: 1.25rem;">
{% for skill in site.data.skills %}
  <div class="card">
    <h4>{{ skill.category }}</h4>
    <ul style="list-style: none; padding-left: 0;">
      {% for item in skill.items %}
        <li>✓ {{ item }}</li>
      {% endfor %}
    </ul>
  </div>
{% endfor %}
</div>
</div>

## 🚀 Featured Projects
<div class="section">
{% for proj in site.data.projects %}
  <div class="item card">
    <h3>{{ proj.title }}</h3>
    <div class="tech"><strong>{{ proj.tech }}</strong></div>
    <p>{{ proj.description }}</p>
    <p><strong>Key Achievement:</strong> {{ proj.achievement }}</p>
    {% if proj.github_url %}
      <a href="{{ proj.github_url }}" class="btn" style="display: inline-block; padding: 0.5rem 1rem; background: #3b82f6; color: white; text-decoration: none; border-radius: 6px;">GitHub →</a>
    {% endif %}
  </div>
{% endfor %}
</div>

## 📜 Certifications
<div class="section">
<ul style="display: flex; flex-wrap: wrap; gap: 0.75rem; list-style: none; padding-left: 0;">
{% for cert in site.data.certifications %}
  <li style="background: #f1f5f9; padding: 0.4rem 1rem; border-radius: 20px; font-size: 0.95rem;">{{ cert }}</li>
{% endfor %}
</ul>
</div>

<div style="text-align: center; margin-top: 2rem;">
  <p>Let’s connect and build quality software together.</p>
  {% include social.html %}
</div>
