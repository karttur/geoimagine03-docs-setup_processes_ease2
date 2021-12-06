---
layout: article
title: regions-ease2stiles_v090.json
categories: setup_processes
excerpt: \# Link default regions to EASE-grid 2 South grid tiles
tags:: 
    - json/regions-ease2stiles
date: 2021-12-06
modified: 2021-12-06
comments: true
share: true
---

# json/regions ease2stiles (setup_processes)

### \# Link default regions to EASE-grid 2 South grid tiles

The json command file <span class='file'>regions-ease2stiles_v090.json</span> is part of karttur's GeoImagine project <span class='project'>setup_processes</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

```
{
  "userproject": {
    "userid": "karttur",
    "projectid": "karttur",
    "tractid": "karttur",
    "siteid": "*",
    "plotid": "*",
    "system": "ease2s"
  },
  "period": {
    "startyear": 2014,
    "endyear": 2014,
    "timestep": "singleyear"
  },
  "process": [
    {
      "processid": "LinkDefaultRegionTiles",
      "overwrite": false,
      "version": "0.9",
      "verbose": 2,
      "parameters": {
        "defregmask": "global",
        "regioncat": "continent",
        "cmdpath": "/usr/local/bin",
        "ogr2ogr": true,
        "clipsrc": "-180,-90,180,0",
        "clipdst": false,
        "checkfixvalidity": true,
        "onlyregionsfullywithinsystem": false
      },
      "srcpath": {
        "volume": "DEMDATA",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstpath": {
        "volume": "DEMDATA"
      },
      "srccomp": [
        {
          "regions": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "tol@1km"
          }
        }
      ],
      "dstcomp": [
        {
          "region": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "tol@1km"
          }
        }
      ]
    },
    {
      "processid": "LinkDefaultRegionTiles",
      "overwrite": false,
      "version": "0.9",
      "verbose": 2,
      "parameters": {
        "defregmask": "global",
        "regioncat": "subcontinent",
        "cmdpath": "/usr/local/bin",
        "ogr2ogr": true,
        "clipsrc": "-180,-90,180,0",
        "clipdst": false,
        "checkfixvalidity": true,
        "onlyregionsfullywithinsystem": false
      },
      "srcpath": {
        "volume": "DEMDATA",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstpath": {
        "volume": "DEMDATA"
      },
      "srccomp": [
        {
          "regions": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "tol@1km"
          }
        }
      ],
      "dstcomp": [
        {
          "region": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "tol@1km"
          }
        }
      ]
    },
    {
      "processid": "LinkDefaultRegionTiles",
      "overwrite": false,
      "version": "0.9",
      "verbose": 2,
      "parameters": {
        "defregmask": "global",
        "regioncat": "country",
        "cmdpath": "/usr/local/bin",
        "ogr2ogr": true,
        "clipsrc": "-180,-90,180,0",
        "clipdst": false,
        "checkfixvalidity": true,
        "onlyregionsfullywithinsystem": false
      },
      "srcpath": {
        "volume": "DEMDATA",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstpath": {
        "volume": "DEMDATA"
      },
      "srccomp": [
        {
          "regions": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "tol@100m"
          }
        }
      ],
      "dstcomp": [
        {
          "region": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "tol@100m"
          }
        }
      ]
    },
    {
      "processid": "LinkDefaultRegionTiles",
      "overwrite": false,
      "version": "0.9",
      "verbose": 2,
      "parameters": {
        "defregmask": "global",
        "regioncat": "continentcountry",
        "cmdpath": "/usr/local/bin",
        "ogr2ogr": true,
        "clipsrc": "-180,-90,180,0",
        "clipdst": false,
        "checkfixvalidity": true,
        "onlyregionsfullywithinsystem": false
      },
      "srcpath": {
        "volume": "DEMDATA",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstpath": {
        "volume": "DEMDATA"
      },
      "srccomp": [
        {
          "regions": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "tol@100m"
          }
        }
      ],
      "dstcomp": [
        {
          "region": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "tol@100m"
          }
        }
      ]
    },
    {
      "processid": "LinkDefaultRegionTiles",
      "overwrite": false,
      "version": "0.9",
      "verbose": 2,
      "parameters": {
        "defregmask": "global",
        "regioncat": "marinecontinent",
        "cmdpath": "/usr/local/bin",
        "ogr2ogr": true,
        "clipsrc": "-180,-90,180,0",
        "clipdst": false,
        "checkfixvalidity": true,
        "onlyregionsfullywithinsystem": false
      },
      "srcpath": {
        "volume": "DEMDATA",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstpath": {
        "volume": "DEMDATA"
      },
      "srccomp": [
        {
          "regions": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "0"
          }
        }
      ],
      "dstcomp": [
        {
          "region": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "0"
          }
        }
      ]
    },
    {
      "processid": "LinkDefaultRegionTiles",
      "overwrite": false,
      "version": "0.9",
      "verbose": 2,
      "parameters": {
        "defregmask": "global",
        "regioncat": "marinesubcontinent",
        "cmdpath": "/usr/local/bin",
        "ogr2ogr": true,
        "clipsrc": "-180,-90,180,0",
        "clipdst": false,
        "checkfixvalidity": true,
        "onlyregionsfullywithinsystem": false
      },
      "srcpath": {
        "volume": "DEMDATA",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstpath": {
        "volume": "DEMDATA"
      },
      "srccomp": [
        {
          "regions": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "0"
          }
        }
      ],
      "dstcomp": [
        {
          "region": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "0"
          }
        }
      ]
    },
    {
      "processid": "LinkDefaultRegionTiles",
      "overwrite": false,
      "version": "0.9",
      "verbose": 2,
      "parameters": {
        "defregmask": "global",
        "regioncat": "marinecountry",
        "cmdpath": "/usr/local/bin",
        "ogr2ogr": true,
        "clipsrc": "-180,-90,180,0",
        "clipdst": false,
        "checkfixvalidity": true,
        "onlyregionsfullywithinsystem": false
      },
      "srcpath": {
        "volume": "DEMDATA",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstpath": {
        "volume": "DEMDATA"
      },
      "srccomp": [
        {
          "regions": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "0"
          }
        }
      ],
      "dstcomp": [
        {
          "region": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "0"
          }
        }
      ]
    },
    {
      "processid": "LinkDefaultRegionTiles",
      "overwrite": false,
      "version": "0.9",
      "verbose": 2,
      "parameters": {
        "defregmask": "global",
        "regioncat": "marinecontinentcountry",
        "cmdpath": "/usr/local/bin",
        "ogr2ogr": true,
        "clipsrc": "-180,-90,180,0",
        "clipdst": false,
        "checkfixvalidity": true,
        "onlyregionsfullywithinsystem": false
      },
      "srcpath": {
        "volume": "DEMDATA",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstpath": {
        "volume": "DEMDATA"
      },
      "srccomp": [
        {
          "regions": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "0"
          }
        }
      ],
      "dstcomp": [
        {
          "region": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "0"
          }
        }
      ]
    },
    {
      "processid": "LinkDefaultRegionTiles",
      "overwrite": false,
      "version": "0.9",
      "verbose": 2,
      "parameters": {
        "defregmask": "global",
        "regioncat": "global",
        "cmdpath": "/usr/local/bin",
        "ogr2ogr": true,
        "clipsrc": "-180,-90,180,0",
        "clipdst": false,
        "checkfixvalidity": true,
        "onlyregionsfullywithinsystem": true
      },
      "srcpath": {
        "volume": "DEMDATA",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstpath": {
        "volume": "DEMDATA"
      },
      "srccomp": [
        {
          "regions": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "0"
          }
        }
      ],
      "dstcomp": [
        {
          "region": {
            "source": "karttur",
            "product": "karttur",
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "suffix": "0"
          }
        }
      ]
    }
  ]
}
```
