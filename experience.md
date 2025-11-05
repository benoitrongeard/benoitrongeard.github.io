---
layout: default
title: "Benoît Rongeard — Tech Lead Freelance - {% t experience.meta.title %}"
description: "{% t experience.meta.description %}"
---

<!-- Hero Section -->
<section class="experience-hero">
  <div class="hero-background">
    <div class="hero-pattern"></div>
  </div>
  <div class="container">
    <div class="hero-content-experience">
      <h1 class="hero-title"><span>{% t experience.hero.title %}</span></h1>
      <div class="experience-stats">
        <div class="stat-item">
          <span class="stat-number">10+</span>
          <span class="stat-label">{% t experience.hero.stats.years %}</span>
        </div>
        <div class="stat-item">
          <span class="stat-number">15+</span>
          <span class="stat-label">{% t experience.hero.stats.projects %}</span>
        </div>
        <div class="stat-item">
          <span class="stat-number">50+</span>
          <span class="stat-label">{% t experience.hero.stats.team %}</span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Timeline Section -->
<section class="timeline-section">
  <div class="container">
    <div class="timeline">
      
      <!-- Coexya - Keolis SA -->
      <div class="timeline-item">
        <div class="timeline-marker">
          <div class="marker-dot"></div>
          <span class="timeline-period">{% t experience.timeline.coexya.period %}</span>
        </div>
        <div class="timeline-content">
          <div class="company-header">
            <h3 class="company-name">{% t experience.timeline.coexya.company %}</h3>
            <span class="duration">{% t experience.timeline.coexya.duration %}</span>
          </div>
          
          <!-- Lead tech Multi-produits -->
          <div class="position-card">
            <div class="position-header">
              <h4 class="position-title">{% t experience.timeline.coexya.multi_products.title %}</h4>
              <div class="position-meta">
                <span class="period">{% t experience.timeline.coexya.multi_products.period %}</span>
                <span class="team-size">{% t experience.timeline.coexya.multi_products.team %}</span>
              </div>
            </div>
            
            <div class="tech-stack">
              <span class="tech-tag">Angular</span>
              <span class="tech-tag">Java/Spring</span>
              <span class="tech-tag">Flutter</span>
              <span class="tech-tag">Azure DevOps</span>
              <span class="tech-tag">Kubernetes</span>
              <span class="tech-tag">PostgreSQL</span>
              <span class="tech-tag">Docker</span>
              <span class="tech-tag">Azure API Management</span>
              <span class="tech-tag">CI/CD</span>
              <span class="tech-tag">Swagger/OpenAPI</span>
              <span class="tech-tag">Azure AD</span>
            </div>
            
            <div class="responsibilities">
              <p><strong>{% t experience.timeline.coexya.multi_products.methodology %}</strong> {% t experience.timeline.coexya.multi_products.methodology_value %}</p>
              
              <h5>{% t experience.timeline.coexya.multi_products.products_title %}</h5>
              <ul class="project-list">
                <li>{% t experience.timeline.coexya.multi_products.products.mks %}</li>
                <li>{% t experience.timeline.coexya.multi_products.products.alerte %}</li>
                <li>{% t experience.timeline.coexya.multi_products.products.oskar %}</li>
                <li>{% t experience.timeline.coexya.multi_products.products.backoffice %}</li>
              </ul>
              
              <h5>{% t experience.timeline.coexya.multi_products.achievements_title %}</h5>
              <ul class="achievements-list">
                {% assign achievements = site.translations[site.lang].experience.timeline.coexya.multi_products.achievements %}
                {% for achievement in achievements %}
                  <li>{{ achievement }}</li>
                {% endfor %}
              </ul>
            </div>
          </div>
          
          <!-- Move2Cloud -->
          <div class="position-card">
            <div class="position-header">
              <h4 class="position-title">{% t experience.timeline.coexya.move2cloud.title %}</h4>
              <div class="position-meta">
                <span class="period">{% t experience.timeline.coexya.move2cloud.period %}</span>
                <span class="team-size">{% t experience.timeline.coexya.move2cloud.team %}</span>
              </div>
            </div>
            
            <div class="tech-stack">
              <span class="tech-tag">Azure</span>
              <span class="tech-tag">Kubernetes</span>
              <span class="tech-tag">Docker</span>
              <span class="tech-tag">CI/CD</span>
              <span class="tech-tag">Azure Resource Manager (ARM)</span>
              <span class="tech-tag">PostgreSQL</span>
              <span class="tech-tag">Ingress nginx</span>
            </div>
            
            <div class="responsibilities">
              <p><strong>{% t experience.timeline.coexya.move2cloud.mission %}</strong> {% t experience.timeline.coexya.move2cloud.mission_value %}</p>
              
              <h5>{% t experience.timeline.coexya.move2cloud.achievements_title %}</h5>
              <ul class="achievements-list">
                {% assign achievements = site.translations[site.lang].experience.timeline.coexya.move2cloud.achievements %}
                {% for achievement in achievements %}
                  <li>{{ achievement }}</li>
                {% endfor %}
              </ul>
            </div>
          </div>

          <!-- Alerte Technique & Reflet Parc -->
          <div class="position-card">
            <div class="position-header">
              <h4 class="position-title">{% t experience.timeline.coexya.alerte_reflet.title %}</h4>
              <div class="position-meta">
                <span class="period">{% t experience.timeline.coexya.alerte_reflet.period %}</span>
                <span class="team-size">{% t experience.timeline.coexya.alerte_reflet.team %}</span>
              </div>
            </div>

            <div class="tech-stack">
              <span class="tech-tag">Flutter</span>
              <span class="tech-tag">.NET Core</span>
              <span class="tech-tag">Azure DevOps</span>
              <span class="tech-tag">Static Web App</span>
              <span class="tech-tag">Azure API Management</span>
              <span class="tech-tag">ARM</span>
              <span class="tech-tag">CI/CD</span>
              <span class="tech-tag">PostgreSQL</span>
              <span class="tech-tag">Swagger/OpenAPI</span>
              <span class="tech-tag">Azure AD</span>
            </div>

            <div class="responsibilities">
              <p><strong>{% t experience.timeline.coexya.alerte_reflet.methodology %}</strong> {% t experience.timeline.coexya.alerte_reflet.methodology_value %}</p>

              <h5>{% t experience.timeline.coexya.alerte_reflet.products_title %}</h5>
              <ul class="project-list">
                <li>{% t experience.timeline.coexya.alerte_reflet.products.alerte_technique.title %}
                  <ul>
                    {% assign features = site.translations[site.lang].experience.timeline.coexya.alerte_reflet.products.alerte_technique.features %}
                    {% for feature in features %}
                      <li>{{ feature }}</li>
                    {% endfor %}
                  </ul>
                </li>
                <li>{% t experience.timeline.coexya.alerte_reflet.products.reflet_parc.title %}
                  <ul>
                    {% assign features = site.translations[site.lang].experience.timeline.coexya.alerte_reflet.products.reflet_parc.features %}
                    {% for feature in features %}
                      <li>{{ feature }}</li>
                    {% endfor %}
                  </ul>
                </li>
              </ul>

              <h5>{% t experience.timeline.coexya.alerte_reflet.achievements_title %}</h5>
              <ul class="achievements-list">
                {% assign achievements = site.translations[site.lang].experience.timeline.coexya.alerte_reflet.achievements %}
                {% for achievement in achievements %}
                  <li>{{ achievement }}</li>
                {% endfor %}
              </ul>
            </div>
          </div>

          <!-- Oskar -->
          <div class="position-card">
            <div class="position-header">
              <h4 class="position-title">{% t experience.timeline.coexya.oskar.title %}</h4>
              <div class="position-meta">
                <span class="period">{% t experience.timeline.coexya.oskar.period %}</span>
                <span class="team-size">{% t experience.timeline.coexya.oskar.team %}</span>
              </div>
            </div>

            <div class="tech-stack">
              <span class="tech-tag">Java 8</span>
              <span class="tech-tag">Spring Boot 2</span>
              <span class="tech-tag">Angular 8</span>
              <span class="tech-tag">GitLab</span>
              <span class="tech-tag">PostgreSQL</span>
              <span class="tech-tag">Docker Swarm</span>
              <span class="tech-tag">DevOps</span>
              <span class="tech-tag">CI/CD</span>
            </div>

            <div class="responsibilities">
              <p><strong>{% t experience.timeline.coexya.oskar.methodology %}</strong> {% t experience.timeline.coexya.oskar.methodology_value %}</p>
              <p><strong>{% t experience.timeline.coexya.oskar.project %}</strong> {% t experience.timeline.coexya.oskar.project_value %}</p>

              <h5>{% t experience.timeline.coexya.oskar.achievements_title %}</h5>
              <ul class="achievements-list">
                {% assign achievements = site.translations[site.lang].experience.timeline.coexya.oskar.achievements %}
                {% for achievement in achievements %}
                  <li>{{ achievement }}</li>
                {% endfor %}
              </ul>
            </div>
          </div>
        </div>
      </div>

      <!-- Interpol -->
      <div class="timeline-item">
        <div class="timeline-marker">
          <div class="marker-dot"></div>
          <span class="timeline-period">{% t experience.timeline.interpol.period %}</span>
        </div>
        <div class="timeline-content">
          <div class="company-header">
            <h3 class="company-name">{% t experience.timeline.interpol.company %}</h3>
            <span class="duration">{% t experience.timeline.interpol.duration %}</span>
          </div>

          <div class="position-card">
            <div class="position-header">
              <h4 class="position-title">{% t experience.timeline.interpol.title %}</h4>
              <div class="position-meta">
                <span class="period">{% t experience.timeline.interpol.period_detail %}</span>
                <span class="team-size">{% t experience.timeline.interpol.team %}</span>
              </div>
            </div>

            <div class="tech-stack">
              <span class="tech-tag">Angular</span>
              <span class="tech-tag">Angular Material</span>
              <span class="tech-tag">NgRx</span>
              <span class="tech-tag">RxJs</span>
              <span class="tech-tag">GitLab</span>
              <span class="tech-tag">CI/CD</span>
            </div>

            <div class="responsibilities">
              <p><strong>{% t experience.timeline.interpol.mission %}</strong> {% t experience.timeline.interpol.mission_value %}</p>

              <h5>{% t experience.timeline.interpol.achievements_title %}</h5>
              <ul class="achievements-list">
                {% assign achievements = site.translations[site.lang].experience.timeline.interpol.achievements %}
                {% for achievement in achievements %}
                  <li>{{ achievement }}</li>
                {% endfor %}
              </ul>
            </div>
          </div>
        </div>
      </div>

      <!-- GiSmartware -->
      <div class="timeline-item">
        <div class="timeline-marker">
          <div class="marker-dot"></div>
          <span class="timeline-period">{% t experience.timeline.gismartware.period %}</span>
        </div>
        <div class="timeline-content">
          <div class="company-header">
            <h3 class="company-name">{% t experience.timeline.gismartware.company %}</h3>
            <span class="duration">{% t experience.timeline.gismartware.duration %}</span>
          </div>

          <div class="position-card">
            <div class="position-header">
              <h4 class="position-title">{% t experience.timeline.gismartware.title %}</h4>
              <div class="position-meta">
                <span class="period">{% t experience.timeline.gismartware.period_detail %}</span>
                <span class="team-size">{% t experience.timeline.gismartware.team %}</span>
              </div>
            </div>

            <div class="tech-stack">
              <span class="tech-tag">AngularJS</span>
              <span class="tech-tag">Cordova</span>
              <span class="tech-tag">PHP</span>
              <span class="tech-tag">IoT</span>
              <span class="tech-tag">JavaScript</span>
              <span class="tech-tag">HTML5</span>
              <span class="tech-tag">CSS</span>
              <span class="tech-tag">Git</span>
              <span class="tech-tag">OpenLayers</span>
              <span class="tech-tag">Leaflet</span>
              <span class="tech-tag">PostgreSQL</span>
              <span class="tech-tag">PostGIS</span>
            </div>

            <div class="responsibilities">
              <p><strong>{% t experience.timeline.gismartware.methodology %}</strong> {% t experience.timeline.gismartware.methodology_value %}</p>
              <p><strong>{% t experience.timeline.gismartware.project %}</strong> {% t experience.timeline.gismartware.project_value %}</p>

              <h5>{% t experience.timeline.gismartware.achievements_title %}</h5>
              <ul class="achievements-list">
                {% assign achievements = site.translations[site.lang].experience.timeline.gismartware.achievements %}
                {% for achievement in achievements %}
                  <li>{{ achievement }}</li>
                {% endfor %}
              </ul>
            </div>
          </div>
        </div>
      </div>

      <!-- Institut G4 -->
      <div class="timeline-item">
        <div class="timeline-marker">
          <div class="marker-dot"></div>
          <span class="timeline-period">{% t experience.timeline.g4.period %}</span>
        </div>
        <div class="timeline-content">
          <div class="company-header">
            <h3 class="company-name">{% t experience.timeline.g4.company %}</h3>
            <span class="duration">{% t experience.timeline.g4.duration %}</span>
          </div>

          <div class="position-card">
            <div class="position-header">
              <h4 class="position-title">{% t experience.timeline.g4.trainer.title %}</h4>
              <div class="position-meta">
                <span class="period">{% t experience.timeline.g4.trainer.period %}</span>
              </div>
            </div>

            <div class="responsibilities">
              <h5>{% t experience.timeline.g4.trainer.trainings_title %}</h5>
              <ul class="achievements-list">
                {% assign trainings = site.translations[site.lang].experience.timeline.g4.trainer.trainings %}
                {% for training in trainings %}
                  <li>{{ training }}</li>
                {% endfor %}
              </ul>
            </div>
          </div>
        </div>
      </div>            <!-- Projets Académiques -->
      <div class="timeline-item">
        <div class="timeline-marker">
          <div class="marker-dot"></div>
          <span class="timeline-period">{% t experience.timeline.academic.other_period %}</span>
        </div>
        <div class="timeline-content">
          <div class="company-header">
            <h3 class="company-name">{% t experience.timeline.academic.other_title %}</h3>
            <span class="duration">{% t experience.timeline.academic.other_duration %}</span>
          </div>

          <div class="position-card">
            <div class="position-header">
              <h4 class="position-title">{% t experience.timeline.academic.other_subtitle %}</h4>
              <div class="position-meta">
                <span class="period">{% t experience.timeline.academic.other_period_detail %}</span>
              </div>
            </div>

            <div class="responsibilities">
              <ul class="achievements-list">
                <p><strong>{% t experience.timeline.academic.projects.runner_mobile.title %}</strong></p>
                <ul>
                  {% assign features = site.translations[site.lang].experience.timeline.academic.projects.runner_mobile.features %}
                  {% for feature in features %}
                    <li>{{ feature }}</li>
                  {% endfor %}
                </ul>
                <p><strong>{% t experience.timeline.academic.projects.events_mobile.title %}</strong></p>
                <ul>
                  {% assign features = site.translations[site.lang].experience.timeline.academic.projects.events_mobile.features %}
                  {% for feature in features %}
                    <li>{{ feature }}</li>
                  {% endfor %}
                </ul>
                <p><strong>{% t experience.timeline.academic.projects.salon_mobile.title %}</strong></p>
                <ul>
                  {% assign features = site.translations[site.lang].experience.timeline.academic.projects.salon_mobile.features %}
                  {% for feature in features %}
                    <li>{{ feature }}</li>
                  {% endfor %}
                </ul>
              </ul>
            </div>
          </div>
        </div>
      </div>

      <!-- Premiers emplois -->
      <div class="timeline-item">
        <div class="timeline-marker">
          <div class="marker-dot"></div>
          <span class="timeline-period">{% t experience.timeline.first_jobs.period %}</span>
        </div>
        <div class="timeline-content">
          <div class="company-header">
            <h3 class="company-name">{% t experience.timeline.first_jobs.company %}</h3>
          </div>

          <div class="position-card compact">
            <div class="position-header">
              <h4 class="position-title">{% t experience.timeline.first_jobs.web_enov.title %}</h4>
              <div class="position-meta">
                <span class="period">{% t experience.timeline.first_jobs.web_enov.period %}</span>
              </div>
            </div>

            <div class="tech-stack">
              <span class="tech-tag">HTML/CSS</span>
              <span class="tech-tag">Bootstrap</span>
              <span class="tech-tag">JavaScript</span>
              <span class="tech-tag">PHP</span>
              <span class="tech-tag">SQL</span>
              <span class="tech-tag">PrestaShop</span>
            </div>

            <div class="responsibilities">
              <p><strong>{% t experience.timeline.first_jobs.mission %}</strong> {% t experience.timeline.first_jobs.web_enov.mission_value %}</p>
              <h5>{% t experience.timeline.first_jobs.achievements_title %}</h5>
              <ul class="achievements-list">
                {% assign achievements = site.translations[site.lang].experience.timeline.first_jobs.web_enov.achievements %}
                {% for achievement in achievements %}
                  <li>{{ achievement }}</li>
                {% endfor %}
              </ul>
            </div>
          </div>

          <div class="position-card compact">
            <div class="position-header">
              <h4 class="position-title">{% t experience.timeline.first_jobs.paquet.title %}</h4>
              <div class="position-meta">
                <span class="period">{% t experience.timeline.first_jobs.paquet.period %}</span>
              </div>
            </div>

            <div class="tech-stack">
              <span class="tech-tag">HTML/CSS</span>
              <span class="tech-tag">Bootstrap</span>
              <span class="tech-tag">JavaScript</span>
              <span class="tech-tag">PHP</span>
              <span class="tech-tag">SQL</span>
              <span class="tech-tag">XML</span>
              <span class="tech-tag">Git</span>
              <span class="tech-tag">GitHub</span>
              <span class="tech-tag">SFTP</span>
            </div>

            <div class="responsibilities">
              <p><strong>{% t experience.timeline.first_jobs.mission %}</strong> {% t experience.timeline.first_jobs.paquet.mission_value %}</p>
              <p><strong>{% t experience.timeline.first_jobs.team %}</strong> {% t experience.timeline.first_jobs.paquet.team_value %}</p>
              <h5>{% t experience.timeline.first_jobs.achievements_title %}</h5>
              <ul class="achievements-list">
                {% assign achievements = site.translations[site.lang].experience.timeline.first_jobs.paquet.achievements %}
                {% for achievement in achievements %}
                  <li>{{ achievement }}</li>
                {% endfor %}
              </ul>
            </div>
          </div>

          <div class="position-card compact">
            <div class="position-header">
              <h4 class="position-title">{% t experience.timeline.first_jobs.lyon1.title %}</h4>
              <div class="position-meta">
                <span class="period">{% t experience.timeline.first_jobs.lyon1.period %}</span>
              </div>
            </div>

            <div class="tech-stack">
              <span class="tech-tag">HTML/CSS</span>
              <span class="tech-tag">Bootstrap</span>
              <span class="tech-tag">JavaScript</span>
              <span class="tech-tag">PHP</span>
              <span class="tech-tag">SQL</span>
              <span class="tech-tag">XML</span>
              <span class="tech-tag">Git</span>
              <span class="tech-tag">GitHub</span>
            </div>

            <div class="responsibilities">
              <p><strong>{% t experience.timeline.first_jobs.project %}</strong> {% t experience.timeline.first_jobs.lyon1.project_value %}</p>
              <p><strong>{% t experience.timeline.first_jobs.team %}</strong> {% t experience.timeline.first_jobs.lyon1.team_value %}</p>
              <h5>{% t experience.timeline.first_jobs.achievements_title %}</h5>
              <ul class="achievements-list">
                {% assign achievements = site.translations[site.lang].experience.timeline.first_jobs.lyon1.achievements %}
                {% for achievement in achievements %}
                  <li>{{ achievement }}</li>
                {% endfor %}
              </ul>
            </div>
          </div>
        </div>
      </div>

    </div>

  </div>
