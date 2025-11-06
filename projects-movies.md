---
layout: default
title: "Movies & Series - {% t projects.movies.meta.title %}"
description: "{% t projects.movies.meta.description %}"
---

<!-- Hero Section -->
<section class="project-hero">
  <div class="project-hero-background">
    <div class="hero-pattern"></div>
    <div class="floating-orb orb-1"></div>
    <div class="floating-orb orb-2"></div>
    <div class="floating-orb orb-3"></div>
  </div>
  
  {% if site.lang == "en" %}
    {% capture home_link %}/en{% endcapture %}
  {% else %}
    {% capture home_link %}/{% endcapture %}
  {% endif %}
  <a href="{{ home_link }}" class="back-button" aria-label="{% t cta.home %}">
    <svg width="20" height="20" fill="currentColor" viewBox="0 0 24 24">
      <path d="M20 11H7.83l5.59-5.59L12 4l-8 8 8 8 1.41-1.41L7.83 13H20v-2z"/>
    </svg>
    <span class="back-text">{% t cta.home %}</span>
  </a>

  <div class="container">
    <div class="project-hero-content">
      <div class="hero-badge">
        <span class="badge-dot"></span>
        <span>{% t projects.movies.badge %}</span>
      </div>
      
      <h1 class="project-title">
        <span class="title-highlight">{% t projects.movies.title_highlight %}</span><br/>
        {% t projects.movies.title %}
      </h1>
      
      <p class="project-description">
        {% t projects.movies.description %}
      </p>

      <div class="project-tags">
        <span class="project-tag">Angular</span>
        <span class="project-tag">TypeScript</span>
        <span class="project-tag">RxJS</span>
        <span class="project-tag">TMDB API</span>
        <span class="project-tag">Responsive Design</span>
      </div>

      <div class="hero-actions">
        <a href="#features" class="btn-primary">
          <span>{% t projects.movies.cta.discover %}</span>
          <svg width="20" height="20" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path d="M19 12H5M12 5l7 7-7 7" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </a>
        <a href="https://github.com/benoitrongeard/movies-app" target="_blank" class="btn-secondary">
          <svg width="20" height="20" fill="currentColor" viewBox="0 0 24 24">
            <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
          </svg>
          <span>{% t projects.movies.cta.github %}</span>
        </a>
      </div>
    </div>

  </div>
</section>

<!-- Features Section - Bento Grid -->
<section id="features" class="features-section">
  <div class="container">
    <h2 class="section-title">{% t projects.movies.features.title %}</h2>
    <p class="section-subtitle">{% t projects.movies.features.subtitle %}</p>

    <div class="features-bento-grid">
      <!-- Feature 1 - Large -->
      <div class="feature-card span-8">
        <div class="feature-icon">
          <svg width="48" height="48" viewBox="0 0 24 24" fill="none">
            <path d="M12 22C17.5228 22 22 17.5228 22 12C22 6.47715 17.5228 2 12 2C6.47715 2 2 6.47715 2 12C2 17.5228 6.47715 22 12 22Z" stroke="currentColor" stroke-width="2"/>
            <path d="M12 6V12L16 14" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
          </svg>
        </div>
        <h3 class="feature-title">{% t projects.movies.features.realtime.title %}</h3>
        <p class="feature-description">{% t projects.movies.features.realtime.description %}</p>
        <div class="feature-image">
          <img src="/assets/img/screens/home.png" alt="Interface principale" loading="lazy" />
        </div>
      </div>

      <!-- Feature 2 -->
      <div class="feature-card span-4">
        <div class="feature-icon">
          <svg width="48" height="48" viewBox="0 0 24 24" fill="none">
            <path d="M21 21L15 15M17 10C17 13.866 13.866 17 10 17C6.13401 17 3 13.866 3 10C3 6.13401 6.13401 3 10 3C13.866 3 17 6.13401 17 10Z" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
          </svg>
        </div>
        <h3 class="feature-title">{% t projects.movies.features.search.title %}</h3>
        <p class="feature-description">{% t projects.movies.features.search.description %}</p>
      </div>

      <!-- Feature 3 -->
      <div class="feature-card span-4">
        <div class="feature-icon">
          <svg width="48" height="48" viewBox="0 0 24 24" fill="none">
            <path d="M12 2L15.09 8.26L22 9.27L17 14.14L18.18 21.02L12 17.77L5.82 21.02L7 14.14L2 9.27L8.91 8.26L12 2Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </div>
        <h3 class="feature-title">{% t projects.movies.features.ratings.title %}</h3>
        <p class="feature-description">{% t projects.movies.features.ratings.description %}</p>
      </div>

      <!-- Feature 4 - Image -->
      <div class="feature-card span-8">
        <div class="feature-image">
          <img src="/assets/img/screens/detail.png" alt="Détail d'un film" loading="lazy" />
        </div>
      </div>

      <!-- Feature 5 -->
      <div class="feature-card span-6">
        <div class="feature-icon">
          <svg width="48" height="48" viewBox="0 0 24 24" fill="none">
            <path d="M16 7C16 9.20914 14.2091 11 12 11C9.79086 11 8 9.20914 8 7C8 4.79086 9.79086 3 12 3C14.2091 3 16 4.79086 16 7Z" stroke="currentColor" stroke-width="2"/>
            <path d="M12 14C8.13401 14 5 17.134 5 21H19C19 17.134 15.866 14 12 14Z" stroke="currentColor" stroke-width="2"/>
          </svg>
        </div>
        <h3 class="feature-title">{% t projects.movies.features.actors.title %}</h3>
        <p class="feature-description">{% t projects.movies.features.actors.description %}</p>
      </div>

      <!-- Feature 6 -->
      <div class="feature-card span-6">
        <div class="feature-icon">
          <svg width="48" height="48" viewBox="0 0 24 24" fill="none">
            <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z" fill="currentColor"/>
          </svg>
        </div>
        <h3 class="feature-title">{% t projects.movies.features.responsive.title %}</h3>
        <p class="feature-description">{% t projects.movies.features.responsive.description %}</p>
      </div>
    </div>

  </div>
