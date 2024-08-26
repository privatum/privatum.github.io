---
layout: splash
permalink: /
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /images/header-image.jpg
  video:
    path: /videos/background-video.mp4
  actions:
    - label: "Learn More"
      url: "/about/"
excerpt: "PrivaTUM"
intro: 
  - excerpt: 'We are dedicated to exploring and advancing the cutting-edge intersection of artificial intelligence and privacy.'
---

{% include feature_row id="intro" type="center" %}

# Welcome to PrivaTUM

We are a passionate collective of computer science students from the Technical University of Munich (TUM) dedicated to exploring and advancing the cutting-edge intersection of artificial intelligence and privacy.

[Learn More About Us](/about/){: .btn .btn--learn-more}

## Upcoming Events
{% include upcoming_events.html %}

## Latest News and Stories

<div class="post-grid">
  {% for post in site.posts limit:3 %}
    <div class="post-item">
      {% if post.header.teaser %}
        <div class="post-image">
          <img src="{{ post.header.teaser | relative_url }}" alt="{{ post.title }}">
        </div>
      {% endif %}
      <div class="post-content">
        <p class="post-category">{{ post.categories[0] | upcase }} {{ post.date | date: "%d.%m.%Y" }}</p>
        <h2 class="post-title">{{ post.title }}</h2>
        <p class="post-excerpt">{{ post.excerpt | strip_html | truncate: 100 }}</p>
        <a href="{{ post.url | relative_url }}" class="read-more">Mehr erfahren</a>
      </div>
    </div>
  {% endfor %}
</div>

<section class="benefits">
  <h2>BENEFITS</h2>
  
  <p class="benefits-tagline">We support you</p>
  
  <div class="benefits-description">
    <p>Are you passionate about AI and ready to make a real-world impact? PrivaTUM invites you to join our AI Research Lab, a platform where visionaries, doers, and risk-takers with an interest in AI and privacy come together to shape the future of technology. We value diversity, curiosity, and a commitment to learning and improvement.</p>
    
  </div>
  
  <div class="benefits-grid">
    <div class="benefit-item">
      <i class="fas fa-network-wired"></i>
      <h3>ACCESS TO OUR NETWORK</h3>
    </div>
    <div class="benefit-item">
      <i class="fas fa-hands-helping"></i>
      <h3>COUNT ON OUR SUPPORT</h3>
    </div>
  </div>
</section>