</section>

<!-- Formation Section -->
<section class="education-section">
  <div class="container">
    <h2 class="section-title">{% t education.title %}</h2>
    <div class="education-grid">
      <div class="education-card">
        <div class="education-header">
          <h3 class="school-name">{% t education.g4.school %}</h3>
          <span class="period">{% t education.g4.period %}</span>
        </div>
        <p class="degree">{% t education.g4.degree %}</p>
        <p class="field">{% t education.g4.field %}</p>
      </div>
      
      <div class="education-card">
        <div class="education-header">
          <h3 class="school-name">{% t education.licence.school %}</h3>
          <span class="period">{% t education.licence.period %}</span>
        </div>
        <p class="degree">{% t education.licence.degree %}</p>
      </div>
      
      <div class="education-card">
        <div class="education-header">
          <h3 class="school-name">{% t education.dut.school %}</h3>
          <span class="period">{% t education.dut.period %}</span>
        </div>
        <p class="degree">{% t education.dut.degree %}</p>
      </div>
    </div>
  </div>
</section>

<!-- Call to Action -->
<section class="footer">
  <div class="container">
    <div class="cta-content">
      <h2 class="cta-title">{% t cta.title %}</h2>
      <p class="cta-description">{% t cta.description %}</p>
      <div class="cta-actions">
        <a href="https://linkedin.com/in/benoit-rongeard-678258100" target="_blank" class="btn-primary">
          <svg width="20" height="20" fill="currentColor" viewBox="0 0 24 24">
            <path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/>
          </svg>
          <span>{% t cta.contact %}</span>
        </a>
        {% if site.lang == "en" %}
          {% capture home_link %}{{ site.baseurl_root }}/en{% endcapture %}
        {% else %}
          {% capture home_link %}{{ site.baseurl_root }}{% endcapture %}
        {% endif %}
        <a href="{{ home_link }}" class="btn-primary btn-exp">
          <svg width="20" height="20" fill="currentColor" viewBox="0 0 24 24">
            <path d="M10 20v-6h4v6h5v-8h3L12 3 2 12h3v8z"/>
          </svg>
          <span>{% t cta.home %}</span>
        </a>
      </div>
    </div>
  </div>
</section>
