---
layout: post
language: en
title: "Hackathon Documentation: Creative use of Complex Networks, Istanbul"
subtitle: "Documentation from Jan 9-10, 2016"
author: "Graph Commons"
header-img: "img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-2.jpg"
description: "Documentation of Hackathon Creative use of Complex Networks, Istanbul, January 9-10th, 2016"
---

We organized a two-day hackathon "[Creative Use of Complex Networks](https://graphcommons.github.io/hackathons/2015/12/23/istanbul-creative-use-of-complex-networks/){:target="_blank"}" hosted by [ATOLYE Istanbul](http://atolyeistanbul.co/roof/#atolyeeng){:target="_blank"} on Jan 9-10, 2016. Participants created semantic network models, built graph databases, and developed graph-driven applications to map and analyze complex issues in civil society. We think civil society would benefit from having their own methods and tools to collectively imagine and author new protocols and create new interfaces that would compose large-scale civic networks and data streams. Below is selected work from the hackathon with short explanations, links to interactive maps, code repositories, data sources, screenshots, and photos.

*[Graph Commons](https://graphcommons.com/){:target="_blank"} is a collaborative network mapping platform and a knowledge base of relationships. With Graph Commons you transform your data into interactive network maps and connect partial information to explore complex relations that impact you and your communities.*

*Click on the images and titles to view the interactive graphs.*

---

## Turkey's Parliamentary Minutes Graph

<a href="https://graphcommons.com/graphs/de6e0fd9-e5a6-42ac-86ad-b98c5a5d15ed?show=graph" target="_blank"><img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/Meclis-Konusmalari-tbmm-parliament-minutes-graphcommons.png"></a>

<a href="https://graphcommons.com/graphs/de6e0fd9-e5a6-42ac-86ad-b98c5a5d15ed?show=graph" target="_blank"><img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/Meclis-Konusmalari-tbmm-parliament-minutes-graphcommons-1.png"></a>

<a href="https://graphcommons.com/graphs/de6e0fd9-e5a6-42ac-86ad-b98c5a5d15ed?show=graph" target="_blank"><img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/Meclis-Konusmalari-tbmm-parliament-minutes-graphcommons-2.png"></a>

<a href="https://graphcommons.com/graphs/de6e0fd9-e5a6-42ac-86ad-b98c5a5d15ed?show=graph" target="_blank"><img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/Meclis-Konusmalari-tbmm-parliament-minutes-graphcommons-3.png"></a>

[Parliamentary Minutes Graph](https://graphcommons.com/graphs/de6e0fd9-e5a6-42ac-86ad-b98c5a5d15ed?show=graph){:target="_blank"} maps the reactions of political parties to the MP speeches given in Turkey's parliament (TBMM). The full speech is typed by official parliament reporters and published on the TBMM website daily. The minute text includes reactions such as laughter, bullying, applause, and protests from various parties to the speaking MP. In the graph, green nodes represent the speech, red nodes are MPs, blue nodes are political parties. You can start exploring the graph by clicking on a speech node that is at the center, which means it got negative or positive reactions from many parties.

The graph is generated (and being updated) by a TBMM-to-graph application called "[Parliamentary Minutes](https://github.com/graphs-for-society/parliamentary-minutes){:target="_blank"}" developed by Doruk Tunaoğlu, Fevzi Kahraman, Onur Güngör, and Osman Başkaya. It has modules for data crawling, information extraction, and graph creation. The group also developed a path searching interface, where you can look up an MP and a party and see if there are any reaction paths exist between them. This application along with last hackathon's [TBMM scraper aka "bureaucracy graph generator"](https://github.com/meclistakip/tbmm-scraper){:target="_blank"} provides a graph-structured activity stream of Turkey's parliament. Also see [Turkey's political chronology database](https://github.com/fatiherikli/turkiye-siyasi-kronoloji){:target="_blank"} compiled by Fatih Erikli.


- Data source: [http://tbmm.gov.tr](http://tbmm.gov.tr){:target="_blank"}
- Code repository: [https://github.com/graphs-for-society/parliamentary-minutes](https://github.com/graphs-for-society/parliamentary-minutes){:target="_blank"}
- Graph generator: [Python wrapper for Graph Commons API](https://github.com/graphcommons/graphcommons-python){:target="_blank"}


---

## Metagraph

<a href="https://graphcommons.com/graphs/9d3f1540-a963-4496-9763-82c4b0c76ef6" target="_blank"><img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/Metagraph-mulksuzlestirme-graphcommons.png"></a>

[Metagraph](https://graphcommons.com/graphs/9d3f1540-a963-4496-9763-82c4b0c76ef6), created by [Yakup Cetinkaya](https://github.com/ta6o), is a graph of similar graphs in the [Networks of Dispossession hub](https://graphcommons.com/hubs/mulksuzlestirme), which contains 22 public graphs. It interconnects graphs based on the number of shared nodes, which are represented as connection weights. You can see clearly energy related graphs are closely connected to each other. This work is a great reflection of how Graph Commons hubs work. You build a networked knowledge base by importing, adding, and collectively editing data over time. The knowledge base itself is a giant graph, not visual and not telling a story, it is rather a data world that you build. Using the hub explore feature, you explore actors and relations you're interested, and generate particular graphs which frame a different aspect of the database, hence tell a particular digestible story from the whole.

This graph is generated by the [Metagraph application](https://github.com/graphcommons/metagraph){:target="_blank"} which collects graph data and generates meta-graphs via the Graph Commons API.

- Data source: [Graph Commons API](https://graphcommons.com/dev){:target="_blank"}
- Code repository: [https://github.com/ta6o/metagraph](https://github.com/ta6o/metagraph){:target="_blank"}
- Graph generator: [Ruby Wrapper for Graph Commons API](https://github.com/graphcommons/graphcommons-ruby){:target="_blank"}

---

## Githubbers network of repositories

<a href="https://graphcommons.com/graphs/0df3be5d-dcfd-4040-b002-0a504d36d176" target="_blank"><img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/Githubbers-graphcommons.png"></a>

<a href="https://graphcommons.com/graphs/0df3be5d-dcfd-4040-b002-0a504d36d176"><img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/Githubbers-filtered-graphcommons.png"></a>

[Githubbers](https://graphcommons.com/graphs/0df3be5d-dcfd-4040-b002-0a504d36d176){:target="_blank"} is a network map of code repositories on Github connected via shared contributors and programming languages used in the projects. Created by [Kerem Gunes](https://github.com/k-gun), the Githubbers graph counts the number of commits by each contributor and the percentage of programming languages used in the project, which are then used as weights of the connections. In the graph, red nodes are repositories, blue nodes are programming languages, and the black nodes are contributors. Using the graph filter you can focus your view to observe only the stronger contributor and language connections.

This graph is generated by the [Githubbers application](https://github.com/k-gun/githubbers){:target="_blank"} which collects data via Github API and generates graphs using the Graph Commons API.

- Data source: [Github API](https://developer.github.com/v3/){:target="_blank"}
- Code repository: [https://github.com/k-gun/githubbers](https://github.com/k-gun/githubbers){:target="_blank"}
- Graph generator: [PHP7 Wrapper for Graph Commons API](https://github.com/graphcommons/graphcommons-php7){:target="_blank"}

---

## Mapping Turkey-Russia Commercial Relationships

<a href="https://graphcommons.com/graphs/510c20ce-0e27-4928-9f65-dfb9a5db6a19" target="_blank"><img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/Rusya-Turkiye-Ticari-iliskiler.png"></a>

[This graph](https://graphcommons.com/graphs/510c20ce-0e27-4928-9f65-dfb9a5db6a19){:target="_blank"} contains the companies registered in Turkey and trade goods with Russia. Created by [Koray Taylan](https://github.com/koraytaylan){:target="_blank"}, this graph presents the potential damage on certain sectors due to the conflict between Russia and Turkey.

- Data source: [kap.gov.tr](http://www.kap.gov.tr/sirketler/islem-goren-sirketler/tum-sirketler.aspx){:target="_blank"} (public companies listed in the stock exchange)
- Graph generator: [Node.js Wrapper for Graph Commons API](https://github.com/igaln/graphcommons-node){:target="_blank"}

## Graph of electric vehicles

<a href="https://graphcommons.com/graphs/176f94b1-417b-4b69-81d4-abf9b0582107" target="_blank"><img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/ElectricVehicles.png"></a>

[This graph sketch](https://graphcommons.com/graphs/176f94b1-417b-4b69-81d4-abf9b0582107){:target="_blank"}, also created by Koray Taylan, shows which car brand produces which new electric car model. It could be improved by adding common properties of these electric car models. Do they have auto parking capability? Do they have auto-pilot capability? Are they part of a charging station network? etc.

---

## SmartPro academy structure graph

<a href="https://graphcommons.com/graphs/7ef928a8-9853-41fc-a05c-e784a4a13c37" target="_blank"><img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/SmartProEdu.png"></a>

Network map of the organizational structure of [SmartPro Academy](http://www.smartpro.com.tr/){:target="_blank"}. [This graph](https://graphcommons.com/graphs/7ef928a8-9853-41fc-a05c-e784a4a13c37){:target="_blank"} shows how courses are organized around tutors and topics as well as the hiring companies who partners with the academy.

---

## Digital cultural ecologies in urban settings

<a href="https://graphcommons.com/graphs/ba4a19b1-b37a-4ece-a27b-f42db527804c" target="_blank"><img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/DigitalCulturalEcologies-midsize-Urban.png"></a>

Initiated by [Asli Telli Aydemir](https://twitter.com/aslitelli){:target="_blank"}, [this graph](https://graphcommons.com/graphs/ba4a19b1-b37a-4ece-a27b-f42db527804c){:target="_blank"} attempts generate a workable taxonomy of digital culture assets for medium-sized cities in Turkey.

---

## 3D graph viewer

<iframe src="https://player.vimeo.com/video/151791682?title=0&byline=0&portrait=0" width="784" height="441" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

[An OpenFrameWorks graph viewer](https://vimeo.com/151791682){:target="_blank"}, developed by [Serkan Sokmen](https://vimeo.com/serkansokmen){:target="_blank"}, renders any graph from Graph Commons as a 3D network visualization. As you may know, 3D visualizations are asked a lot, but not preferred for network mapping, because 3D camera view prevents clear comparison of the sizes of the nodes that are in the back vs at the front. However, first-person shooter camera gaze is great for flying through a three dimensional network space. Also instead of relying on radius for representing important nodes, it is recommended to use a metaphor of star constellations, that is to say use internal illumination of node spheres to represent degree centrality.


## Mapping Slack chat conversations

<a href="https://graphcommons.com/graphs/cf021d76-70d8-4179-805f-dca822a11ee9" target="_blank"><img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/GraphCommons-Slack-Activity.png"></a>

[Graph Commons Slack Activity](https://graphcommons.com/graphs/cf021d76-70d8-4179-805f-dca822a11ee9){:target="_blank"} is the network map of Slack public conversations generated by [@graphbot](), which is a project we undertook at Graph Commons. When you add @graphbot to your team, it maps who mentions whom, and who is active in which channel in your Slack team. A question like "@graphbot what is your graph url?" returns the expected url. You can ask who mentioned you recently, and recommendations for a channel. We'd say Graphbot is quite effective for large communities using Slack for their collaborations.

---

## Presentations

[How to use Graph Commons API](https://gitlab.com/ahmetkizilay/hackathon-sunum){:target="_blank"} by Ahmet Kızılay

Introduction to Neo4j and Cypher by Tuna Vargı

---

## Graph Commons API Wrappers

- [Ruby Wrapper](https://github.com/ta6o/graphcommons-ruby){:target="_blank"} initiated by Yakup Cetinkaya

- [Python Wrapper](https://github.com/graphcommons/graphcommons-python){:target="_blank"} initiated by Fatih Erikli

- [Node.js Wrapper](https://github.com/igaln/graphcommons-node){:target="_blank"} initiated by Igal Nassima

- [PHP7 Wrapper](https://github.com/graphcommons/graphcommons-php7){:target="_blank"} and [PHP Wrapper](https://github.com/graphcommons/graphcommons-php){:target="_blank"} initiated by Kerem Güneş

View the [Graph Commons API Documentation](https://graphcommons.github.io/api-v1){:target="_blank"} for other Libraries & Examples.

---

## Moments from the hackathon


<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-26.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-31.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-30.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-18.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-19.jpg">


<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-0.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-1.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-2.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-4.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-5.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-8.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-9.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-10.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-11.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-12.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-24.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-13.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-14.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-15.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-17.jpg">


<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-20.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-21.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-22.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-23.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-25.jpg">


<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-27.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-28.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-29.jpg">



<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-32.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-33.jpg">

<img class="graph-image" src="{{ site.baseurl }}/img/istanbul-2016/graphcommons-hackathon2-istanbul-2016-34.jpg">


---

For questions and comments on the tools or graphs, contact the respective participants. For the Hackathon questions and comments in general contact us at the [Graph Commons Contact page](https://graphcommons.com/contact).

_This event could not be possible without [Ayça Aldatmaz](https://twitter.com/manythingoes) and [Ahmet Kızılay](https://twitter.com/ahmetkizilay)'s hard labor, our host [ATOLYE Istanbul](http://atolyeistanbul.co/roof/#atolyeeng), and an insightful presentation by [Tuna Vargi](https://github.com/vargi). We thank you all!_
