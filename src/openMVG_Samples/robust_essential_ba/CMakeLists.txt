
ADD_DEFINITIONS(-DTHIS_SOURCE_DIR="${CMAKE_CURRENT_SOURCE_DIR}")

ADD_EXECUTABLE(openMVG_sample_robustEssential_ba robust_essential_ba.cpp)
TARGET_LINK_LIBRARIES(openMVG_sample_robustEssential_ba 
  openMVG_image
  openMVG_multiview
  openMVG_features
  vlsift
  stlplus
  ceres
  ${OPENMVG_LIBRARY_DEPENDENCIES})

SET_PROPERTY(TARGET openMVG_sample_robustEssential_ba PROPERTY FOLDER OpenMVG/Samples)
