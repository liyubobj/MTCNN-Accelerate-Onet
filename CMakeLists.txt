cmake_minimum_required(VERSION 2.6)
project(MTCNN_Accelerate-Onet)

SET(CMAKE_C_COMPILER g++)
SET(CMAK_CXX_COMPILER g++)
add_compile_options(-std=c++11)
add_compile_options(-m64)

include_directories(
    /usr/local/cuda/include
    /opt/py-faster-rcnn/caffe-fast-rcnn/build/src/
    /opt/py-faster-rcnn/caffe-fast-rcnn/include)
link_directories(
    /usr/local/cuda/lib64
    /opt//py-faster-rcnn/caffe-fast-rcnn/build/lib)

set(SOURCE_FILES main.cpp mtcnn.cpp mtcnn.h)
add_executable(MTCNN_Accelerate-Onet ${SOURCE_FILES})

target_link_libraries(MTCNN_Accelerate-Onet
    -lcaffe 
    -lboost_system 
    -lboost_filesystem
    -lopencv_core 
    -lopencv_highgui 
    -lopencv_imgproc
    -lglog
    -lgflags
    -lprotobuf
    -lm
)
