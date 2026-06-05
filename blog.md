---
layout: default
---

# 📝 Blog

Catatan akademik, refleksi penelitian, dan artikel tentang teknologi dan inovasi pendidikan.

---

## Artikel Terbaru

{% for post in site.posts limit:10 %}
<div class="card" style="margin-bottom: 20px;">
    <h3 style="margin-top: 0;">
        <a href="{{ post.url }}">{{ post.title }}</a>
    </h3>
    <p style="color: #666; font-size: 14px; margin: 5px 0;">
        📅 {{ post.date | date: "%d %B %Y" }}
        {% if post.author %} • Oleh {{ post.author }}{% endif %}
        {% if post.categories %}• {{ post.categories | join: ', ' }}{% endif %}
    </p>
    <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
    <a href="{{ post.url }}">Baca Selengkapnya →</a>
</div>
{% endfor %}

---

## Arsip Posting

### Berdasarkan Kategori

{% for category in site.categories %}
<h3>📂 {{ category[0] }}</h3>
<ul>
{% for post in category[1] %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a> 
    <span style="color: #666; font-size: 12px;">({{ post.date | date: "%b %Y" }})</span>
  </li>
{% endfor %}
</ul>
{% endfor %}

---

### Berdasarkan Tahun

{% for year in site.posts | group_by: "publish_year" reversed %}
<h3>📅 {{ year.name }}</h3>
<ul>
{% for post in year.items %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a> 
    <span style="color: #666; font-size: 12px;">({{ post.date | date: "%d %b" }})</span>
  </li>
{% endfor %}
</ul>
{% endfor %}

---

<p style="text-align: center; margin-top: 40px; padding-top: 20px; border-top: 1px solid #e1e4e8;">
  <a href="/">← Kembali ke Profil Utama</a>
</p>
