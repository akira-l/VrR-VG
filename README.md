# VrR-VG
Visual-relevant Relationships dataset

The dataset is constructed from Visual Genome(VG). The image data need to be download from VG and we provide filtered annotations in VrR-VG. 

The given annotations are xml files and the format of xml is same to standard VG annotations. 

For image information, the xml files contains sources, size, name, etc. of images

For single instance annotations, the xml files contains classes names, ground truth bounding boxes, attributes, etc. 

For inter-instance annotations, the xml files containts relation data, subject id and object id. 

To re-implement performance of scene graph generation methods in our dataset. You need to convert the data to fit the different dataloaders in methods.

For example, in neural-motifs, you should allocate relationships to labeled classes, and change the visual_genome.py file. 
