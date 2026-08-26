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
.pub-year { color: DarkRed !important; margin: 1.4em 0 0.2em 0 !important; font-size: 1.5em !important; }
.pub-rule { height: 1px; border: none; background-color: #333; margin: 0 0 1.1em 0; }
.pub-item { display: grid; grid-template-columns: 135px 1fr; gap: 1.1em;
  align-items: start; margin-bottom: 1.5em; }
.pub-thumb img { width: 100%; border: 1px solid #e5e5e5; border-radius: 4px; display: block; }
.pub-thumb-placeholder { display: flex; align-items: center; justify-content: center;
  min-height: 62px; padding: 0.5em; border: 1px solid; border-radius: 4px;
  font-size: 0.8em; font-weight: bold; text-align: center; line-height: 1.3; }
.pub-title { font-weight: bold; font-size: 1.02em; line-height: 1.35; }
.pub-authors { font-size: 0.88em; color: #444; margin-top: 0.25em; }
.pub-meta { margin-top: 0.35em; }
.pub-pill { display: inline-block; padding: 0.1em 0.55em; border: 1px solid;
  border-radius: 3px; font-size: 0.78em; font-weight: bold; vertical-align: middle; }
.pub-venue { font-size: 0.84em; color: #777; font-style: italic; margin-left: 0.5em; }
.pub-excerpt { font-size: 0.85em; color: #666; line-height: 1.5; margin-top: 0.4em; }
.pub-links { margin-top: 0.4em; font-size: 0.85em; }
.pub-links a { margin-right: 0.6em; }
@media (max-width: 600px) {
  .pub-item { grid-template-columns: 1fr; gap: 0.6em; }
  .pub-thumb { max-width: 240px; }
}
.pub-preprints { margin: 0.2em 0 0.6em 0; padding-left: 1.3em; }
.pub-preprints li { margin-bottom: 0.55em; line-height: 1.5; }
.pub-prep-title { font-weight: bold; font-size: 0.98em; }
.pub-prep-pill { display: inline-block; padding: 0.1em 0.55em; margin-left: 0.45em;
  border: 1px solid #aaaaaa; border-radius: 3px; background-color: #f2f2f2;
  color: #555555; font-size: 0.74em; font-weight: bold; vertical-align: middle;
  white-space: nowrap; }
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
<p style="font-size: 0.9em;">You can also find my articles on <a href="{{ author.googlescholar }}"><u>my Google Scholar profile</u></a>. Jump to: <a href="#preprints">Preprints</a> · 
{% for y in years %}<a href="#y{{ y }}">{{ y }}</a>{% unless forloop.last %} · {% endunless %}{% endfor %}</p>
{% endif %}

<h2 class="pub-year" id="preprints">Working Preprints</h2>
<hr class="pub-rule" />
<ol class="pub-preprints">
  <li><span class="pub-prep-title">MIU: A Mutual Information Framework for Unlearning</span><span class="pub-prep-pill">In preparation</span></li>
  <li><span class="pub-prep-title">Theoretical Foundations of Machine Unlearning</span><span class="pub-prep-pill">In preparation</span></li>
</ol>

{% for y in years %}
<h2 class="pub-year" id="y{{ y }}">{{ y }}</h2>
<hr class="pub-rule" />
{% for post in pubs %}{% if post.year == y %}{% include archive-single-publication.html %}{% endif %}{% endfor %}
{% endfor %}
