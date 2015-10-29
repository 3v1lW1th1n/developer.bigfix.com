---
title: Reference
categories:
  - title: Execution Commands
    section: execution
    description: The [execution commands](./execution/) allow you to run external commands and control their behavior.
    commands:
      - action launch preference low-priority
      - action launch preference normal-priority
      - dos
      - notify client
      - override
      - run
      - rundetached
      - runhidden
      - script
      - script64
      - wait
      - waitdetached
      - waithidden
  - title: File Commands
    section: file
    description: The [file commands](./file/) allow you copy, move, and delete files.
    commands:
      - copy
      - move
      - delete
---

{% for category in categories %}
<div>
  <h2>{{category.title}}</h2>
  {{category.description}}
  <ul>
    {% for command in category.commands %}
    <li><a href="/action-script/reference/{{category.section}}/{{command | replace(' ', '-')}}.html">{{command}}</a></li>
    {% endfor %}
  </ul>
</div>
{% endfor %}
