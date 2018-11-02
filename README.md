# Calculate NDVI for large remoted sensing images by Python

Acknowlegement:
<li>   @ Script Created on May 3rd 2016</li>
<li>   @ Author: Weixing Zhang</li>
<li>   @ Purpose: Calculate NDVI for large images</li>
<li>   @ python 2.76</li>
<li>   @ Required modules: gdal, os.path, numpy, and argparse</li>


I thank Roger Veciana i Rovira for sharing his code about raster classification
Link:http://geoexamples.blogspot.com/2013/06/gdal-performance-raster-classification.html
I learned and gained a lot of help from Python community. Thank you!
I share this script mainly because back then, I could not find a easy-to-use Python script to
calculate NDVI for large RS images. I hope this script will save someone's time! 

(1) You can run it directly from the command line as such:

python NDVI.py -block 500 -redband 1 -NIRband 4 -i G:\input.tif -o G:\output.tif

(2) You can customize your own parameters and input and output directory in the script as such:
 
<li>   block_size = 500                     # Size of processing block by pixel</li>
<li>   redband_num = 1                      # Order of red band in input raster</li>
<li>   NIRband_num = 4                      # Order of NIR band in input raster</li>
<li>   inputRaster_path = r"G:\input.tif"   # Direcotry of input</li>
<li>   outputRaster_path = r"G:\output.tif" # Direcotry of output</li>
