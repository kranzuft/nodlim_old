---
layout: root
title: Exercises
heading: Programming Exercises w/ Solutions 
quote: Programming languages express computations in a form comprehensible to both people and machines.
qauth: Robert Harper
qcite: https://www.cs.cmu.edu/~rwh/plbook/2nded.pdf
---

<hr>

Below is the table of contents for all programming challenge books. Solutions are included for all problems. Most problems are for the absolute beginner, but experts can refresh their skills, and compare their solutions to our own. If you believe your solution is superiour to our own, please <a href="{{ site.github.url }}/contact/">contact</a> us.

<nav class="tocnav">
  {% for matter in site.collections %}
  {% if matter.topic != NULL %}
  <hr>
  <strong>
      <a href="{{ site.github.url }}/{{ matter.label }}/index">
      BOOK {{ matter.booknum }}: {{ matter.title }}
    </a>
  </strong>
  <ol> 
    {% for doc in matter.docs %}
    {% if doc.questions != null %}
    <li class="tocnav section">
      <a href="{{ site.github.url }}/{{ matter.label }}/{{ doc.section }}/">
        {{ doc.title }}
      </a>
    </li>
    {% endif %}
    {% endfor %} 
  </ol>
  {% endif %}
  {% endfor %}
</nav>
