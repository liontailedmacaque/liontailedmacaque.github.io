---
layout: page
---

<!---
<img src="/assets/homepage/SnailBrightSmall2.jpg" height="100%" width="100%" style="margin: 0px 0px 20px 0px; float: center;">
--->

<h3>Books</h3>

<a href="https://smile.amazon.com/dp/B0BR9DQMVS"><img src="/assets/homepage/ChessCover4.png" height="25%" width="25%" style="margin: 0px 10px 20px 0px; float: left;">
<b>The Chess Memory Palace</b></a> explains how to use advanced memory techniques to learn chess openings. Available as [a paper copy](https://smile.amazon.com/dp/B0BR9DQMVS) or [an ebook](https://www.etsy.com/listing/1368398070).
<div style="clear: both;"></div>

<a href="https://smile.amazon.com/Curious-Letter-Nebuchadnezzar-John-Holden/dp/B09FS5DSJK"><img src="/assets/homepage/NebCover2.png" height="25%" width="25%" style="margin: 0px 10px 20px 0px; float: left;">
<b>A Curious Letter from Nebuchadnezzar</b></a> is a retelling of chapter 4 of the Book of Daniel, from the Bible, in rhyme and pictures. Available as [a paper copy](https://smile.amazon.com/Curious-Letter-Nebuchadnezzar-John-Holden/dp/B09FS5DSJK).
<div style="clear: both;"></div>

<h3>Blog</h3>

{% for post in site.posts %}
<span class="date-home">({{ post.date | date: "%Y/%m" }})</span> [{{ post.title }}]({{ post.url }}) <br>
{% endfor %}
