set(MGHIO_SRC
itkMGHImageIOFactory.cxx
itkMGHImageIO.cxx
)

add_library(MGHIO ${ITK_LIBRARY_BUILD_TYPE} ${MGHIO_SRC})
target_link_libraries(MGHIO ${ITKIOImageBase_LIBRARIES} ${ITKZLIB_LIBRARIES})
itk_module_target(MGHIO)
