<h1 id="research"></h1>

<h2 style="margin: 60px 0px -15px;">Research</h2>

<div class="research">
<ol class="bibliography">

{% for link in site.data.research.main %}

<li>
<div class="pub-row">
  <div class="col-sm-9 abbr" style="position: relative;padding-right: 15px; padding-left: 15px;">
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1"> 
            <abbr class="badge">{{ link.journal_short }}</abbr>
  </div>
  <div class="col-sm-3" style="position: relative; padding-left: 15px;">
      <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.journal }}</em>
      </div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>

<br>

{% endfor %}

</ol>
</div>


