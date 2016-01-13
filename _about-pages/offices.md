---
title:      Offices
caption:    We have five offices in three countries
avatar:     /images/about/globe.png
nav-weight: 30
---

<div class="page-offices">
  {% for o in site.data.offices %}
    <div class="office">
      <div>
        <div class="column">
          {{ o.map }}
        </div>
        <div class="column">
          <h3>{{ o.title }}</h3>
          <p class="auto-break"><span>{{ o.address| strip_html}}</span><span>VAT: {{ o.vat }}</span></p>
          <p class="auto-break"><a href="tel:{{ o.phone }}">{{ o.phone }}</a><a href="mailto:{{ o.email }}">{{ o.email }}</a></p>
        </div>
      </div>
    </div>
  {% endfor %}
</div>
