## view-adaptive-image-generation

  Need to dowload the NTU-RGB+D skeleton dataset

  Extract the dataset to ./data/ntu/nturgb+d_skeletons/
  
  
### Process the data
 cd ./data/ntu
 
 Get skeleton of each performer
 
    python get_raw_skes_data.py
 
 
  Remove the bad skeleton
  
    python get_raw_denoised_data.py

  Transform the skeleton to the center of the first frame
  
    python seq_transformation.py
 
 
 ## To generate the mapping images:
 
 run the script, "generate_skeleton_map_images.ipynb"; in the script just change the directory path
