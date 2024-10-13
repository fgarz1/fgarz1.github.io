---
layout: default
---

Text can be **bold**, _italic_, ~~strikethrough~~ or `keyword`.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# secuirty operations center (SOC)

My very first project will be creating my own, very simple, security operations center. To creat my own SOC, I will be using Microsft Azure. I start off by creating a virtual machine using the preset configuration option on Azure. Keep in mind, I left RDP open for this virtual machine. After that, I configured an SIEM in the form of microsoft sentinel. I set up a data connector to receieve the logs from my VM; I used Windows Security Events via AMA. I created a rule on microsfot sentinel to alert me of any successful local sign ins every five minutes: 'SecurityEvent|where Activity contains "success" and Account !contains "system".' I excluded any system sign ins on this rule.
### Incident Alert
![Sentinel Alert](https://github.com/fgarz1/fgarz1.github.io/blob/main/Sentinel%20Alert.jpg)
