
# This file was gererated by the build system used internally in the Yandex monorepo.
# Only simple modifications are allowed (adding source-files to targets, adding simple properties
# like target_include_directories). These modifications will be ported to original
# ya.make files by maintainers. Any complex modifications which can't be ported back to the
# original buildsystem will not be accepted.



add_library(catboost-libs-calc_metrics)
target_link_libraries(catboost-libs-calc_metrics PUBLIC
  contrib-libs-cxxsupp
  yutil
  cpp-threading-local_executor
  catboost-libs-data
  catboost-libs-metrics
  private-libs-target
  private-libs-options
)
target_sources(catboost-libs-calc_metrics PRIVATE
  ${CMAKE_SOURCE_DIR}/catboost/libs/calc_metrics/calc_metrics.cpp
)
