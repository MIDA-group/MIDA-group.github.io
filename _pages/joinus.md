---
layout: infolab-toplevel
title: Join Us
permalink: /joinus/
header:
  overlay_image: /assets/images/banner_small.jpg
  overlay_filter: "0.4"
toc: true
---

# Open positions

[//]: # (At our lab we host a limited number of thesis projects, listed below. Those working on these projects become temporary members of the lab, are expected to complete the project under the agreed time constraints (typically 2.5 months for bachelors and 5 months for masters) and to actively participate in the lab activities, so that they can contribute to information sharing and knowledge development. Bachelor/Master students are expected to work full time on the project, that is, around 40 hours per week. A high degree of independence, ambition and linguistic skills (English) are necessary, as all projects are part of the research activities of the lab and are expected to contribute to it with new knowledge, algorithms, code, etc. If you are interested, please send an email to the person responsible for the project incuding your transcript, a CV, and a short motivation.)


{% for poslist in site.data.positions %}
## {{ poslist.level }}

{% for pos in poslist.positions %}
{% if pos.status == "open" %}
**{{ pos.title }}**<br/>
Description: {{ pos.author }}<br/>
Requirements: {{ pos.author }}<br/>
Contact: {{ pos.author }}<br/>
{% if pos.url != nil %}<a href="{{ pos.url }}">More info</a>{% endif %}
{% endif %}
{% endfor %}

{% endfor %}

# Before joining

This section collects some information about life in Sweden and about how we work, that can be useful if you are interested in joining the lab as a PhD student or postdoc.

- **A comparative study of fairness-aware community detection methods** With the growing interest in the field of algorithmic fairness, various approaches have been recently introduced to partition graphs into clusters while simultaneously satisfying fairness constraints. This project aims to study and experimentally compare these methods, their scalability, as well as the effect of different demographic fairness functions. For info, contact Georgios: georgios.panayiotou@it.uu.se

[//]: # (- **Generation of large-scale social networks of formal ties** In the Data Mining course (prerequisite for this project), you have seen the ER model, which can be used to generate simple graphs. This is a fundamental model to generate random (and thus unrealistic) networks, that can be used to understand whether what we see in real networks is a result of randomness or an actual signal to be analysed. The objective of this project is to define and implement a model that can generate realistic data about formal social ties (that is: family ties, same-workplace, same-school, same-neighborhood, etc.). The work will start with a kind of “multilayered” ER-like model, and define (and implement) a sequence of more and more realistic models by adding non-random assumptions about the distribution of the ties (just as an example, things such as: higher probability of having family ties when people live close by and go to the same school, then longitudinal information about how links evolve in time, etc.). A computational challenge is that this model must be able to generate large data – with 10 to 20 million individuals and billions of ties. This is part of a project where we use registry data to generate population-scale social networks to study segregation and other sociological problems. We need this work both to share data (because we are of course not allowed to share the real data), and to make hypotheses about how such data is generated. For info, contact Matteo.)

# Before joining

This section collects some information about life in Sweden and about how we work, that can be useful if you are interested in joining the lab.

## Working and living in Sweden

Sweden is a fantastic place for living and working. Swedes are friendly and speak excellent English.  The quality of life is high, with a strong emphasis on outdoor activities.  The Swedish working climate emphasises an open atmosphere, with active discussions involving both junior and senior staff.  Spouses of employees are entitled to work permits. Healthcare is free after a small co-pay and the university subsidises athletic costs, such as a gym membership.  The parental benefits in Sweden are among the best in the world, including extensive parental leave (for both parents), paid time off to care for sick children, and affordable daycare.  For more information, be sure to read <a href="https://www.uu.se/en/about-uu/join-us/advantages" target="_new">Why choose Sweden?</a> and <a href="https://www.uu.se/en/about-uu/join-us/why-uppsala-university" target="_new">Why choose Uppsala University?</a>.

## Expected availability from Infolab members

Given the creative nature of part of our work, Infolab members are generally free to work when and where it best fits them, compatibly with tasks requiring presence (e.g., teaching) and regulations that may be enforced by the Department or University.

At the same time, everyone is expected to contribute to the lab, which implies being available to give feedback, sharing their current research with other members (see below), and participating in lab meetings.

Lab members are free to take time to work offline. In particular, it is not necessary to be continuously online on our Slack space. Checking the Slack at least once a day is however expected, and if one cannot be online for a few days for any reason (e.g. holidays) it is good practice to inform the other lab members.

## Research quality at the Infolab

While "quality" is a subjective term, and we expect lab members to reflect about this concept and adopt their own definitions of quality, we also have some guidelines to ensure that some common ground is established. In particular, we want our research to be based on appropriate methods, clearly and transparently communicated, developed with ethical and societal awareness, replicable (when possible), and usable by others.

To achieve this, research at Infolab is organised into *research activities*. A research activity is anything leading to a published article, a grant proposal, a PhD dissertation, an undergraduate thesis, research software, etc. Each research activity is led by a member of the lab, who is the *contact author* and is responsible for the research to advance and for its quality. Under normal circumstances, the contact author should be available to answer questions about the activity and its outcomes for at least two years after the outcome has been made public, even in case of a change of affiliation.

Members of the lab should feel a responsibility of getting and receiving feedback from other members. At the beginning of a new research activity, the (contact) author(s) should pitch the idea to the other lab members, who should be available to provide constructive feedback. Before submitting a paper or research proposal the authors are invited to share it with the other lab members, who should be available to provide constructive feedback. Getting feedback even earlier is also encouraged, although not expected.

At submission time, for all products containing experiments the code to replicate the experiments should be made available in a repository in the Infolab's git workspace, in an easy-to-execute format (with exceptions, for example double-blind review processes).

## Authorship

Each research activity must have a clear list of authors. At the Infolab we define authors as in: "each author is expected to have made substantial contributions to the conception or design of the work; or the acquisition, analysis, or interpretation of data; or the creation of new software used in the work; or have drafted the work or substantively revised it; AND to have approved the submitted version (and any substantially modified version that involves the author’s contribution to the study); AND to have agreed both to be personally accountable for the author’s own contributions and to ensure that questions related to the accuracy or integrity of any part of the work, even ones in which the author was not personally involved, are appropriately investigated, resolved, and the resolution documented in the literature."[^1]

[^1]: Transparency in authors’ contributions and responsibilities to promote integrity in scientific publication. Marcia K. McNutt, Monica Bradford, Jeffrey M. Drazen, Brooks Hanson, BobHoward, Kathleen Hall Jamieson, Véronique Kiermer, Emilie Marcus, Barbara Kline Pope, Randy Schekman, Sowmya Swaminathan, Peter J. Stang, Inder M. Verma. Proceedings of the National Academy of Sciences Mar 2018, 115 (11) 2557-2560; DOI:10.1073/pnas.1715374115

## Start-up checklist

When joining the lab:

1. If you are not already in Uppsala, make sure you start looking for an accommodation well in advance, this can take time.
1. A current faculty member will register you to our internal systems.
    * Slack (we do not normally use email for communication).
    * The lab's Git space (please provide your git account).
    * Group storage space.
1. Follow the Twitter and Facebook accounts of the lab, if you use these social media for work.
