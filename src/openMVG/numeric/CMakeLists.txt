ADD_LIBRARY(openMVG_numeric
  numeric.cpp
  numeric.h)
SET_PROPERTY(TARGET openMVG_numeric PROPERTY FOLDER OpenMVG/OpenMVG)
INSTALL(TARGETS openMVG_numeric DESTINATION lib/)

UNIT_TEST(openMVG numeric openMVG_numeric)
UNIT_TEST(openMVG poly openMVG_numeric)
UNIT_TEST(openMVG lm openMVG_numeric)
