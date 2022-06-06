---
layout: default
title: polishDB
subtitle: knitting, coding, making and other related stuff
permalink: /polish/
---

<section class="filter-simple">

<div class="grid-container">
	<div class="grid-x grid-padding-x margin-x">
		<div class="large-12 cell">
			<div>
				<div class="button-group round">
					<button class="button hollow filter-simple-button is-active" data-filter="all">All</button>
					<button class="button hollow filter-simple-button" data-filter="Sparkly">Sparkly</button>
					<button class="button hollow filter-simple-button" data-filter="Glitter">Glitter</button>
					<button class="button hollow filter-simple-button" data-filter="Matte">Matte</button>
					<button class="button hollow filter-simple-button" data-filter="Jelly">Jelly</button>
					<button class="button hollow filter-simple-button" data-filter="Texture">Texture</button>
					<button class="button hollow filter-simple-button" data-filter="Plate">Plate</button>
				</div>
			</div>
		</div>
{% for polish in site.data.polishes %}
		<div class="cell small-12 medium-6 large-4 card filter-simple-item {{polish.finishprimary}}">
		  <div class="polish-card-thumbnail" style="padding:5px; background-color:rgb({{polish.rgb}});">
			<a href="#">{{polish.colorwheel}}</a>
		  </div>
		  <h2 class="polish-card-title"><a href="https://www.google.com/search?site=imghp&tbm=isch&q={{polish.polishname}}">{{polish.polishname}}</a></h2>
		  <span class="polish-card-desc">{{polish.desc}}</span>
		  <span class="polish-card-price">{{polish.line}} ({{polish.mfr}})</span>
		</div>
{% endfor %}
	</div>
</div>
</section>

