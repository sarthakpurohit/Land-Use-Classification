# Land-Use-Classification ​🌏​🗺​

Classifying the land use of a given satellite image.

Land-use classification schemes typically address both land use and land cover. A major land-use classification system developed by the United States Geological Survey (USGS) has multiple levels of classification. The categories within these levels are arranged in a nested hierarchy. The most general or aggregated classification (level I) includes broad land-use categories, such as ‘agriculture’ or ‘urban and built-up’ land . This level of classification is commonly used for regional and other large-scale applications. Within each level I class are a number of more detailed (level II) land-use and land-cover classes.


# 📍 Problem Statement
   Satellite imagery can help us find solutions to the growing number of environmental problems that we face today. It allows us to not only get a bird’s eye view of what’s around us, but also uncovers parts of the world that are rarely seen. Tapping into the potential of categorizing land cover and land use around the world means that humans can more efficiently make use of natural resources, hopefully lowering cases of waste and deprivation. But despite its potential to be incredibly useful, satellite data is massive and confusing, and making sense of it requires complex analysis.
  
  ![ds p](https://user-images.githubusercontent.com/78519911/135376980-b77d540c-1f63-40ac-b746-13ff91d02b2c.gif)

   
# 📋 Objective 
  This project could help a variety of stakeholders, including conservationists, urban planners, and environmental scientists, survey and identify patterns in land use to see which natural areas are under threat or which areas are best for urban development. But in this case, I will tailor this project to a client that is similar to the agriculture imagery company that I currently work for. Imagery companies can use land use classification models to categorize what’s in each image and optimize their efforts towards the parts of land that are important to them. For example, an agriculture company will only want to be concerned with land that’s labelled as pasture, annual crop, or permanent crop. If a satellite is constantly taking images, this project would help save hours of time manually sorting through imagery.
  
  Land use classification is important for identifying the parts of an image to which certain analyses are applied. For example, if the company has different crop stress algorithms for fields that are next to urban areas versus fields that are next to rivers, this project would help them to automate the process of applying these specialized algorithms and more effectively solve environmental problems.
  
  # Installation 💻
   
   ```
   git clone https://github.com/sarthakpurohit/Land-Use-Classification
   cd Land-Use-Classification
   ```
   
   For Anaconda users:
   
   Create virtual environment named `landuse`
   ```
   conda create -n landuse
   ```
   
   Activate landuse environment
   ```
   conda activate landuse
   ```
   
   Install pytorch
   ```
   conda install pytorch torchvision torchaudio cpuonly -c pytorch
   ```
   
   Install matplotlib
   ```
   conda install matplotlib
   ```
   
   Install jupyter notebook
   ```
   conda install -c conda-forge jupyterlab
   ```
   
   Install streamlit
   ```
   conda install -c conda-forge streamlit
   ```
  
  To run WebApp
  ```
  streamlit run datascienceUI.py
  ```
  
  # Dataset Used 📊📁
 For this project, I used open source EuroSAT Sentinel-2 satellite images from the German Research Center for Artificial Intelligence, which can be downloaded locally [link](http://madm.dfki.de/downloads). The dataset consists of 27,000 labeled images of 10 different land use classes:

- Annual Crop
- Forest
- Herbaceous Vegetation
- Highway
- Industrial
- Pasture
- Permanent Crop
- Residential
- River
- Sea / Lake


![image](https://user-images.githubusercontent.com/78519911/138552682-df140d3e-438c-49cc-9246-e82f17500278.png)





![image](https://user-images.githubusercontent.com/78519911/138552697-c15b4548-806d-44fa-9e75-8a00a3ad0b5a.png)


Each multispectral image consists of 13 different color bands that represent different wavelengths of light/color and different resolutions. These different light bands help distinguish parts of the landscape that reflect certain types of light in particular ways. Since most images don’t include special bands like Vegetation Red Edge, Coastal aerosol, or SWIR, for this project I chose to only use the red, green, and blue bands in an effort to make my model generalizable to most images.

![Sentinel-2Poster](https://user-images.githubusercontent.com/78519911/135378729-2eec9673-714d-4584-be69-eb3f789fa13f.jpg)



![image](https://user-images.githubusercontent.com/78519911/138552671-567e570e-ed4e-4490-b18d-db7c7c17999f.png)




# Pipeline of the Project 

 ✔️ Data preparation
 
 ✔️ Exploratory data analysis
 
 ✔️ Convolutional neural network model
 
 ✔️ CNN with model tuning

# Architecture 👨‍💻

![41598_2020_74215_Fig1_HTML](https://user-images.githubusercontent.com/78519911/135385106-8290f9c2-c058-4957-bc29-79146a0b3ccb.jpg)


# Predicted Output.
![FireShot Capture 001 - datascienceUI · Streamlit - localhost](https://user-images.githubusercontent.com/78519911/142714328-f9e19187-5f4d-4e26-8458-d6943854568b.png)


# Reference 
Dataset - http://madm.dfki.de/downloads
