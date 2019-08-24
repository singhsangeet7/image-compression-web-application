# image-compression-web-application
A web application to compress a image  using k means ml algorithm
File:
Python webapplication( full code) - app.py
Only python code - python_code.py
Interface image - front.png
Output & input image - output.png /input.png

Concept:
K-means clustering will group similar colors together into ‘k’ clusters (say k=16) of different colors (RGB values). Therefore, each cluster centroid is the representative of the color vector in RGB color space of its respective cluster. Now, these ‘k’ cluster centroids will replace all the color vectors in their respective clusters. Thus, we need to only store the label for each pixel which tells the cluster to which this pixel belongs. Additionally, we keep the record of color vectors of each cluster center.

Code Algo:

1)First initialise the points and mean, Points will store all the image points into 3 columns of RGB. Means is initialised to zeros initially and now any random values of rows are kept in means.
2)Then comes the kmeans where the value of means is clustered, using distance function which calcuate eucladian distances.
3)another array called index keep tarck of the min distace cluster from that particular point.
4)Now all the mean values are transferred to cluster array which remodifies the image based on the new points.
5)The image is displayed on the screen which can be further downloaded.
