---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<style>
.pub-stats { margin: 0.4em 0 1.6em 0; font-size: 0.9em; color: #555; }
.pub-stats .s { display: inline-block; padding: 0.15em 0.6em; margin-right: 0.4em;
  border: 1px solid #dcdcdc; border-radius: 12px; background-color: #fafafa; }
.pub-year { color: DarkRed !important; margin: 1.5em 0 0.2em 0 !important; font-size: 1.5em !important; }
.pub-rule { height: 1px; border: none; background-color: #333; margin: 0 0 1.2em 0; }

.pub-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 1.1em; }

.pub-tile { display: flex; flex-direction: column; overflow: hidden;
  border: 1px solid #e2e2e2; border-top: 3px solid #52adc8; border-radius: 8px;
  background-color: #fff;
  transition: transform 0.25s ease, box-shadow 0.25s ease, border-color 0.25s ease; }
.pub-tile:hover { transform: translateY(-5px); box-shadow: 0 8px 22px rgba(0,0,0,0.14); }
.pub-tile.journal { border-top-color: #62c462; }
.pub-tile.workshop { border-top-color: #f89406; }
.pub-tile.preprint { border-top-color: #aaaaaa; }

.pub-banner { position: relative; overflow: hidden; background-color: #fbfbfb;
  border-bottom: 1px solid #eee; height: 150px; }
.pub-banner img { width: 100%; height: 150px; object-fit: contain; padding: 8px;
  display: block; transition: transform 0.35s ease; }
.pub-tile:hover .pub-banner img { transform: scale(1.06); }
.pub-banner-empty { display: flex; align-items: center; justify-content: center; height: 150px;
  background: linear-gradient(135deg, #eef7fa 0%, #f7fbfc 100%); }
.pub-banner-empty span { font-weight: bold; color: #7fa9b8; font-size: 1.15em;
  letter-spacing: 0.03em; text-align: center; padding: 0 0.6em; }
.pub-pill { position: absolute; top: 8px; right: 8px; padding: 0.15em 0.6em;
  border-radius: 3px; background-color: rgba(255,255,255,0.93); border: 1px solid #52adc8;
  color: #39798c; font-size: 0.74em; font-weight: bold; }
.pub-tile.journal .pub-pill { border-color: #62c462; color: #458945; }
.pub-tile.workshop .pub-pill { border-color: #f89406; color: #ae6804; }
.pub-tile.preprint .pub-pill { border-color: #aaaaaa; color: #555; }

.pub-content { display: flex; flex-direction: column; flex: 1; padding: 0.85em 1em 0.9em 1em; }
.pub-title { font-weight: bold; font-size: 0.98em; line-height: 1.35; }
.pub-authors { font-size: 0.82em; color: #555; margin-top: 0.3em; line-height: 1.45; }

.pub-abs { margin-top: 0.55em; }
.pub-abs > summary { cursor: pointer; display: inline-block; list-style: none;
  padding: 0.12em 0.6em; border: 1px solid #d5d5d5; border-radius: 12px;
  background-color: #f7f7f7; color: #555; font-size: 0.76em; font-weight: bold;
  transition: background-color 0.2s ease, border-color 0.2s ease; }
.pub-abs > summary::-webkit-details-marker { display: none; }
.pub-abs > summary::after { content: " \25BE"; }
.pub-abs[open] > summary::after { content: " \25B4"; }
.pub-abs > summary:hover { background-color: #eef7fa; border-color: #52adc8; color: #39798c; }
.pub-abs-body { font-size: 0.83em; color: #666; line-height: 1.55; margin-top: 0.5em; }

.pub-links { margin-top: auto; padding-top: 0.7em; font-size: 0.8em; }
.pub-links a { margin-right: 0.7em; font-weight: bold; }
.pub-venue-full { display: block; margin-top: 0.4em; color: #999; font-style: italic;
  font-size: 0.95em; line-height: 1.4; }

@media (prefers-reduced-motion: reduce) {
  .pub-tile, .pub-banner img { transition: none; }
  .pub-tile:hover { transform: none; }
  .pub-tile:hover .pub-banner img { transform: none; }
}
</style>

{% assign pubs = site.publications | sort: 'date' | reverse %}
{% assign years = site.publications | map: 'year' | uniq | sort | reverse %}
{% assign n_conf = site.publications | where: 'type', 'conference' | size %}
{% assign n_jour = site.publications | where: 'type', 'journal' | size %}
{% assign n_work = site.publications | where: 'type', 'workshop' | size %}

<div class="pub-stats">
  <span class="s">📚 {{ site.publications | size }} papers</span>
  <span class="s">🎤 {{ n_conf }} conference</span>
  <span class="s">📖 {{ n_jour }} journal</span>
  <span class="s">🛠️ {{ n_work }} workshop</span>
</div>

{% if author.googlescholar %}
<p style="font-size: 0.9em;">You can also find my articles on <a href="{{ author.googlescholar }}"><u>my Google Scholar profile</u></a>. Jump to:
{% for y in years %}<a href="#y{{ y }}">{{ y }}</a>{% unless forloop.last %} · {% endunless %}{% endfor %}</p>
{% endif %}

{% for y in years %}
<h2 class="pub-year" id="y{{ y }}">{{ y }}</h2>
<hr class="pub-rule" />
<div class="pub-grid">
{% for post in pubs %}{% if post.year == y %}{% include archive-single-publication.html %}{% endif %}{% endfor %}
</div>
{% endfor %}
