# Face Recognition System

Use of LBPH algorithm has been made to develop and design a face detection and recognitation system on python using numpy.

# What is LBPH ?

In LBPH algorithm for face recognition these four steps are carried out step by step:The face is detected using video capture using 3x3 pixel matrix. The captured images follow the four parameters like Radius ,Neighbors,Grid X ,Grid Y . Radius is used to build the circular local binary pattern and represents the radius around the central pixel(set to 1). Neighbor parameter is the number of sample points to build the circular local binary pattern(set to 8 usually). Grid X gives the number of cells in the horizontal direction as the number of cells increases accuracy of grid is increased.Grid Y gives the number of cells in the vertical direction as the number of cells increases accuracy of grid is increased. The algorithm uses a concept of a sliding window, Sliding window refers to an imaginary boxes that hold the frames on both sender and receiver side, based on the parameters radius and neighbors.Using Grid X and Grid Y parameter images are divided into multiple grid and the histogram is generated of each region of gray scale image. The Histogram is then used for detecting the face from training dataset.

# Technologies used:

1. Python.
2. Numpy.
3. SQL.
4. Ruby.

# Usage

DataSetGenerator.py is responsible to capture images of a user after the name of the user is saved to database.

```
Run dataSetGenerator.py
```

trainer.py processes all the data that is stored in the database and converts them to histograms.

```
Run trainer.py
```

detector.py Capture images and compares them with stored images top check if person is known or not

```
Run detector.py
```

# File Structure

After images are captured they are stored in the dataset folder and if after detector is running and person is unknown then images are transferred into unknown folder

```
|__dataSet
|__Unknown
```

All this can be stored as evidence and reports.

![Alt Detector](https://github.com/RohanShah27/Face-Recognition-System/blob/master/screenshot/detector.png?raw=true "Title")

# Publications

1. Research Paper published on IJSRD journal 2019
   http://ijsrd.com/Article.php?manuscript=IJSRDV7I20500
2. Implementation paper published on ICaste2019-2020
