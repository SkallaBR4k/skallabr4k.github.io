---
layout: default
---

# Hi, I'm Skalla

I'm a Linux sysadmin and DevOps engineer. Here I share:

- Infrastructure automation projects
- Linux troubleshooting guides  
- DevOps tools and workflows
- Random technical experiments

## Recent Posts

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <span>{{ post.date | date: "%b %-d, %Y" }}</span> — 
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
