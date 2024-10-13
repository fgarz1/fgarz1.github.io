# Decription
This is where I will be documenting different projects I work on as my career in cyber security progresses. 

# secuirty operations center (SOC)

My very first project will be creating my own, very simple, security operations center. To create my own SOC, I will be using Microsoft Azure. I start off by creating a virtual machine using the preset configuration option on Azure. Keep in mind, I left RDP open for this virtual machine. After that, I configured an SIEM in the form of microsoft sentinel. I set up a data connector to receieve the logs from my VM; I used Windows Security Events via AMA. I created a rule on microsfot sentinel to alert me of any successful local sign ins every five minutes: 'SecurityEvent|where Activity contains "success" and Account !contains "system".' I excluded any system sign ins on this rule. After I login in to the vm via RDP I recieve an inicdent alert on microsft sentinel thus my SIEM is successfully active.
