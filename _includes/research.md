<h1 id="research"></h1>

<h2 style="margin: 60px 0px -15px;">Research</h2>

<div class="research">
<ol class="bibliography">

{% for link in site.data.research.main %}

<li>
<div class="pub-row" style="padding-top: 5px;">
  <div class="col-sm-9 abbr" style="position: relative;padding-right: 15px; padding-left: 15px;">
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1"> 
            <abbr class="badge">{{ link.journal_short }}</abbr>
  </div>
  <div class="col-sm-3" style="position: relative; padding-left: 15px;">
      <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
      <div class="description">{{ link.description }}</div>
  </div>
</div>
</li>

<br>

{% endfor %}

</ol>
</div>


