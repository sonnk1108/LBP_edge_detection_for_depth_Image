# LBP_edge_detection_for_depth_Image
In this project, I implement an approach to detect edge. This approach focus on low resolution depth image. 
This work implemented from paper “ LBP Based_Edge_Detection_Method_for_Depth_Images_With_Low_Resolutions” Link : https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8556465
Method

The proposed edge detection method involves three main steps:

Adjusting the contrast of the depth image using a simple linear contrast stretching technique. This enhances the visibility of edges for later processing.
Applying a modified Local Binary Pattern (LBP) operator to generate a rough edge map. The standard LBP is adapted to make it more sensitive to depth discontinuities. An adaptive thresholding approach compares each pixel to local maximum and average values.
Removing isolated small edges using a 5x5 pixel filtering mask slid across the image. This eliminates artifacts while retaining major edges.
The key ideas are modifying the LBP operator to work better on depth images rather than textures, and using an adaptive threshold rather than a global one. This allows the LBP to detect and highlight depth discontinuities.

The contrast enhancement as a preprocessing step improves the results. The post-processing filtering helps refine the edge map.

Overall, adapting LBP for depth images and an adaptive threshold are presented as the main novel components for effectively detecting edges in low resolution depth maps where other standard methods fail. The simple linear processing makes the method fast and suitable for real-time applications.
