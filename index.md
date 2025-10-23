---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<img class="profile-picture" src="assets/profile_picture.jpg">

Hi! I'm Nitin, a CS PhD Student at [The University of Texas at Austin](https://www.utexas.edu/), where I'm advised by [Prof. Aditya Akella](https://www.cs.utexas.edu/~akella/index.html). My research interests lie at the intersection of computer systems and machine learning.

Before UT, I was a [Pre-Doctoral Research Fellow](https://www.microsoft.com/en-us/research/people/t-nitinkedia/) in the [AI Infrastructure group](https://www.microsoft.com/en-us/research/project/ai-infrastructure/) at [Microsoft Research, India](https://www.microsoft.com/en-us/research/lab/microsoft-research-india/), where I worked with [Dr. Ramachandrandran Ramjee](https://www.microsoft.com/en-us/research/people/ramjee/), [Dr. Jayashree Mohan](https://www.microsoft.com/en-us/research/people/jamohan/), [Dr. Ashish Panwar](https://www.microsoft.com/en-us/research/people/ashishpanwar/) and [Dr. Nipun Kwatra](https://www.microsoft.com/en-us/research/people/nkwatra/). My research focus was on optimizing Large Language Model (LLM) inference there.

Previously, I was a Senior Software Engineer at [Zeta](https://zeta.tech), [a unicorn startup modernizing legacy banking systems with a cloud-native stack](https://aws.amazon.com/solutions/case-studies/zeta-amazon-eks/). During my three years there, I scaled their multi-tenant web application platform and developed Zeta’s API Playground.

I graduated with a B.Tech. in Computer Science and Engineering from [IIT Guwahati](https://iitg.ac.in/) in 2020. I have fond memories of competing in programming contests at [Codeforces](https://codeforces.com/profile/nk7). See this [repo](https://github.com/nitinkedia7/competitive-coding) for fast plug-n-play data structures and algorithm implementations in C++.


## Publications
{% for pub in site.data.publications | sort: "order" %}

**[{{ pub.title }}]({{ pub.url }})**  
{{ pub.authors }}  
{% if pub.type == "preprint" %}_Preprint_  {% elsif pub.venue %}*{{ pub.venue }}*  {% endif %}
[PDF]({{ pub.pdf }}) / [Code]({{ pub.code }})

{% endfor %}
