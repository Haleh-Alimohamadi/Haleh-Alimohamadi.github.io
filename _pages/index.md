---
layout: single
title: "All About Chris"
excerpt: "Homepage"
author_profile: true
permalink: /
twitter: true
---
I received my Ph.D. from the Department of Computer Science and Engineering at the University of California, San Diego (UCSD). My research interests are brain-inspired computing, machine learning acceleration, computer architecture, and embedded systems. 
The outputs of my research have been published in over 100 top conferences/journals and opened a new direction for enabling fast and robust general intelligence. My Ph.D. research was the main initiative to open a recent $5M DARPA program focusing on brain-inspired computing (HyDDENN). As a graduate student, I have received the most prestigious awards from both Computer science department and school of engineering at UC San Diego. In 2019, my research has been recognized with the Bernard and Sophia Gordon Engineering Leadership Award, the Outstanding Researcher Award, and the Powell Fellowship by the Jacob School of Engineering (among over 1.4K graduate students). I have also received the Best Doctorate Research in Computer Science at UC San Diego in 2018, the Best Presentation Award in 2019 PhD Forum at Design Automation Conference (DAC), and several Best Paper Nomination Awards at multiple conferences including DAC 2019, DAC 2020, and DATE 2020. 

<h1>Latest Posts</h1>
{% assign sorted = site.posts | sort:'date' | reverse %}
<ul>
{% for post in sorted limit:3%}
	<div class="{{ include.type | default: "list" }}__item">
	  <article class="archive__item" itemscope itemtype="http://schema.org/CreativeWork">
	    <li>
	      <h3 class="archive__item-title" itemprop="headline">
			 	  <a href="{{ root_url }}{{ post.url }}">{{ post.title }}</a>
	      </h3>
        <p class="archive__item-excerpt" itemprop="description">{{post.excerpt}}</p>
	    </li>
	 </article>
	</div>
{% endfor %}
<ul>
<a href="/blog/" class="back-to-top">More posts &rarr;</a>

