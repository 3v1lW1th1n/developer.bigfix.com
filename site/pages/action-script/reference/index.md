---
title: Reference
categories:
  - title: Client Commands
    section: client
    description: The [client commands](./client/) allow you to control the behavior of the BigFix client.
    commands:
      - notify client
      - administrator add
      - administrator delete
      - notify client
      - relay select
      - restart
      - set clock
      - setting
      - setting delete
      - shutdown
      - site force evaluation
      - subscribe
      - unsubscribe
  - title: Download Commands
    section: download
    description: The [download commands](./download/) allow you to download files to the client machine.
    commands:
      - download
      - download as
      - execute prefetch plug-in
  - title: Execution Commands
    section: execution
    description: The [execution commands](./execution/) allow you to run external commands and control their behavior.
    commands:
      - action launch preference low-priority
      - action launch preference normal-priority
      - dos
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
      - appendfile
      - archive now
      - copy
      - createfile until
      - delete
      - extract
      - move
      - utility
  - title: Registry Commands
    section: registry
    description: The [registry commands](./registry/) allow you edit the Windows Registry.
    commands:
      - regdelete
      - regdelete64
      - regset
      - regset64
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
