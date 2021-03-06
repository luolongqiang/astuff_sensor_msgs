cmake_minimum_required(VERSION 2.8.3)
project(ibeo_msgs)

## Compile as C++11, supported in ROS Kinetic and newer
# add_compile_options(-std=c++11)

## Find catkin macros and libraries
find_package(catkin REQUIRED
  message_generation
  std_msgs
)

# Generate messages in the 'msg' folder
add_message_files(FILES
  CameraImage.msg
  ContourPointSigma.msg
  DeviceStatus.msg
  ErrorWarning.msg
  HostVehicleState2805.msg
  HostVehicleState2806.msg
  HostVehicleState2807.msg
  IbeoDataHeader.msg
  MountingPositionF.msg
  Object2221.msg
  Object2225.msg
  Object2270.msg
  Object2271.msg
  Object2280.msg
  ObjectData2221.msg
  ObjectData2225.msg
  ObjectData2270.msg
  ObjectData2271.msg
  ObjectData2280.msg
  Point2Df.msg
  Point2Di.msg
  Point2Dui.msg
  ResolutionInfo.msg
  ScanData2202.msg
  ScanData2204.msg
  ScanData2205.msg
  ScanData2208.msg
  ScannerInfo2204.msg
  ScannerInfo2205.msg
  ScanPoint2202.msg
  ScanPoint2204.msg
  ScanPoint2205.msg
  ScanPoint2208.msg
  Sigma2D.msg
  Size2D.msg
  TrackedProperties.msg
  UntrackedProperties.msg
  Velocity2D.msg
)

# Generate added messages and services with any dependencies listed here
generate_messages(DEPENDENCIES std_msgs)

catkin_package(CATKIN_DEPENDS
  message_runtime
  std_msgs
)
