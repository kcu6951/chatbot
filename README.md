# chatbot
김채운

<style>
  df-messenger {
   --df-messenger-bot-message: #D6F7FC;
   --df-messenger-chat-background-color: #EFF6F6;
   --df-messenger-input-box-color: #EFF1F1;
   --df-messenger-font-color: black;
   --df-messenger-user-message: #FBF7B9;
  }
</style>
    
    {% if site.google_analytics %}
      <script async src="https://www.googletagmanager.com/gtag/js?id={{ site.google_analytics }}"></script>
      <script>
        window.dataLayer = window.dataLayer || [];
        function gtag(){dataLayer.push(arguments);}
        gtag('js', new Date());
        gtag('config', '{{ site.google_analytics }}');
      </script>
    {% endif %}
    <meta charset="UTF-8">

{% seo %}
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link rel="preload" href="https://fonts.googleapis.com/css?family=Open+Sans:400,700&display=swap" as="style" type="text/css" crossorigin>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="theme-color" content="#157878">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <link rel="stylesheet" href="{{ '/assets/css/style.css?v=' | append: site.github.build_revision | relative_url }}">
  </head>
  <body>
    <a id="skip-to-content" href="#content">Skip to the content.</a>

    <header class="page-header" role="banner">
      <h1 class="project-name">{{ page.title | default: site.title | default: site.github.repository_name }}</h1>
      <h2 class="project-tagline">{{ page.description | default: site.description | default: site.github.project_tagline }}</h2>
      {% if site.github.is_project_page %}
        <a href="{{ site.github.repository_url }}" class="btn">View on GitHub</a>
      {% endif %}
      {% if site.show_downloads %}
        <a href="{{ site.github.zip_url }}" class="btn">Download .zip</a>
        <a href="{{ site.github.tar_url }}" class="btn">Download .tar.gz</a>
      {% endif %}
    </header>

    <main id="content" class="main-content" role="main">
      {{ content }}

      <footer class="site-footer">
        {% if site.github.is_project_page %}
          <span class="site-footer-owner"><a href="{{ site.github.repository_url }}">{{ site.github.repository_name }}</a> is maintained by <a href="{{ site.github.owner_url }}">{{ site.github.owner_name }}</a>.</span>
        {% endif %}
        <span class="site-footer-credits">This page was generated by <a href="https://pages.github.com">GitHub Pages</a>.</span>
      </footer>
    </main>
  </body>
</html>
