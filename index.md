---
buttons:
  - text: "Twitter"
    url: "https://twitter.com/username"
    class: "button-twitter"  # Class dari brands.css untuk styling
  - text: "GitHub"
    url: "https://github.com/username"
    class: "button-github"
---

<!-- Konten HTML lainnya tetap -->

<div class="button-stack" role="navigation">
  {% for button in page.buttons %}
    <a href="{{ button.url }}" class="button {{ button.class }}">{{ button.text }}</a>
  {% endfor %}
</div>