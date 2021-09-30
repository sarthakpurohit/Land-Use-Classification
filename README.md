# Land-Use-Classification
Classifying the land use of a given satellite image
# PROBLEM STATEMENT
   Satellite imagery can help us find solutions to the growing number of environmental problems that we face today. It allows us to not only get a bird’s eye view of what’s around us, but also uncovers parts of the world that are rarely seen. Tapping into the potential of categorizing land cover and land use around the world means that humans can more efficiently make use of natural resources, hopefully lowering cases of waste and deprivation. But despite its potential to be incredibly useful, satellite data is massive and confusing, and making sense of it requires complex analysis.
   
   
# OBJECTIVE
  This project could help a variety of stakeholders, including conservationists, urban planners, and environmental scientists, survey and identify patterns in land use to see which natural areas are under threat or which areas are best for urban development. But in this case, I will tailor this project to a client that is similar to the agriculture imagery company that I currently work for. Imagery companies can use land use classification models to categorize what’s in each image and optimize their efforts towards the parts of land that are important to them. For example, an agriculture company will only want to be concerned with land that’s labelled as pasture, annual crop, or permanent crop. If a satellite is constantly taking images, this project would help save hours of time manually sorting through imagery.
  
  Land use classification is important for identifying the parts of an image to which certain analyses are applied. For example, if the company has different crop stress algorithms for fields that are next to urban areas versus fields that are next to rivers, this project would help them to automate the process of applying these specialized algorithms and more effectively solve environmental problems.
  
  
  # DATASET USED
 For this project, I used open source EuroSAT Sentinel-2 satellite images from the German Research Center for Artificial Intelligence, which can be downloaded locally link. The dataset consists of 27,000 labeled images of 10 different land use classes:

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

Each multispectral image consists of 13 different color bands that represent different wavelengths of light/color and different resolutions. These different light bands help distinguish parts of the landscape that reflect certain types of light in particular ways. Since most images don’t include special bands like Vegetation Red Edge, Coastal aerosol, or SWIR, for this project I chose to only use the red, green, and blue bands in an effort to make my model generalizable to most images.

# Pipeline of the Project 
# Architechture 
# Predicted Output
# Reference 

