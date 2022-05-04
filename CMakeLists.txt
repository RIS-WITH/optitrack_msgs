cmake_minimum_required(VERSION 2.8.3)
project(optitrack_msgs)

find_package(catkin REQUIRED COMPONENTS
  message_generation
  std_msgs
)

 add_message_files(
   FILES
   or_pose_estimator_state.msg
   or_t3d_aacc_cov.msg
   or_t3d_aacc.msg
   or_t3d_acc_cov.msg
   or_t3d_acc.msg
   or_t3d_att_cov.msg
   or_t3d_att_pos_cov.msg
   or_t3d_att.msg
   or_t3d_avel_cov.msg
   or_t3d_avel.msg
   or_t3d_pos_cov.msg
   or_t3d_pos.msg
   or_t3d_vel_cov.msg
   or_t3d_vel.msg
   or_time_ts.msg
)

generate_messages(
   DEPENDENCIES
   std_msgs
)

catkin_package(
  CATKIN_DEPENDS message_runtime std_msgs
)