---
layout: layout
---

<html lang="en">
<head>

  <!-- Basic Page Needs
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->

  <meta charset="utf-8">
  <title>Anton McConville - Digital Designer and Developer</title>
  <meta name="description" content="">
  <meta name="author" content="">

  <!-- Mobile Specific Metas
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->

  <meta name="viewport" content="width=device-width, initial-scale=1">

  <!-- FONT
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->

  <!-- <link href="https://fonts.googleapis.com/css?family=Ropa+Sans" rel="stylesheet" type="text/css"> -->

  <link href="https://fonts.googleapis.com/css?family=Karla" rel="stylesheet">
  <!-- CSS
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link rel="stylesheet" href="css/normalize.css">
  <!-- <link rel="stylesheet" href="css/skeleton.css"> -->
  <link rel="stylesheet" href="css/anton.css">

  <!-- Favicon
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->

  <link rel="icon" type="image/png" href="images/favicon.png">

  <!-- Global site tag (gtag.js) - Google Analytics -->

  <script async src="https://www.googletagmanager.com/gtag/js?id=UA-135798241-1"></script>

  <script>
    window.dataLayer = window.dataLayer || [];

    function gtag() {
      dataLayer.push(arguments);
    }
    gtag('js', new Date());

    gtag('config', 'UA-135798241-1');
  </script>

</head>

<body>
  <div class="top">
    <div class="bar">
      <a href="./index.html">
        <div class="title">
          <div class="name">Anton McConville</div>
          <div class="subtitle">Digital Designer & Developer</div>
        </div>
      </a>
      <div class="navigation">
        <a class="selected" href="index.html">projects</a>
        <a class="deselected end" href="pages/about.html">about</a>
      </div>
    </div>
  </div>
  <div class="control">
    <div class="content">
      <div class="related">
        <ul>
          {% for post in site.posts %}
          <li>
    	     <span>{{ post.date | date: "%B %e, %Y" }}</span>
           <a href="{{ post.url | prepend:'/blog' }}">{{ post.title }}</a>
          </li>
          {% endfor %}
        </ul>
      </div>
    </div>
  </div>
</body>
</html>
