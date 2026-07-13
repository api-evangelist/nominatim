---
title: "New Wikimedia-based scoring file available"
url: "https://nominatim.org/2024/08/07/wikimedia-file.html"
date: "2024-08-07"
author: "Marc Tobias (mtmail)"
feed_url: "https://nominatim.org/feed.xml"
---
Nominatim tries to assign each place in its database a base “importance” score number to answer the question “If 30 places have the name ‘Berlin’, which one is the most likely a user meant?” For Berlin that’s the one in Germany. We humans say “of course” but that’s not how computers work. Looking at a places’ type (city vs village), size, OpenStreetMap tags, population all have disadvantages, usually simply lacking a good data source for the whole world.
