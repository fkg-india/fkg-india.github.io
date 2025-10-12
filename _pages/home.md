---
layout: single
title: "<p style='font-size: 0.8em;'>FoodComputing@Ashoka</p>"
permalink: /home
toc: false
sidebar:
  nav: sidebar
  sticky: true
header:
  height: 100vh
  overlay_image: /assets/images/banner/food_banner.jpg
  caption: "wallpapers"
  actions:
  - label: "<a href='/connect/' target='_blank' style='display: inline-block; padding: 10px 15px; background-color: transparent; color: white; text-decoration: none; border: 2px solid white; border-radius: 5px; font-weight: bold;' onmouseover='this.style.backgroundColor=\"white\"; this.style.color=\"black\"' onmouseout='this.style.backgroundColor=\"transparent\"; this.style.color=\"white\"'> <i class='fas fa-fw fa-link'></i>Internship Opportunities<a>"
    url: "#"
  - label: "<a href='https://sites.google.com/view/rasoi-ncvpripg-2025/' target='_blank' style='display: inline-block; padding: 10px 15px; background-color: transparent; color: white; text-decoration: none; border: 2px solid white; border-radius: 5px; font-weight: bold;' onmouseover='this.style.backgroundColor=\"white\"; this.style.color=\"black\"' onmouseout='this.style.backgroundColor=\"transparent\"; this.style.color=\"white\"'> <i class='fas fa-fw fa-link'></i> NCVPRIPG'25 RASOI Data Challenge</a>"
    url: "#"
  - label: "<a href='https://mm-food.github.io/' target='_blank' style='display: inline-block; padding: 10px 15px; background-color: transparent; color: white; text-decoration: none; border: 2px solid white; border-radius: 5px; font-weight: bold;' onmouseover='this.style.backgroundColor=\"white\"; this.style.color=\"black\"' onmouseout='this.style.backgroundColor=\"transparent\"; this.style.color=\"white\"'> <i class='fas fa-fw fa-link'></i> ACM MMFood'25 Workshop</a>"
    url: "#"
  - label: "<a href='/assets/resources/MMFood25_CFP.pdf' target='_blank' style='display: inline-block; padding: 10px 15px; background-color: transparent; color: white; text-decoration: none; border: 2px solid white; border-radius: 5px; font-weight: bold;' onmouseover='this.style.backgroundColor=\"white\"; this.style.color=\"black\"' onmouseout='this.style.backgroundColor=\"transparent\"; this.style.color=\"white\"'> <i class='fas fa-download'></i> Download ACM MMFood'25 Call for Papers</a>"
    url: "#"
excerpt: "Cooking humane, intelligent, scalable food solutions, <br> where <b>food</b>, <b>data</b>, & <b>AI</b> simmer into deliciously interdisciplinary research."
permalink: /home

banner_left:
  - image_path: /assets/images/banner/food_banner_alt.jpg
    excerpt: "Welcome to the **Food Computing Lab**! We strive to deepen our understanding of food and its intricate connections, including but not limited to *recipes, cooking, well-being, nutrition, dietary practices, agriculture, agrecology, misinformation, and heritage* - particularly in the **Indian context**. Our work emphasizes the importance of understanding food not only as a source of sustenance and enjoyment, but also as a vital component of a healthy and sustainable lifestyle. Using novel AI-driven computational technologies, we mine, curate and analyze data and relationships within food systems to uncover insights that enable *healthier eating habits, recipe generation, food recommendation, knowledge discovery, and informed decision-making*. To know more about our work, please browse the [research](/research/) section."
    image_caption: unsplash
---

<div class="d-flex align-items-center mb-4"> <!-- Flex container for logo and heading -->
  {% include feature_row_home_img id="banner_left" type="left" %}
</div>

<hr>

<h3 style="text-align:left; font-size: 1.5rem; margin-top: 30px;">Publications</h3>

