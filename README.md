# LBP_edge_detection_for_depth_Image
In this project, I implement an approach to detect edge. This approach focus on low resolution depth image. 
This work implemented from paper “ LBP Based_Edge_Detection_Method_for_Depth_Images_With_Low_Resolutions” Link : https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8556465



![image](https://github.com/sonnk1108/LBP_edge_detection_for_depth_Image/assets/64638305/fbeec931-3f86-4291-bea2-b6b33b4d5ac1)

The proposed edge detection method involves three main steps:

Step 1:  Adjust the contrast of the depth image using a simple linear contrast stretching technique. This enhances the visibility of edges for later processing.

Step 2: Applying a modified Local Binary Pattern (LBP) operator to generate a rough edge map. The standard LBP is adapted to make it more sensitive to depth discontinuities. An adaptive thresholding approach compares each pixel to local maximum and average values.

Step 3: Removing isolated small edges using a 5x5 pixel filtering mask slid across the image. This eliminates artifacts while retaining major edges. The key ideas are modifying the LBP operator to work better on depth images rather than textures, and using an adaptive threshold rather than a global one. This allows the LBP to detect and highlight depth discontinuities.

For details explanation, Please read my medium blog here : https://medium.com/@khanhson0811/boost-your-depth-image-edge-detection-with-this-modified-lbp-method-018cc59b9b35
