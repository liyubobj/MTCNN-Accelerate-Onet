# MTCNN-caffe
MTCNN Face Detection &amp; Alignment
This is a C++ version used Caffe
## 
half model shrink the orignal onet by half quantities of parameters with faster forward computing and similar results on fddb
you can try different thresholds and minsize value to  perform best on your own datasets

# Useage
- [caffe](https://github.com/BVLC/caffe)
	cmake ..
	make -j8
    method : mtcnn 0 (camera) ,1 (video) ,2 imageList ,3 image, 4 landmarkPts	
camera:	./MTCNN-Accelerate-Onet 0 
video:	./MTCNN-Accelerate-Onet 1 video_path
imageList: ./MTCNN-Accelerate-Onet 2 imagelist_path
image:     ./MTCNN-Accelerate-Onet 3 image_path
landmarkPts ./MTCNN-Accelerate-Onet 4 imagelist ptslist

# Results
![image](https://github.com/blankWorld/MTCNN-caffe/raw/master/img/mtcnn-fddb.jpg)
![image](https://github.com/blankWorld/MTCNN-caffe/raw/master/img/_res_0_Parade_marchingband_1_364.jpg)
![image](https://github.com/blankWorld/MTCNN-caffe/raw/master/img/_res_0_Parade_marchingband_1_408.jpg)
![image](https://github.com/blankWorld/MTCNN-caffe/raw/master/img/_res_img_78.jpg)
![image](https://github.com/blankWorld/MTCNN-caffe/raw/master/img/_res_img_534.jpg)
![image](https://github.com/blankWorld/MTCNN-caffe/raw/master/img/_res_img_561.jpg)
![image](https://github.com/blankWorld/MTCNN-caffe/raw/master/img/_res_img_591.jpg)
![image](https://github.com/blankWorld/MTCNN-caffe/raw/master/img/_res_img_769.jpg)