<section id="publications-widget">
  <div class="pub-header-row">
    <h2 id="pub-heading">DISCOVER OUR LATEST RESEARCH STORIES BELOW</h2>

    <div class="pub-search-wrap">
      <label for="pub-search" class="sr-only">Search publications</label>
      <input id="pub-search" type="search" placeholder="Search publications..." aria-label="Search publications">
    </div>
  </div>

  <div class="pub-table-wrap">
    <table id="pub-table" class="pub-table" summary="List of publications with year and title">
      <colgroup>
        <col style="width:72px;">
        <col style="width:auto;">
      </colgroup>
      <thead>
        <tr>
          <th scope="col" class="th-year">Year</th>
          <th scope="col" class="th-title">Title</th>
        </tr>
      </thead>
      <tbody id="pub-tbody">
        <!-- rows injected by JS -->
      </tbody>
    </table>
  </div>

  <nav class="pagination" aria-label="Publications pagination">
    <button id="prev-btn" aria-label="Previous page">Previous</button>
    <div id="page-numbers" class="page-numbers"></div>
    <button id="next-btn" aria-label="Next page">Next</button>
  </nav>

  <hr><hr>

</section>

<hr>

<h3 style="text-align:left; font-size: 1.5rem; margin-top: 30px;">Beyond Recipes: Tracing the Complexities of Indian Food</h3>

<div class="horizontal-timeline-wrapper">
  <div class="horizontal-timeline">
    {% for event in site.data.timeline %}
      <div class="timeline-item">
        <h4>{{ event.title }}</h4>
        <p>{{ event.description }}</p>
      </div>
    {% endfor %}
  </div>
</div>

<hr>

#### Announcements
<div class="notice--danger">
  <h4>Internship Opportunities</h4>
  <p>We are actively seeking enthusiastic and passionate students for internship. If you are interested in working with us, please fill the <a href='/connect/' target='_blank'>form</a> here or mail us directly at foodcomputing.ashoka@gmail.com to express your interest.</p>
