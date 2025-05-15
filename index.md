---
layout: page
---

<h3>Books</h3>

<a href="{{ site.amazon_book_url_chessmemorypalace }}"><img src="/assets/homepage/ChessCover4.png" height="25%" width="25%" style="margin: 0px 10px 20px 0px; float: left;">
<b>The Chess Memory Palace</b></a> explains how to use advanced memory techniques to learn chess openings. Available as <a href="{{ site.amazon_book_url_chessmemorypalace }}">paperback</a> or [ebook](https://chessmemorypalace.etsy.com) -- [or read the first 3 chapters online](/chessmemorypalace). Subscribe to [@ChessMemoryPalace on YouTube](https://www.youtube.com/@ChessMemoryPalace) for video tutorials.

{% include a-affiliate-note.html %}
<div style="clear: both;"></div>

<a href="{{ site.amazon_book_url_nebuchadnezzar }}"><img src="/assets/homepage/NebCover2.png" height="25%" width="25%" style="margin: 0px 10px 20px 0px; float: left;">
<b>A Curious Letter from Nebuchadnezzar</b></a> is a retelling of Chapter 4 of the Book of Daniel, from the Bible, in rhyme and pictures. Available as <a href="{{ site.amazon_book_url_nebuchadnezzar }}">paperback</a>.
<div style="clear: both;"></div>

<h3>Blog</h3>

{% for post in site.posts %}
<span class="date-home">({{ post.date | date: "%Y/%m" }})</span> [{{ post.title }}]({{ post.url }}) <br>
{% endfor %}

  <!-- Subscription form in its own wrapper -->
  <div class="index-subscribe" style="margin-top: 2rem;">
    {% include subscribe.html %} 
  </div>

<!---
<img src="/assets/homepage/SnailBrightSmall2.jpg" height="100%" width="100%" style="margin: 0px 0px 20px 0px; float: center;">
--->

<h3>Contact</h3>

[Click here to contact me](https://docs.google.com/forms/d/e/1FAIpQLScYNyYMXEeDmbTU0U2UCoyCN1fyd7xRho3S-ddgzg6S6a3bLw/viewform?usp=sf_link)
