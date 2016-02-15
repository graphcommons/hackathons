---
layout: post
language: en
title:      "Hackathon Documentation: Creative use of Complex Networks, Istanbul"
subtitle:   "Documentation from Jan 9-10, 2016"
author:     "Graph Commons"
header-img: "img/istanbul-2016/hackathon2.jpg"
description:"Documentation of Hackathon Creative use of Complex Networks, Istanbul, January 9-10th, 2016"
---

We organized a two-day hackathon "[Creative Use of Complex Networks](https://graphcommons.github.io/hackathons/2015/12/23/istanbul-creative-use-of-complex-networks/)" hosted by [ATOLYE Istanbul](http://atolyeistanbul.co/roof/#atolyeeng) on Jan 9-10, 2016. Participants created semantic network models, built graph databases, and developed graph-driven applications to map and analyze complex issues in civil society. We think civil society would benefit from having their own methods and tools to collectively imagine and author new protocols and create new interfaces that would compose large-scale civic networks and data streams. Below is selected work from the hackathon with short explanations, links to interactive maps, code repositories, data sources, screenshots, and photos.

*[Graph Commons](https://graphcommons.com/) is a collaborative network mapping platform and a knowledge base of relationships. With Graph Commons you transform your data into interactive network maps and connect partial information to explore complex relations that impact you and your communities.*

*Click on the images and titles to view the interactive graphs.*

---

## Turkey's Parliamentary Minutes Graph

https://graphcommons.com/graphs/de6e0fd9-e5a6-42ac-86ad-b98c5a5d15ed?show=graph

This graph maps the reactions of political parties to the MP speeches given in Turkey's parliament (TBMM). The full speech is typed by official parliament reporters and published on the TBMM website daily. The minute text includes reactions such as laughter, bullying, applause, and protests from various parties to the speaking MP. In the graph, green nodes represent the speech, red nodes are MPs, blue nodes are political parties. You can start exploring the graph by clicking on a speech node that is at the center, which means it got negative or positive reactions from many parties.

The graph is generated (and being updated) by a TBMM-to-graph application called "[Parliamentary Minutes](https://github.com/graphs-for-society/parliamentary-minutes)" developed by Doruk Tunaoğlu, Fevzi Kahraman, Onur Güngör, and Osman Başkaya. It has modules for data crawling, information extraction, and graph creation. The group also developed a path searching interface, where you can look up an MP and a party and see if there are any reaction paths exist between them. This application along with last hackathon's [TBMM scraper aka "bureaucracy graph generator"](https://github.com/meclistakip/tbmm-scraper) provides a graph-structured activity stream of Turkey's parliament.

Data source: http://tbmm.gov.tr
Code repository: https://github.com/graphs-for-society/parliamentary-minutes
Using Python wrapper for Graph Commons API: https://github.com/graphcommons/graphcommons-python

Also see Turkey's political chronology database
https://github.com/fatiherikli/turkiye-siyasi-kronoloji

---

## Metagraph

https://graphcommons.com/graphs/9d3f1540-a963-4496-9763-82c4b0c76ef6

Metagraph, created by [Yakup Cetinkaya](https://github.com/ta6o), is a graph of similar graphs in the [Networks of Dispossession hub](https://graphcommons.com/hubs/mulksuzlestirme), which contains 22 public graphs. It interconnects graphs based on the number of shared nodes, which are represented as connection weights. You can see clearly energy related graphs are closely connected to each other. This work is a great reflection of how Graph Commons hubs work. You build a networked knowledge base by importing, adding, and collectively editing data over time. The knowledge base itself is a giant graph, not visual and not telling a story, it is rather a data world that you build. Using the hub explore feature, you explore actors and relations you're interested, and generate particular graphs which frame a different aspect of the database, hence tell a particular digestible story from the whole.

Data source: [Graph Commons API](https://graphcommons.com/dev)
Code repository: https://github.com/ta6o/metagraph
Using Ruby Wrapper for Graph Commons API: https://github.com/graphcommons/graphcommons-ruby

---

## Githubbers network of repositories and collaborations

https://graphcommons.com/graphs/0df3be5d-dcfd-4040-b002-0a504d36d176

Network map of code repositories on Github connected via shared contributors and languages used in the project. Created by [Kerem Gunes](https://github.com/k-gun), the Githubbers graph counts the number of commits by each contributor and the percentage of programming languages used in the project, which are then used as weights of the connections. In the graph, red nodes are repositories, blue nodes are programming languages, and the black nodes are contributors. Using the graph filter you can focus your view to observe only the stronger contributor and language connections.

This graph is generated by the [Githubbers application](https://github.com/k-gun/githubbers) which collects data via Github API and generates graphs using the Graph Commons API.

Data source: Github API
Code repository: https://github.com/k-gun/githubbers
Using PHP7 Wrapper for Graph Commons API: https://github.com/graphcommons/graphcommons-php7

---

## Mapping Turkey-Russia Commercial Relationships

This graph contains the companies registered in Turkey and trade goods with Russia. Created by [Koray Taylan](https://github.com/koraytaylan), this graph presents the potential damage on certain sectors due to the conflict between Russia and Turkey.

Data source: kap.gov.tr, all the public companies listed in the stock exchange. http://www.kap.gov.tr/sirketler/islem-goren-sirketler/tum-sirketler.aspx
Using Node.js Wrapper for Graph Commons API: https://github.com/igaln/graphcommons-node

## Graph of electric vehicles

https://graphcommons.com/graphs/176f94b1-417b-4b69-81d4-abf9b0582107

This graph sketch, also created by Koray Taylan, shows which car brand produces which new electric car model. It could be improved by adding common properties of these electric car models. Do they have auto parking capability? Do they have auto-pilot capability? Are they part of a charging station network? etc.

---

## SmartPro academy structure graph

https://graphcommons.com/graphs/7ef928a8-9853-41fc-a05c-e784a4a13c37

Network map of the organizational structure of [SmartPro Academy](http://www.smartpro.com.tr/). It shows how courses are organized around tutors and topics as well as the hiring companies who partners with the academy.

---

## Digital cultural ecologies in urban settings

https://graphcommons.com/graphs/ba4a19b1-b37a-4ece-a27b-f42db527804c

Initiated by [Asli Telli Aydemir](https://twitter.com/aslitelli), this graph attempts generate a workable taxonomy of digital culture assets for medium-sized cities in Turkey.

---

## 3D graphs with OpenFrameWorks

https://vimeo.com/151791682

An OpenFrameWorks graph viewer, developed by Serkan Sokmen, renders any graph from Graph Commons as a 3D network visualization. As you may know, 3D visualizations are asked a lot, but not preferred for network mapping, because 3D camera view prevents clear comparison of the sizes of the nodes that are in the back vs at the front. However, first-person shooter camera gaze is great for flying through a three dimensional network space. Also instead of relying on radius for representing important nodes, it is recommended to use a metaphor of star constellations, that is to say use internal illumination of node spheres to represent degree centrality.


## Mapping Slack chat conversations

https://graphcommons.com/graphs/cf021d76-70d8-4179-805f-dca822a11ee9

We've built a @graphbot that maps public conversations, who mentions whom, and who is active in which channel in your Slack team.


---

## Presentations

"How to use Graph Commons API" by Ahmet Kızılay

https://gitlab.com/ahmetkizilay/hackathon-sunum

"Getting started with Cypher and Neo4j" by Tuna Vargi

---

## Graph Commons API Wrappers

- [Ruby Wrapper](https://github.com/ta6o/graphcommons-ruby) initiated by Yakup Cetinkaya

- [Python Wrapper](https://github.com/graphcommons/graphcommons-python) initiated by Fatih Erikli

- [Node.js Wrapper](https://github.com/igaln/graphcommons-node) initiated by Igal Nassima

- [PHP7 Wrapper](https://github.com/graphcommons/graphcommons-php7) and [PHP Wrapper](https://github.com/graphcommons/graphcommons-php) initiated by Kerem Güneş

Graph Commons API Documentation, Libraries & Examples
https://graphcommons.github.io/api-v1/#libraries-amp-examples

---
