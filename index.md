---
layout: page
---

<img src="/assets/homepage/Snail.jpg" height="50%" width="100%" style="margin: 0px 0px 20px 0px; float: center;">

<h3>Books</h3>

<a href="https://www.amazon.co.uk/Curious-Letter-Nebuchadnezzar-John-Holden/dp/B09FS5DSJK?pldnSite=1"><img src="/assets/homepage/Nebuchadnezzar.jpg" height="25%" width="25%" style="margin: 0px 10px 20px 0px; float: left;">
<b>A Curious Letter from Nebuchadnezzar</b></a> is a retelling of chapter 4 of the Book of Daniel, from the Bible, in rhyme and pictures.
<div style="clear: both;"></div>

<h3>Blog</h3>

{% for post in site.posts %}
<span class="date-home">({{ post.date | date: "%Y/%m" }})</span> [{{ post.title }}]({{ post.url }}) <br>
{% endfor %}