</div>
<div class="notice--danger">
  <h4>ACM Multimedia - MMFood'25 [October 2025]</h4>
  <p>The <a href="https://mm-food.github.io/" target="_blank" class="alert-link">1st International Workshop on Multi-modal Food Computing (MMFood'25)</a> will be hosted in conjunction with the 33rd ACM International Conference on Multimedia (ACMMM25) on <b>28th Oct. in Dublin, Ireland.</b> 2025. The details of the hackathon based on Indian food knowledge graph will be made available soon.</p>
</div>

<style>
.horizontal-timeline-wrapper {
  overflow-x: auto;
  padding: 20px 0;
  margin-bottom: 40px;
  position: relative;
  scrollbar-width: thin;
  scrollbar-color: #a47551 #f4f0ec;
}

.horizontal-timeline-wrapper::-webkit-scrollbar {
  height: 8px;
}
.horizontal-timeline-wrapper::-webkit-scrollbar-track {
  background: #f4f0ec;
}
.horizontal-timeline-wrapper::-webkit-scrollbar-thumb {
  background-color: #a47551;
  border-radius: 4px;
}

.horizontal-timeline {
  display: flex;
  gap: 24px;
  padding: 60px 15px 15px;
  position: relative;
  font-size: 0.75em;
  scroll-snap-type: x mandatory;
  min-width: max-content; /* 💡 Ensures it grows with content */
}

.horizontal-timeline::before {
  content: "";
  position: absolute;
  top: 34px;
  left: 0;
  height: 2px;
  width: 100%;
  background-image: repeating-linear-gradient(to right, #7b3f00 0 6px, transparent 6px 12px);
  z-index: 0;
}

.timeline-item {
  flex: 0 0 220px;
  background-color: #fffdf8;
  border: 1px solid #e5d9c5;
  border-radius: 8px;
  padding: 16px;
  scroll-snap-align: start;
  box-shadow: 0 4px 6px rgba(0,0,0,0.05);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  position: relative;
  z-index: 1;
  cursor: pointer;
}

.timeline-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 12px rgba(0,0,0,0.1);
}

.timeline-item::before {
  content: '';
  position: absolute;
  top: -36px;
  left: 50%;
  transform: translateX(-50%);
  width: 18px;
  height: 18px;
  background-color: #7b3f00;
  border: 3px solid #fff;
  border-radius: 50%;
  box-shadow: 0 0 0 3px rgba(123, 63, 0, 0.25), 0 2px 4px rgba(0, 0, 0, 0.1);
  z-index: 2;
}

.timeline-item h4 {
  margin: 0 0 8px;
  color: #6a3900;
  font-size: 1.1em;
  font-weight: 600;
}

.timeline-item p {
  margin: 0;
  line-height: 1.5em;
  color: #3a2c1a;
  font-size: 0.9em;
}

:root{
  --muted:#6b6b6b;
  --accent:#0b7dda;
  --row-hover:#f7fbff;
  --pill-bg:#e6f3ff;
  --pill-color:#045a8d;

  /* header bg + text */
  --header-bg: #eef6fb;
  --header-text: #04263a;
}

/* container + header row (title and search same line) */
#publications-widget{max-width:900px;margin:12px auto;font-family:Inter,system-ui,-apple-system,'Segoe UI',Roboto,'Helvetica Neue',Arial;color:#111;padding:8px}
.pub-header-row{
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:12px;
  margin-bottom:10px;
  background:var(--header-bg);
  color:var(--header-text);
  padding:10px 12px;
  border-radius:8px;
  border:1px solid rgba(4,38,58,0.04);
}
#pub-heading{font-size:13px;margin:0;font-weight:700;letter-spacing:0.04em}

/* search — reduced width */
#pub-search{padding:7px 10px;border:1px solid #e6e6e6;border-radius:8px;width:180px;font-size:13px}

/* table — smaller font sizes for title, year, tag; fixed layout so header width stable */
.pub-table-wrap{overflow:auto;border-radius:6px}
.pub-table{width:100%;border-collapse:collapse;font-size:13px;table-layout:fixed}
.pub-table thead th{ text-align:left;padding:8px 8px;border-bottom:1px solid #eee;color:var(--muted);font-weight:600;font-size:12px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.th-year{width:72px}
.th-title{width:calc(100% - 72px)}

/* body cells */
.pub-table tbody td{padding:10px 8px;border-bottom:1px dashed #f1f1f1;vertical-align:middle;overflow:hidden}
.pub-row{transition:transform .15s ease, box-shadow .15s ease, background .12s ease; transform-origin:left center}
.pub-row:hover{background:var(--row-hover); transform: scale(1.02); box-shadow: 0 8px 22px rgba(11,125,218,0.06); z-index:1}

/* small typography */
.pub-year { font-size:12px; color:var(--muted); white-space:nowrap; }
.pub-title-link{color:inherit;text-decoration:none;font-weight:600;font-size:13px; display:inline-block; max-width: calc(100% - 140px); vertical-align:middle;}
.pub-title-link:hover{text-decoration:underline;color:var(--accent)}
.pub-tag-pill{font-size:11px;padding:3px 8px;border-radius:999px;background:var(--pill-bg);color:var(--pill-color);font-weight:700;margin-left:8px;display:inline-block; white-space:nowrap;}

/* ensure tags appear AFTER title and don't force header to resize */
.title-and-tags{display:flex;align-items:center;gap:8px;flex-wrap:wrap;}

/* visually separate header from content */
.pub-table thead { background: white; position:sticky; top:0; z-index:2 }

/* pagination and misc */
.pagination{display:flex;gap:8px;align-items:center;justify-content:flex-start;margin-top:12px}
.pagination button{padding:6px 10px;border-radius:6px;border:1px solid #e8e8e8;background:#fff;cursor:pointer;font-size:12px}
.page-numbers{display:flex;gap:6px}
.page-numbers button{padding:6px 8px;border-radius:6px;border:none;background:transparent;color:var(--muted);cursor:pointer;font-size:12px}
.page-numbers button[aria-current]{font-weight:700;color:inherit}
.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border:0}

/* responsive: stack header and allow search full width */
@media (max-width:640px){
  .pub-header-row{flex-direction:column;align-items:flex-start;gap:8px}
  #pub-search{width:100%;}
  .pub-row:hover{transform: none; box-shadow:none}
  .pub-title-link{max-width:100%}
}
</style>



<script>
// FALLBACKS: page.publications -> site.data.my_publications -> site.data.publications
const _page_pubs = {{ page.publications  | default: 'null' | jsonify }};
const _pubs      = {{ site.data.publications   | default: 'null' | jsonify }};

let PUBS = [];
if (Array.isArray(_page_pubs)) PUBS = _page_pubs;
else if (Array.isArray(_pubs)) PUBS = _pubs;

if (!Array.isArray(PUBS)) PUBS = [];

// sort newest-first by year (numeric)
PUBS.sort((a,b) => (parseInt(b.year)||0) - (parseInt(a.year)||0));

const ROWS_PER_PAGE = 8;
let filtered = PUBS.slice();
let page = 1;

const tbody = document.getElementById('pub-tbody');
const search = document.getElementById('pub-search');
const prevBtn = document.getElementById('prev-btn');
const nextBtn = document.getElementById('next-btn');
const pageNumbers = document.getElementById('page-numbers');

function makeRow(p) {
  const tr = document.createElement('tr');
  tr.className = 'pub-row';

  // Year cell (small)
  const tdYear = document.createElement('td');
  tdYear.className = 'pub-year';
  tdYear.textContent = p.year || '';
  tr.appendChild(tdYear);

  // Title cell: title first, then tags (tags AFTER the title)
  const tdTitle = document.createElement('td');

  const titleAndTags = document.createElement('div');
  titleAndTags.className = 'title-and-tags';

  // title link (small)
  const titleWrap = document.createElement('div');
  titleWrap.style.flex = '1 1 auto';
  const link = document.createElement('a');
  link.className = 'pub-title-link';
  link.textContent = p.title || '';
  link.href = (p.urls && (p.urls.article || p.urls.doi || p.urls.arxiv || p.urls.pdf)) ? (p.urls.article || p.urls.doi || p.urls.arxiv || p.urls.pdf) : '#';
  link.target = '_blank';
  link.rel = 'noopener';
  titleWrap.appendChild(link);

  titleAndTags.appendChild(titleWrap);

  // tags AFTER title
  if (Array.isArray(p.tags) && p.tags.length) {
    const tagsWrap = document.createElement('div');
    tagsWrap.style.flex = '0 0 auto';
    tagsWrap.style.display = 'flex';
    tagsWrap.style.gap = '6px';
    p.tags.forEach(tag => {
      const pill = document.createElement('span');
      pill.className = 'pub-tag-pill';
      pill.textContent = tag;
      tagsWrap.appendChild(pill);
    });
    titleAndTags.appendChild(tagsWrap);
  }

  tdTitle.appendChild(titleAndTags);
  tr.appendChild(tdTitle);

  return tr;
}

function renderTable() {
  tbody.innerHTML = '';
  const start = (page - 1) * ROWS_PER_PAGE;
  const rows = filtered.slice(start, start + ROWS_PER_PAGE);
  if (rows.length === 0) {
    const tr = document.createElement('tr');
    const td = document.createElement('td');
    td.setAttribute('colspan', 2);
    td.style.color = 'var(--muted)';
    td.style.padding = '18px 8px';
    td.textContent = 'No results found.';
    tr.appendChild(td);
    tbody.appendChild(tr);
    return;
  }
  rows.forEach(r => tbody.appendChild(makeRow(r)));
}

function renderPagination() {
  pageNumbers.innerHTML = '';
  const totalPages = Math.max(1, Math.ceil(filtered.length / ROWS_PER_PAGE));
  for (let i = 1; i <= totalPages; i++) {
    const btn = document.createElement('button');
    btn.textContent = i;
    if (i === page) btn.setAttribute('aria-current', 'page');
    btn.addEventListener('click', () => { page = i; renderTable(); renderPagination(); });
    pageNumbers.appendChild(btn);
  }
  prevBtn.disabled = page === 1;
  nextBtn.disabled = page === totalPages;
}

function normalize(s){ return (s||'').toString().toLowerCase(); }

search.addEventListener('input', () => {
  const q = normalize(search.value.trim());
  if (!q) filtered = PUBS.slice();
  else filtered = PUBS.filter(p =>
    normalize(p.title).includes(q) ||
    (p.tags && p.tags.join(' ').toLowerCase().includes(q)) ||
    normalize(String(p.year || '')).includes(q) ||
    normalize(p.venue || '').includes(q)
  );
  page = 1;
  renderTable();
  renderPagination();
});

prevBtn.addEventListener('click', () => { if (page > 1) page--; renderTable(); renderPagination(); });
nextBtn.addEventListener('click', () => { const total = Math.ceil(filtered.length / ROWS_PER_PAGE); if (page < total) page++; renderTable(); renderPagination(); });

/* initial render */
renderTable();
renderPagination();
</script>
