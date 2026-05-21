---
layout: single
title: "<p style='font-size: 0.8em;'>Research</p>"
permalink: /research/
classes: single
toc_label: "Research Themes"
toc_icon: "pen"
toc: true
sidebar:
  nav: sidebar
  sticky: true


---

> <p style="font-size: 0.8em;">We engage in multiple research themes with the aim to improve our understanding of all things <b>food, data, and AI</b>. Our current research inquiries are broadly categorized as: </p>

<hr>

##### 1. Food Knowledge Graph

<div class="section-indent research-question">
  Can we build a comprehensive, granular, and reliable <b>Food Knowledge Graph</b> for Indian cuisine detailing ingredient, recipe, process, nutrition, etc.?
  {% include feature_row_custom items=site.data.research_themes.knowledge_graph %}
</div>

###### &nbsp;&nbsp;&nbsp; <i class="fa-solid fa-seedling"></i> <u> Contributions & Impact </u>
{% assign kg_pubs = site.data.publications | where: "primary_track", "knowledge_graph" %}
{% include publication_grid.html items=kg_pubs %}

<br>
<hr>

<!--------------------------------->

##### 2. Diet-based Health Research & Analysis
  
<div class="section-indent research-question">
  Can a holistic and context-aware <b>Personal Food Model</b> enable us to study the interplay of food with diet-based diseases, health, and well-being?
  {% include feature_row_custom items=site.data.research_themes.dietary_health %}
</div>

###### &nbsp;&nbsp;&nbsp; <i class="fa-solid fa-seedling"></i> <u> Contributions & Impact </u>
{% assign hr_pubs = site.data.publications | where: "primary_track", "dietary_health" %}
{% include publication_grid.html items=hr_pubs %}


<br>
<hr>

<!--------------------------------->

##### 3. Multimodal & AI Food Solutions

<div class="section-indent research-question">
  Can we build <b>Multimodal & AI Food Solutions</b> tailored to Indian cuisine that combine visual, textual, and procedural understanding to enable intelligent food analysis, recipe generation, and data interpretation at scale?
  {% include feature_row_custom items=site.data.research_themes.multimodal_food %}
</div>

###### &nbsp;&nbsp;&nbsp; <i class="fa-solid fa-seedling"></i> <u> Contributions & Impact </u>
{% assign mf_pubs = site.data.publications | where: "primary_track", "multimodal_food" %}
{% include publication_grid.html items=mf_pubs %}

<br>
<hr>

<!--------------------------------->

##### 4. Food Availability Atlas
  
<div class="section-indent research-question">
  Can we develop a <b>Food Availability Atlas</b> by incorporating geo-tagged food data, such as eatery maps, regional availability, pricing, consumption trends, and heritage, to support contextual applications?
  {% include feature_row_custom items=site.data.research_themes.food_atlas %}
</div>

###### &nbsp;&nbsp;&nbsp; <i class="fa-solid fa-seedling"></i> <u> Contributions & Impact </u>
{% assign fa_pubs = site.data.publications | where: "primary_track", "food_atlas" %}
{% include publication_grid.html items=fa_pubs %}

<br>
<hr>

<!--------------------------------->

##### 5. Nutriagroeconomy & Agroecology
  
<div class="section-indent research-question">
  Can we model the Indian agri-food ecosystem <b>(Nutri-agroeconomy & Agroecology)</b> by integrating local knowledge systems, ecological principles, food policy frameworks, and end-to-end food flow data?
  {% include feature_row_custom items=site.data.research_themes.food_systems %}
</div>

###### &nbsp;&nbsp;&nbsp; <i class="fa-solid fa-seedling"></i> <u> Contributions & Impact </u>
{% assign fs_pubs = site.data.publications | where: "primary_track", "food_systems" %}
{% include publication_grid.html items=fs_pubs %}

<br>
<hr>

<!--------------------------------->

##### 6. Food Knowledge Dissemination

<div class="section-indent research-question">
  Can we build intelligent systems for Personal Health Navigation with contextual and conversational abilities in vernacular text and speech to enable equitable <b>Food Knowledge Dissemination</b>?
  {% include feature_row_custom items=site.data.research_themes.knowledge_dissemination %}
</div>

###### &nbsp;&nbsp;&nbsp; <i class="fa-solid fa-seedling"></i> <u> Contributions & Impact </u>
{% assign kd_pubs = site.data.publications | where: "primary_track", "knowledge_dissemination" %}
{% include publication_grid.html items=kd_pubs %}

<br>
<hr>

<!--------------------------------->

<style>
  .section-indent {
    margin-left: 2rem;
    font-size: 0.85em;
  }
</style>