add_executable(armarker2pose.exe  armarker2pose.cpp)
target_link_libraries(armarker2pose.exe ${catkin_LIBRARIES})
add_dependencies(armarker2pose.exe  ar_pose_generate_messages_cpp)
