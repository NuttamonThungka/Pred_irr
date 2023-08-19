- **SolarCalculator** is the folder that contain the function to calculate the importance variable using in clearsky model that compute the clear-sky irraduance
-   - ```cal_zna``` is the function to calculate zeith angle
    - ```cal_airmass``` is the function to calculate air mass
    - ```cal_clearsky``` is the function to calculate clear-sky irradiance
 
  - ```cloudindex_file_creation.ipynb``` is the file that generate the cloud index at the interested site. For the location of Synergy is (lat, long) : (14.00294247371573, 100.6267303787081)
    ```generate_data.ipynb``` is the file that generate the data for train the model.
      - the output of this file are ```Image_train.cav``` and ```Attribute_train.csv```
