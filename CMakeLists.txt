cmake_minimum_required(VERSION 2.8)
project( DisplayImage )
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable( DisplayImage DisplayImage.cpp )
target_link_libraries( DisplayImage ${OpenCV_LIBS} )


add_executable( image image.cpp )
target_link_libraries( image ${OpenCV_LIBS} )

add_executable( Grayimage Grayimage.cpp )
target_link_libraries( Grayimage ${OpenCV_LIBS} )

add_executable( ErodingandDilating ErodingandDilating.cpp )
target_link_libraries( ErodingandDilating ${OpenCV_LIBS} )


add_executable( Morphology_tf Morphology_tf.cpp )
target_link_libraries( Morphology_tf ${OpenCV_LIBS} )

add_executable( Image-Pyramids Image-Pyramids.cpp )
target_link_libraries( Image-Pyramids ${OpenCV_LIBS} )

add_executable( Basic_thresholding_op Basic_thresholding_op.cpp )
target_link_libraries( Basic_thresholding_op ${OpenCV_LIBS} )