</section>

<!-- Tech Stack Section -->
<section class="project-tech-section">
  <div class="container">
    <h2 class="section-title">{% t projects.movies.tech.title %}</h2>
    <p class="section-subtitle">{% t projects.movies.tech.subtitle %}</p>

    <div class="tech-grid">
      <div class="tech-item">
        <img src="https://skillicons.dev/icons?i=angular" alt="Angular" />
        <h4>Angular 17</h4>
        <p>{% t projects.movies.tech.angular %}</p>
      </div>
      <div class="tech-item">
        <img src="https://skillicons.dev/icons?i=ts" alt="TypeScript" />
        <h4>TypeScript</h4>
        <p>{% t projects.movies.tech.typescript %}</p>
      </div>
      <div class="tech-item">
        <img src="https://skillicons.dev/icons?i=rxjs" alt="RxJS" />
        <h4>RxJS</h4>
        <p>{% t projects.movies.tech.rxjs %}</p>
      </div>
      <div class="tech-item">
        <div class="custom-icon">API</div>
        <h4>TMDB API</h4>
        <p>{% t projects.movies.tech.api %}</p>
      </div>
    </div>

  </div>
</section>

<!-- Screenshots Gallery -->
<section class="gallery-section">
  <div class="container">
    <h2 class="section-title">{% t projects.movies.gallery.title %}</h2>
    <p class="section-subtitle">{% t projects.movies.gallery.subtitle %}</p>

    <div class="screenshots-grid">
      <div class="screenshot-item large">
        <img src="/assets/img/screens/home.png" alt="Page d'accueil" loading="lazy" />
        <div class="screenshot-overlay">
          <h4>{% t projects.movies.gallery.home %}</h4>
        </div>
      </div>
      <div class="screenshot-item">
        <img src="/assets/img/screens/detail-crop.png" alt="Détail film" loading="lazy" />
        <div class="screenshot-overlay">
          <h4>{% t projects.movies.gallery.detail %}</h4>
        </div>
      </div>
      <div class="screenshot-item">
        <img src="/assets/img/screens/search.png" alt="Recherche" loading="lazy" />
        <div class="screenshot-overlay">
          <h4>{% t projects.movies.gallery.search %}</h4>
        </div>
      </div>
      <div class="screenshot-item">
        <img src="/assets/img/screens/detail.png" alt="Détail complet" loading="lazy" />
        <div class="screenshot-overlay">
          <h4>{% t projects.movies.gallery.detail %}</h4>
        </div>
      </div>
    </div>

  </div>
</section>

<!-- CTA Section -->
<section class="project-cta-section">
  <div class="container">
    <div class="cta-content">
      <h2 class="cta-title">{% t projects.movies.cta.title %}</h2>
      <p class="cta-description">{% t projects.movies.cta.description %}</p>
      <div class="cta-actions">
        <a href="https://github.com/benoitrongeard/movies-app" target="_blank" class="btn-primary btn-large">
          <svg width="24" height="24" fill="currentColor" viewBox="0 0 24 24">
            <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
          </svg>
          <span>{% t projects.movies.cta.view_code %}</span>
        </a>
      </div>
    </div>
  </div>
</section>
