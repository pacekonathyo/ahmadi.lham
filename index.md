---
layout: default
---

# 👤 Ahmadi Lham

**Academic Profile & Personal Blog**

---

## 📋 Tentang Saya

Selamat datang di halaman profile akademik saya. Saya adalah seorang akademisi yang bersemangat dalam penelitian, pengajaran, dan berbagi pengetahuan melalui berbagai platform.

### Bidang Keahlian
- 🔬 Research & Development
- 📚 Academic Writing
- 💻 Technology & Innovation
- 🎓 Educational Technology

---

## 🎓 Pendidikan

| Tahun | Degree | Institusi |
|-------|--------|-----------|
| 2019 | Master of Science | Universitas [Nama] |
| 2017 | Bachelor of Science | Universitas [Nama] |

---

## 💼 Pengalaman Profesional

**Posisi Saat Ini**
- Position Title at University/Institution
- Periode: [Tahun] - Sekarang

**Pengalaman Sebelumnya**
- Previous Position at Organization
- Periode: [Tahun] - [Tahun]

---

## 📖 Publikasi

### Jurnal Internasional
1. **Judul Artikel** (2024)
   - Journal Name, Volume XX, Issue X
   - DOI: [Link]

2. **Judul Artikel Lainnya** (2023)
   - Journal Name, Volume XX, Issue X
   - DOI: [Link]

### Konferensi
- Presentasi di [Nama Konferensi] (2024)
- Presentasi di [Nama Konferensi] (2023)

---

## 🏆 Penghargaan & Pengakuan

- Award Name (Year)
- Recognition or Certification (Year)

---

## 🔗 Tautan Penting

- 📧 Email: [{{ site.email }}](mailto:{{ site.email }})
- 🐙 GitHub: [@{{ site.github_username }}](https://github.com/{{ site.github_username }})
- 🔗 LinkedIn: [Your Profile](https://linkedin.com)
- 📚 Google Scholar: [Profile Link](https://scholar.google.com)

---

## 📝 Blog Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%d %b %Y" }}
{% endfor %}

---

<div style="text-align: center; margin-top: 40px; padding-top: 20px; border-top: 1px solid #e5e5e5;">
  <p style="font-size: 12px; color: #666;">
    Last updated: {{ site.time | date: "%d %B %Y" }} | 
    <a href="https://github.com/{{ site.github_username }}/ahmadi.lham">View on GitHub</a>
  </p>
</div>
