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
  - excerpt: ''
---

{% include feature_row id="intro" type="center" %}

# Welcome to PrivaTUM

We are a passionate collective of computer science students from the Technical University of Munich (TUM) dedicated to exploring and advancing the cutting-edge intersection of artificial intelligence and privacy.

<!-- [Learn More About Us](/about/){: .btn .btn--learn-more} -->

## Upcoming Events
{% include upcoming_events.html %}

## Latest News and Stories

<div class="post-grid">
  {% for post in site.posts limit:1 %}
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
        <a href="{{ post.url | relative_url }}" class="read-more">Show more</a>
      </div>
    </div>
  {% endfor %}
</div>

<section class="benefits">
  <h2>BENEFITS</h2>
  
  <p class="benefits-tagline">We support you</p>
  <div class="benefits-container">
    <div class="benefits-description">
      <p>Are you fascinated by the intersection of AI and privacy? We're seeking innovative minds to join us in developing privacy-preserving AI techniques that protect individual data while enabling powerful machine learning insights. Our topics span differential privacy, federated learning, and secure multi-party computation. If you're passionate about shaping the future of ethical AI that respects privacy, we invite you to be part of our diverse, curious, and committed team. Together, we can advance AI technology while safeguarding personal information.</p>
    </div>
    <div class="benefits-image">
      <!-- Add an image here -->
      <!-- <img src="/path/to/your/image.jpg" alt="Benefits of joining PrivaTUM"> -->
    </div>
  </div>
  <!-- <div class="benefits-grid">
    <div class="benefit-item">
      <i class="fas fa-network-wired"></i>
      <h3>ACCESS TO OUR NETWORK</h3>
    </div>
    <div class="benefit-item">
      <i class="fas fa-hands-helping"></i>
      <h3>COUNT ON OUR SUPPORT</h3>
    </div>
  </div> -->
</section> 

<section class="benefits">
  <h2>BENEFITS</h2>
  
  <p class="benefits-tagline">We support you</p>
  <div class="benefits-container">
    <div class="benefits-description">
      <p>Join our community to stay updated on the latest in privacy-preserving AI and connect with like-minded researchers and professionals.</p>
      <div class="join-buttons">
        <a href="https://join.slack.com/t/privatum-workspace/shared_invite/zt-2pjf4jky9-xKO0kHonJIWKjN0XlIJRlg" class="btn btn--slack">Join our Slack</a>
        <a href="#" class="btn btn--mailing-list">Join our Mailing List</a>
      </div>
    </div>
    <div class="benefits-image">
      <!-- Add an image here -->
      <!-- <img src="/path/to/your/image.jpg" alt="Benefits of joining PrivaTUM"> -->
    </div>
  </div>
  <!-- <div class="benefits-grid">
    <div class="benefit-item">
      <i class="fas fa-network-wired"></i>
      <h3>ACCESS TO OUR NETWORK</h3>
    </div>
    <div class="benefit-item">
      <i class="fas fa-hands-helping"></i>
      <h3>COUNT ON OUR SUPPORT</h3>
    </div>
  </div> -->
</section> 


<section class="team-members">
  <h2>MEET THE TEAM</h2>
  
  <div class="team-grid">
    <!-- <div class="team-member">
      <img src="/images/team/nikola.jpeg" alt="Nikola Selic">
      <h3>Nikola Selic</h3>
      <p>Founder</p>
      <div class="social-icons">
        <a href="https://www.linkedin.com/in/nikola-selic/" class="linkedin"><i class="fab fa-linkedin"></i></a>
      </div>
    </div> -->
    <!-- Add more team members as needed -->
  </div>
</section>



<section class="contact-us">
  <h2>You still have other questions?</h2>
  <a href="mailto:contact@privatum.tech" class="btn btn--contact">Ask us here</a>
</section>