# Concrete Heat: Contributions of Urban Land Use to Heatwave Intensity in Shanghai, China

## Contributors
**Ajadi Sodiq Abayomi**, **Helyne Adamson**, **Thomas Rakiswende Bere**, **Sharon Christa**, **Elisabeth Lindner**, **Xiaoxiao Zhao**

## Presentations
- [Project Presentation (PDF)](presentations/eight-minute-presentation.pdf)

# Research question/objective

In this research study, we investigate the relationship between land use and land cover and heatwave intensity in Shanghai, China. Specifically, we will investigate the link between impervious surface and heatwave intensity for the years 1991-2024.

# Background/Motivation

Heatwaves have become a climate-related hazard that is happening globally. It causes a significant impact on human health, energy consumption, and infrastructure ([Luck & Wu, 2002](https://www.sciencedirect.com/science/article/pii/S0034425711002525#bb0180)). Urban areas have more concrete buildings and rooftops that absorb more heat when compared to natural landscapes. This results in elevated temperatures compared to surrounding areas. High population densities exacerbate heat stress (Reid et al., 2000).

Existing research has established that land cover and land use patterns influence local microclimates (Carlson & Arthur, 2000). Numerous studies have already been conducted that establish the relationship between land cover types and local microclimates (Crum & Jenerette, 2017). 

Shanghai is one of the largest and most rapidly urbanizing cities in China  ([China Statistics Press, 2020](https://www.sciencedirect.com/science/article/pii/S0048969722013560#bb0020)). Its expansion is not just horizontally, but also vertical. Due to this constant change and complex development pattern, Shanghai is a classic example that can help illustrate the relationship between impervious surfaces and elevated temperatures. Even though the link between land cover and heat island effect is established and well documented (Wang et al., 2017; Yang et al., 2022), very few studies are conducted that focuses on how impervious surfaces, land use and land cover are correlated with heat wave intensity (Shi et al., 2023). This can be critical to urban climate resilience planning. Few studies have integrated land use data with heatwave metrics to identify this relationship, especially in rapidly urbanizing megacities like Shanghai. 

This study addresses this gap by analyzing the correlation between impervious surface coverage and heatwave intensity in Shanghai by linking land use characteristics with spatial and temporal variation with the heatwave severity.

The study is modeled after and builds upon the work by Wang et al. (2017).

Wang, H., Zhang, Y., Tsou, J. Y., & Li, Y. (2017). Surface Urban Heat Island Analysis of Shanghai (China) Based on the Change of Land Use and Land Cover. Sustainability, 9(9), 1538. [https://doi.org/10.3390/su9091538](https://doi.org/10.3390/su9091538)

# Hypothesis

We expect to find a positive correlation between impervious surface and heatwave intensity.

# Data

| Datasets | Source | Why useful (Purpose) |
| :---- | :---- | :---- |
| ERA5 Land | [https://cds.climate.copernicus.eu/datasets/derived-era5-land-daily-statistics?tab=download](https://cds.climate.copernicus.eu/datasets/derived-era5-land-daily-statistics?tab=download) | Heatwaves detection and characteristics study |
| Land use land cover (LULC) | [https://livingatlas.arcgis.com/en/home/](https://livingatlas.arcgis.com/en/home/)  | Urban heat island detection |
| LANDSAT (5-8) | Google Earth Engine | Measures of impervious surfaces |
| Nighttime Lights  | Google Earth Engine | To determine urban sprawl (i.e., movement of people from rural areas to urban centers) and socioeconomic activities over the study period.  |

# Methods/Approach

To determine the relationship between urban land features and heatwave intensity, a multi-step spatiotemporal analysis will be conducted, combining remote sensing data with climate reanalysis data:

1. ### Heat wave detection & characterisation

   * Calculate normals (ERA-5 Land data and LST data)  
   * Calculate 90th percentile for heatwave detection  
   * Study heatwave characteristics (intensity, frequency, duration)

2. ### Land use identification & classification

   * Extract relevant satellite indices (e.g NDVI and MNDWI) to compute impervious surfaces  
   * Categorise key land use & cover types (impervious surfaces, green spaces, water bodies, other land/soil) using a Maximum Likelihood approach(?) (or a decision tree classifier)

3. ### Land use-temperature correlation analysis

   * Calculate correlation between land surfaces and heatwaves characteristics (both linear fitting and quadratic fitting?)

# Expected outcomes

This study is expected to produce a comprehensive understanding of the relationship between urban land use, specifically impervious surface expansion, and the intensity, frequency, and duration of heatwaves in Shanghai from 1991 to 2024\. By integrating satellite remote sensing, reanalysis climate data, the research will generate multi-dimensional insights into the urban heatwave phenomenon. Our research outcome include:

1. Quantification of heatwave trends and urban growth, provide implications for the city government considering urban expansion.  
2. Assess the potential causal impacts of urban structure and land use allocation on the local climate conditions, and provide recommendations for urban developers and policy makers.

# Literature 

Carlson, Toby N., and S. Traci Arthur. "The impact of land use—land cover changes due to urbanization on surface microclimate and hydrology: a satellite perspective." Global and planetary change 25, no. 1-2 (2000): 49-65. [https://doi.org/10.1016/S0921-8181(00)00021-7](https://doi.org/10.1016/S0921-8181\(00\)00021-7) 

China Statistics Press, 2020\. China City Statistical Yearbook-2020. China Stat. Press.

Crum, Steven M., and G. Darrel Jenerette. "Microclimate variation among urban land covers: The importance of vertical and horizontal structure in air and land surface temperature relationships." Journal of Applied Meteorology and Climatology 56, no. 9 (2017): 2531-2543.

Luck, M., Wu, J. A gradient analysis of urban landscape pattern: a case study from the Phoenix metropolitan region, Arizona, USA. Landscape Ecology 17, 327–339 (2002). [https://doi.org/10.1023/A:1020512723753](https://doi.org/10.1023/A:1020512723753)

Reid, R.S.; Kruska, R.L.; Muthui, N.; Taye, A.; Wotton, S.; Wilson, C.J.; Mulatu, W. Land-use and land-cover dynamics in response to changes in climatic, biological and socio-political forces: The case of southwestern Ethiopia. Landsc. Ecol. 2000, 15, 339–355. \[[Google Scholar](http://scholar.google.com/scholar_lookup?title=Land-use+and+land-cover+dynamics+in+response+to+changes+in+climatic,+biological+and+socio-political+forces:+The+case+of+southwestern+Ethiopia&author=Reid,+R.S.&author=Kruska,+R.L.&author=Muthui,+N.&author=Taye,+A.&author=Wotton,+S.&author=Wilson,+C.J.&author=Mulatu,+W.&publication_year=2000&journal=Landsc.+Ecol.&volume=15&pages=339%E2%80%93355&doi=10.1023/A:1008177712995)\] \[[CrossRef](http://dx.doi.org/10.1023/A:1008177712995)\]

Shi, Zitong, Xuecao Li, Tengyun Hu, Bo Yuan, Peiyi Yin, and Dabang Jiang. "Modeling the intensity of surface urban heat island based on the impervious surface area." Urban Climate 49 (2023): 101529\.

Yang, Y., Shen, G. R., Zhang, C., Hao, S., Zhang, Z. Y. L., & Yin, S. (2022). Quantitative analysis and prediction of urban heat island intensity on urban-rural gradient: A case study of Shanghai. Science of The Total Environment, 829, Article 154264\. [https://doi.org/10.1016/j.scitotenv.2022.154264](https://doi.org/10.1016/j.scitotenv.2022.154264)

Yang, X., L. Ruby Leung, N. Zhao, C. Zhao, Y. Qian, K. Hu, X. Liu, and B. Chen (2017), Contribution of urbanization to the increase of extreme heat events in an urban agglomeration in east China, *Geophys. Res. Lett.*, 44, 6940–6950, doi:[10.1002/2017GL074084](https://doi.org/10.1002/2017GL074084).

* Useful for urbanisation data source/methods? They have a novel way of aligning/calibrating NightTimeLight (NTL) images to quantify urban development and study urban expansion

