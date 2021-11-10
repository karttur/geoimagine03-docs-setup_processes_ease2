---
layout: article
title: ancillary-import-ease2_v090.json
categories: setup_processes
excerpt:  Import the shape file with the EASE2N in native projection
tags:: 
    - ancillary-import-ease2
date: 2021-11-10
modified: 2021-11-10
comments: true
share: true
---

# ancillary import ease2 (setup_processes)

###  Import the shape file with the EASE2N in native projection

The json command file <span class='file'>ancillary-import-ease2_v090.json</span> is part of karttur's GeoImagine project <span class='project'>setup_processes</span>. Calling the json file will execute the following commands of the GeoImagine Framework.

```
{
  "userproject": {
    "userid": "karttur",
    "projectid": "karttur",
    "tractid": "karttur",
    "siteid": "*",
    "plotid": "*",
    "system": "ancillary"
  },
  "period": {
    "timestep": "static"
  },
  "process": [
    {
      "processid": "OrganizeAncillary",
      "overwrite": false,
      "parameters": {
        "importcode": "shp",
        "epsg": "6931",
        "orgid": "karttur",
        "dsname": "modistiles",
        "dsversion": "1.0",
        "accessdate": "20211109",
        "regionid": "globe",
        "regioncat": "globe",
        "dataurl": "",
        "metaurl": "",
        "title": "EASE 2 North tiles",
        "label": "EASE 2 North tiles inn ative projection"
      },
      "srcpath": {
        "volume": ".",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstpath": {
        "volume": "DEMDATA",
        "hdr": "shp",
        "dat": "shp"
      },
      "srcraw": [
        {
          "modtiles": {
            "datadir": "data/ease2n",
            "datafile": "6931tiles-multi_karttur_epsg6931",
            "datalayer": "tiles",
            "title": "EASE 2 North tiles",
            "label": "EASE 2 North tiles inn ative projection"
          }
        }
      ],
      "dstcomp": [
        {
          "modtiles": {
            "source": "karttur",
            "product": "ease2ntiles",
            "content": "tiles",
            "layerid": "ease2ntiles",
            "prefix": "ease2ntiles",
            "suffix": "epsg6931",
            "dataunit": "tile",
            "celltype": "vector",
            "cellnull": "0",
            "measure": "N",
            "masked": "N"
          }
        }
      ]
    },
    {
      "processid": "OrganizeAncillary",
      "overwrite": false,
      "parameters": {
        "importcode": "shp",
        "epsg": "6932",
        "orgid": "karttur",
        "dsname": "modistiles",
        "dsversion": "1.0",
        "accessdate": "20211109",
        "regionid": "globe",
        "regioncat": "globe",
        "dataurl": "",
        "metaurl": "",
        "title": "EASE 2 South tiles",
        "label": "EASE 2 South tiles in native projection"
      },
      "srcpath": {
        "volume": ".",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstpath": {
        "volume": "DEMDATA",
        "hdr": "shp",
        "dat": "shp"
      },
      "srcraw": [
        {
          "modtiles": {
            "datadir": "data/ease2s",
            "datafile": "6932tiles-multi_karttur_epsg6932",
            "datalayer": "tiles",
            "title": "EASE 2 South tiles",
            "label": "EASE 2 South tiles in native projection"
          }
        }
      ],
      "dstcomp": [
        {
          "modtiles": {
            "source": "karttur",
            "product": "ease2stiles",
            "content": "tiles",
            "layerid": "ease2stiles",
            "prefix": "ease2stiles",
            "suffix": "epsg6932",
            "dataunit": "tile",
            "celltype": "vector",
            "cellnull": "0",
            "measure": "N",
            "masked": "N"
          }
        }
      ]
    },
    {
      "processid": "OrganizeAncillary",
      "overwrite": false,
      "parameters": {
        "importcode": "shp",
        "epsg": "6933",
        "orgid": "karttur",
        "dsname": "modistiles",
        "dsversion": "1.0",
        "accessdate": "20211109",
        "regionid": "globe",
        "regioncat": "globe",
        "dataurl": "",
        "metaurl": "",
        "title": "EASE 2 Tropical tiles",
        "label": "EASE 2 Tropical tiles in native projection"
      },
      "srcpath": {
        "volume": ".",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstpath": {
        "volume": "DEMDATA",
        "hdr": "shp",
        "dat": "shp"
      },
      "srcraw": [
        {
          "modtiles": {
            "datadir": "data/ease2t",
            "datafile": "6933tiles-multi_karttur_epsg6933",
            "datalayer": "tiles",
            "title": "EASE 2 Tropical tiles",
            "label": "EASE 2 Tropical tiles in native projection"
          }
        }
      ],
      "dstcomp": [
        {
          "modtiles": {
            "source": "karttur",
            "product": "ease2ttiles",
            "content": "tiles",
            "layerid": "ease2ttiles",
            "prefix": "ease2ttiles",
            "suffix": "epsg6933",
            "dataunit": "tile",
            "celltype": "vector",
            "cellnull": "0",
            "measure": "N",
            "masked": "N"
          }
        }
      ]
    }
  ]
}
```
