## Set up your Assignment

1.  Set up your Assignment 07 using the instructions from [Assignment 00](https://github.com/SAIC-ARTTECH-3039-5039/Assignment_00/blob/master/README.md).

## Do the Assignment

0.  This is a continuation of our in-class assignment with a few additions.

1.  Train the `Session_07/00_EigenFaces` example with 1000 faces. The data is [here](https://www.dropbox.com/s/itg288ry7detdsn/1000.zip?dl=0). We trained it with just a few hundred in class.

2.  Building from `Session_07/01_EigenFacesReconstruction`, encode an image that the PCA model has not seen (i.e. it wasn't in your 1000 faces in the step above).

3.  Save the weights to disk in a JSON file.

4.  Create an application that can read the weights from the JSON file + your `pca.data` model and recreate the image.

5.  Create one of the following applications:

    -   Create an application that represents a live camera image `ofVideoGrabber` stream using only the top 200 or less PCA weights.  The number 200 should be adjustable with a keyboard or mouse input.

    -   Using the 1000 face database, encode each image in the database as a 50-200 (or more or less?) dimensional vector of weights in a spatial hash.  Use the live camera feed (`ofVideoGrabber`) in combination with `ofxSpatialHash` to search for the 5 closest image matches to the live image input. See [this example](https://github.com/bakercp/ofxSpatialHash/blob/master/example_kdtree_nd/src/ofApp.h) for help.

## To submit an Assignment

1.  Follow the instructions from [Assignment 00](https://github.com/SAIC-ARTTECH-3039-5039/Assignment_00/blob/master/README.md).

2.  Create a directory in this repo with your project code including the annotated training data, the trained network, and some screenshots of the results.  Commit that directory!  Basically, I want anything needed to re-create your results.
