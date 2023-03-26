---
title: About
layout: page
description: About
bodyClass: page-about
---

At Antrum Technologies, we create software that fills a void. No niche remains untouched.

![About our services](/images/thom-holmes-Lrfw0U_o9I0-unsplash.jpg)

# About us

We are proudly based in Eindhoven, the Netherlands.

# Our services

<div class="row justify-content-center">
  {% for feature in site.data.features %}
  <div class="col-12 col-md-6 col-lg-4 mb-2">
    <div class="feature">
      <h2 class="feature-title">{{ feature.title }}</h2>
      <div class="feature-content">{{ feature.description }}</div>
    </div>
  </div>
  {% endfor %}
</div>

# Information you might need

### Address
Lanceloetstraat 6, Eindhoven, 5625 BW, the Netherlands

### CoC number
89275233

### VAT number
NL864931621B01