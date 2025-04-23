---
layout: page
---

  <!-- Subscription form in its own wrapper -->
  <div class="index-subscribe">
    {% include subscribe.html %} 
  </div>

<h3>Books</h3>

<a href="https://smile.amazon.com/dp/B0BR9DQMVS"><img src="/assets/homepage/ChessCover4.png" height="25%" width="25%" style="margin: 0px 10px 20px 0px; float: left;">
<b>The Chess Memory Palace</b></a> explains how to use advanced memory techniques to learn chess openings. Available as [paperback](https://smile.amazon.com/dp/B0BR9DQMVS) or [ebook](https://www.etsy.com/listing/1368398070) -- [or read the first 3 chapters online](/chessmemorypalace). Subscribe to [@ChessMemoryPalace on YouTube](https://www.youtube.com/@ChessMemoryPalace) for video tutorials.
<div style="clear: both;"></div>

<a href="https://smile.amazon.com/Curious-Letter-Nebuchadnezzar-John-Holden/dp/B09FS5DSJK"><img src="/assets/homepage/NebCover2.png" height="25%" width="25%" style="margin: 0px 10px 20px 0px; float: left;">
<b>A Curious Letter from Nebuchadnezzar</b></a> is a retelling of Chapter 4 of the Book of Daniel, from the Bible, in rhyme and pictures. Available as [paperback](https://smile.amazon.com/Curious-Letter-Nebuchadnezzar-John-Holden/dp/B09FS5DSJK).
<div style="clear: both;"></div>

<h3>Blog</h3>

{% for post in site.posts %}
<span class="date-home">({{ post.date | date: "%Y/%m" }})</span> [{{ post.title }}]({{ post.url }}) <br>
{% endfor %}

<!---
<img src="/assets/homepage/SnailBrightSmall2.jpg" height="100%" width="100%" style="margin: 0px 0px 20px 0px; float: center;">
--->

<h3>Contact</h3>

[Click here to contact me](https://docs.google.com/forms/d/e/1FAIpQLScYNyYMXEeDmbTU0U2UCoyCN1fyd7xRho3S-ddgzg6S6a3bLw/viewform?usp=sf_link)
