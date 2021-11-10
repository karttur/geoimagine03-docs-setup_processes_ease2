---
layout: article
title: regions-ease2ntiles_v090.json
categories: setup_processes
excerpt:  Link default regions to EASE2 North grid tiles
tags:: 
    - regions-ease2ntiles
date: 2021-11-10
modified: 2021-11-10
comments: true
share: true
---

# regions ease2ntiles (setup_processes)

###  Link default regions to EASE2 North grid tiles

The json command file <span class='file'>regions-ease2ntiles_v090.json</span> is part of karttur's GeoImagine project <span class='project'>setup_processes</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

```
{
  "userproject": {
    "userid": "karttur",
    "projectid": "karttur",
    "tractid": "karttur",
    "siteid": "*",
    "plotid": "*",
    "system": "ease2n"
  },
  "period": {
    "timestep": "static"
  },
  "process": [
    {
      "processid": "LinkDefaultRegionTiles",
      "overwrite": false,
      "version": "0.9",
      "verbose": 2,
      "parameters": {
        "defregmask": "global"
        },
      "srcpath": {
        "volume": "DEMDATA",
        "hdr": "shp",
        "dat": "shp"
      },
      "srccomp": [
        {
          "regions": {
            "source": "karttur",
            "product": "roi",
            "content": "pubroi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "v010"
          }
        }
      ]
    }
  ]
}
```
