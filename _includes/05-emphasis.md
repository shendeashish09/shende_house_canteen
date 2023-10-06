*This text will be italic*
_This will also be italic_

**This text will be bold**
__This will also be bold__

_You **can** combine them_

---
food: Pizza
---

<h1>{{ page.food }}</h1>


---
name: Jane Doe
position: Developer
---
Jane has worked on Jekyll for the past *five years*.



{% for staff_member in site.staff_members %}
  <h2>{{ staff_member.name }} - {{ staff_member.position }}</h2>
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}
