# Create Rich Dataset of Drone Images with 3D models, DSM, DTM, Ortho Images produced Using Photogrammetry Pipeline and Visualize Extracted Features from the 2D and 3D Drone Data.

**Objectives :** 

- Make a rich dataset of and from images captured by a drone
- Collect overlapped aerial images using DJI Mavic 2 pro
- Compare photogrammetry pipelines to find a suitable fit to produce DSM,DTM,Ortho Image and 3D Mesh or Point Cloud Data
- Setup a browser application to view processed Mesh Object data, Ortho Image, Simplified Buildings in a map like environment
- Setup Automatic Feature Extraction Algorithms for 2D and 3D data to be viewed in the browser application 
- Use the rich drone dataset for Deep Learning Research

**Methods :**

- For data collection, flying a 3D grid mission on Pix4D Capture with 75 degree camera angle and 80% front and side overlap gave the optimum 3d .obj models for future use.

- Exploration of photogrammetry pipelines like DroneDeploy, Pix4D Mapper, OpenDroneMap and Meshroom led to select DroneDeploy as the best online short term solution while Meshroom with Open Drone Map provided the best open source,offline,local pipeline to use for our specific use case.

- For setting up a browser application CesiumJS is showing promis and is being looked into at the moment.

- Automatic building height extraction is being worked on at the moment. The most promising pipeline is using a neural network to extract building footprints, from Ortho Images (which we get as output from OpenDroneMap), as coordinate polygons. Use the polygons to extract Elevation Data from Digital Surface Models (produced by OpenDroneMap).

- Further use of Mesh data for calculating optimum area for solar panels in any given region, Flood Delineation using DSM and Feature Extraction from 3D models are being looked into at the moment.


**Video of Output from Photogrammetry Pipeline :**

[![IMAGE ALT TEXT HERE](https://github.com/antorhasan/drone_prj/blob/master/new.png)](https://www.youtube.com/watch?v=odiGVLqg5V8&feature=youtu.be)
