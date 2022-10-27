---
title: "Research"
date: 2022-09-14T12:52:23-04:00
draft: false
---

## Current Projects

### Specified sector-wise PM$_{2.5}$ health impacts in India, 2014

High concentration of PM$_{2.5}$ in India is a growing concern in terms of its effect on human health. It is significant to evaluate how much sector-wise emission affects ambient exposure to particulate matters. Previous research focuses on main sectors like total residential emission, which is a combination of various kinds of fuels. However, posing regulations on unspecified main sectors may be unfeasible. This study aims to break down the contributions and provide better references for air-cleaning policy makers.

{{< echarts >}}

{
 "title": {
    "text": "Sector-wise Emission in India, 2014 (%)",
    "top": "4.5%",
    "left": "center",
    "textStyle": {
      "color": "black",
      "fontSize": "15"
    }
  },
  "tooltip": {
    "position": "top"
  },
  "grid": {
    "height": "80%",
    "top": "12%",
	"width": "85%",
	"left": "right"

  },
  "xAxis": {
    "type": "category",
    "data": [
        "BB", "B", "OI", "P", "T", "OA", "N",
        "DC", "S", "FC", "RC", "OR"
    ],
    "splitArea": {
      "show": true
    }
  },
  "yAxis": {
    "type": "category",
    "data": [
        "PM2.5 7.1Tg", "CO 77.3Tg", "OC 2.0Tg", "BC 1.1Tg",
        "SO2 15.1Tg", "NOx 9.8Tg", "PM10 10.1Tg", "NH3 5.2Tg"
    ],
    "splitArea": {
      "show": true
    }
  },
  "visualMap": {
    "min": 0,
    "max": 25,
    "calculable": false,
    "orient": "horizontal",
    "left": "right",
    "bottom": "89%"
  },
  "series": [
    {
      "name": "Sector",
      "type": "heatmap",
      "data": [[0,0,4.97],[1,0,6.32],[2,0,15.49],[3,0,18.55],[4,0,0.99],[5,0,0.96],[6,0,3],[7,0,17.32],[8,0,19.92],[9,0,11.28],[10,0,0.95],[11,0,0.26],[0,1,5.47],[1,1,5],[2,1,24.95],[3,1,3.81],[4,1,8.9],[5,1,0.01],[6,1,2.3],[7,1,8.07],[8,1,26.14],[9,1,14.43],[10,1,0.46],[11,1,0.47],[0,2,11.19],[1,2,7.62],[2,2,2.4],[3,2,0.57],[4,2,0.61],[5,2,0.49],[6,2,4.25],[7,2,24.08],[8,2,25.73],[9,2,20.87],[10,2,1.91],[11,2,0.3],[0,3,2.96],[1,3,23.62],[2,3,4.03],[3,3,0.83],[4,3,14.38],[5,3,2.35],[6,3,1.55],[7,3,7.92],[8,3,15.36],[9,3,23.66],[102.84,3,"-"],[110.5,3,"-"],[0,4,0.16],[1,4,"-"],[2,4,30.24],[3,4,63.19],[4,4,1.15],[5,4,0.42],[6,4,0.12],[7,4,2.71],[8,4,0.46],[9,4,0.74],[100.73,4,"-"],[110.09,4,"-"],[0,5,1.74],[1,5,1.34],[2,5,20.73],[3,5,42.48],[4,5,17.76],[5,5,3.66],[6,5,0.73],[7,5,4.06],[8,5,4.98],[9,5,1.81],[10,5,0.14],[11,5,0.56],[0,6,3.73],[1,6,9.1],[2,6,19.62],[3,6,26.24],[4,6,0.77],[5,6,0.72],[6,6,2.49],[7,6,13.23],[8,6,14.58],[9,6,8.44],[100.86,6,"-"],[11,6,0.22],[0,7,1.72],[1,7,"-"],[2,7,0.63],[3,7,0.14],[4,7,1.57],[5,7,84.09],[6,7,0.2],[7,7,7.73],[8,7,1.2],[9,7,2.6],[10,7,0.08],[11,7,0.05]],
      "label": {
        "show": true
      },
      "emphasis": {
        "itemStyle": {
          "shadowBlur": 10,
          "shadowColor": "rgba(0, 0, 0, 0.5)"
        }
      }
    }
  ]
}

{{< /echarts >}}
In the study, [WRF-Chem](https://www2.acom.ucar.edu/wrf-chem) model is utilized to assess contribution from different sectors to ambient PM$_{2.5}$. [PKU-Fuel](http://inventory.pku.edu.cn/) inventory is modified with [EDGAR-HTAPv3](https://edgar.jrc.ec.europa.eu/dataset_htap_v3), [GFED](https://www.globalfiredata.org/) and [PPAC](https://www.ppac.gov.in/) data to update *Biomass Burning* and *Dung Cake Burning* in India. Emissions are divided into {{< link href=Sectors.html content=12-sectors >}} (see abbreviations here) and presented by species in percentages above.

IER C-R function is used to estimate sector-specific contributions to premature mortalities for the 12 sensitivity tests. Residential sector results in 300 (95% CI, same below: 150-530) thousand deaths, while Power generation and Industry separately account for 220 (100-400) and 150 (70-260) thousand deaths. In residential sector, dung cake and straw both contribute over 100 thousand deaths. While other industry show greater impacts on urban health, brick production poses heavier burdens for rural counterpart.

{{< figure src=/images/IER-Sector-UR.jpg >}}

------

