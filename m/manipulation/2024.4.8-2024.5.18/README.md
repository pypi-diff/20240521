# Comparing `tmp/manipulation-2024.4.8.tar.gz` & `tmp/manipulation-2024.5.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manipulation-2024.4.8.tar", max compression
+gzip compressed data, was "manipulation-2024.5.18.tar", max compression
```

## Comparing `manipulation-2024.4.8.tar` & `manipulation-2024.5.18.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0     1561 2024-02-22 14:57:44.046800 manipulation-2024.4.8/LICENSE.TXT
--rw-r--r--   0        0        0      464 2024-02-22 14:57:44.046800 manipulation-2024.4.8/README.md
--rw-r--r--   0        0        0      167 2024-02-22 14:57:44.110801 manipulation-2024.4.8/manipulation/__init__.py
--rw-r--r--   0        0        0      846 2024-02-22 14:57:44.110801 manipulation-2024.4.8/manipulation/_static/custom.css
--rw-r--r--   0        0        0     6481 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/clutter.py
--rw-r--r--   0        0        0      891 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/conf.py
--rw-r--r--   0        0        0    16339 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/create_sdf_from_mesh.py
--rw-r--r--   0        0        0      211 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/drake_gym.py
--rw-r--r--   0        0        0     9221 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/envs/box_flipup.py
--rw-r--r--   0        0        0     8482 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/envs/planar_gripper_pushing_a_box.py
--rw-r--r--   0        0        0    32464 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/clutter/normal_solution.npy
--rw-r--r--   0        0        0     1724 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/clutter/test_analytic_grasp.py
--rw-r--r--   0        0        0     6751 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/clutter/test_grasp_candidate.py
--rw-r--r--   0        0        0     1768 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/clutter/test_normal.py
--rw-r--r--   0        0        0     3978 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/clutter/test_simulation_tuning.py
--rw-r--r--   0        0        0     3598 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/deep_perception/test_contrastive.py
--rw-r--r--   0        0        0     1563 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/force/test_hybrid.py
--rw-r--r--   0        0        0     4758 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/grader.py
--rw-r--r--   0        0        0     3934 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/mobile/test_mobile_base_ik.py
--rw-r--r--   0        0        0     1188 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pick/plot_planar_manipulator.py
--rw-r--r--   0        0        0    26806 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pick/test_differential_ik.py
--rw-r--r--   0        0        0     3585 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pick/test_planar_manipulator.py
--rw-r--r--   0        0        0     2874 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pick/test_rigid_transforms.py
--rw-r--r--   0        0        0     1881 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pick/test_robot_painter.py
--rw-r--r--   0        0        0     1139 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pick/test_simple_qp.py
--rw-r--r--   0        0        0     3642 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pose/test_icp.py
--rw-r--r--   0        0        0     1445 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pose/test_pose_estimation.py
--rw-r--r--   0        0        0     3240 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pose/test_ransac.py
--rw-r--r--   0        0        0     3380 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/rl/test_stochastic_optimization.py
--rw-r--r--   0        0        0     2825 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/rl/test_vpg.py
--rw-r--r--   0        0        0      870 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/robot/test_direct_joint_control.py
--rw-r--r--   0        0        0     1184 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/robot/test_hardware_station_io.py
--rw-r--r--   0        0        0     2261 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/robot/test_reflected_inertia.py
--rw-r--r--   0        0        0      672 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/robot/test_survey.py
--rw-r--r--   0        0        0     1372 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/segmentation/test_mask.py
--rw-r--r--   0        0        0     2271 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/segmentation/test_segmentation_and_grasp.py
--rw-r--r--   0        0        0        0 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/__init__.py
--rw-r--r--   0        0        0    23490 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/geometry.py
--rw-r--r--   0        0        0     3711 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py
--rw-r--r--   0        0        0     6529 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/robot.py
--rw-r--r--   0        0        0    14614 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py
--rw-r--r--   0        0        0     1464 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/test_door_opening.py
--rw-r--r--   0        0        0     2391 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/test_rrt_planning.py
--rw-r--r--   0        0        0     5489 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/test_taskspace_iris.py
--rw-r--r--   0        0        0     3764 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/icp.py
--rw-r--r--   0        0        0      243 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/index.md
--rw-r--r--   0        0        0      256 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/meshcat_cpp_utils.py
--rw-r--r--   0        0        0      102 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/meshcat_utils.md
--rw-r--r--   0        0        0    17872 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/meshcat_utils.py
--rw-r--r--   0        0        0     5938 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf
--rw-r--r--   0        0        0     1656 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/models/book.sdf
--rw-r--r--   0        0        0     1280 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/models/bunny/README
--rw-r--r--   0        0        0   658744 2024-02-22 14:57:44.122801 manipulation-2024.4.8/manipulation/models/bunny/bun_zipper_res2.ply
--rw-r--r--   0        0        0   196232 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/bunny/bunny.npy
--rw-r--r--   0        0        0     1496 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/camera_box.sdf
--rw-r--r--   0        0        0      155 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/clutter.dmd.yaml
--rw-r--r--   0        0        0     1544 2024-04-08 12:21:31.612057 manipulation-2024.4.8/manipulation/models/clutter.scenarios.yaml
--rw-r--r--   0        0        0      367 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/clutter_mustard.dmd.yaml
--rw-r--r--   0        0        0      183 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/clutter_planning.dmd.yaml
--rw-r--r--   0        0        0      165 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/clutter_w_cameras.dmd.yaml
--rw-r--r--   0        0        0     2000 2024-04-08 12:21:31.612057 manipulation-2024.4.8/manipulation/models/cupboard.scenario.yaml
--rw-r--r--   0        0        0     2485 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/double_pendulum.urdf
--rw-r--r--   0        0        0      215 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/floating_joint.urdf
--rw-r--r--   0        0        0     1407 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/floor.sdf
--rw-r--r--   0        0        0     1471 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/003_cracker_box.sdf
--rw-r--r--   0        0        0     1469 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/004_sugar_box.sdf
--rw-r--r--   0        0        0     1630 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/005_tomato_soup_can.sdf
--rw-r--r--   0        0        0     4990 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/006_mustard_bottle.sdf
--rw-r--r--   0        0        0     1479 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/009_gelatin_box.sdf
--rw-r--r--   0        0        0     1475 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/010_potted_meat_can.sdf
--rw-r--r--   0        0        0     1104 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/061_foam_brick.sdf
--rw-r--r--   0        0        0      246 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/README.md
--rw-r--r--   0        0        0     4709 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/bin.sdf
--rw-r--r--   0        0        0     9110 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/cupboard.sdf
--rw-r--r--   0        0        0     6069 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/extra_heavy_duty_table_surface_only_collision.sdf
--rw-r--r--   0        0        0     5708 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/schunk_wsg_50_with_tip.sdf
--rw-r--r--   0        0        0    21069 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_000.obj
--rw-r--r--   0        0        0    21659 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_001.obj
--rw-r--r--   0        0        0    23842 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_002.obj
--rw-r--r--   0        0        0    24252 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_003.obj
--rw-r--r--   0        0        0    26183 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_004.obj
--rw-r--r--   0        0        0    15215 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_005.obj
--rw-r--r--   0        0        0    18773 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_006.obj
--rw-r--r--   0        0        0    23818 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_007.obj
--rw-r--r--   0        0        0    24964 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_008.obj
--rw-r--r--   0        0        0      658 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/iiwa_and_wsg.dmd.yaml
--rw-r--r--   0        0        0      943 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mecanum/README.md
--rw-r--r--   0        0        0     1126 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mecanum/drake_obstacles.dmd.yaml
--rw-r--r--   0        0        0     3138 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mecanum/ground.sdf
--rw-r--r--   0        0        0    61205 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mecanum/mecanum_base.urdf
--rw-r--r--   0        0        0      673 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mecanum/obstacle_boxes.sdf
--rw-r--r--   0        0        0      663 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mecanum/obstacles.sdf
--rw-r--r--   0        0        0    19599 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mobile_iiwa14_primitive_collision.urdf
--rw-r--r--   0        0        0     1662 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mustard_w_cameras.dmd.yaml
--rw-r--r--   0        0        0      374 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/package.xml
--rw-r--r--   0        0        0     2574 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/planar_bin.sdf
--rw-r--r--   0        0        0     3716 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/planar_foam_brick_collision_as_visual.sdf
--rw-r--r--   0        0        0    12684 2024-03-29 13:38:05.672171 manipulation-2024.4.8/manipulation/models/planar_iiwa14_no_collision.urdf
--rw-r--r--   0        0        0     1185 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/planar_joint.sdf
--rw-r--r--   0        0        0     1114 2024-04-08 12:21:31.612057 manipulation-2024.4.8/manipulation/models/planar_manipulation_station.scenario.yaml
--rw-r--r--   0        0        0   141408 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/pr2_collision_fixed.urdf
--rw-r--r--   0        0        0     1836 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/pr2_shelves.dmd.yaml
--rw-r--r--   0        0        0    49209 2024-03-17 12:35:12.475299 manipulation-2024.4.8/manipulation/models/rubiks_cube.sdf
--rw-r--r--   0        0        0    15864 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/rubiks_cube_2_by_2.sdf
--rw-r--r--   0        0        0      111 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/schunk_wsg_50_welded_fingers.dmd.yaml
--rw-r--r--   0        0        0     2963 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/schunk_wsg_50_welded_fingers.sdf
--rw-r--r--   0        0        0     2660 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf
--rw-r--r--   0        0        0     2350 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/segmentation_and_grasp_scene.dmd.yaml
--rw-r--r--   0        0        0     2784 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/shelves.sdf
--rw-r--r--   0        0        0     2876 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/shelves_w_ellipsoid_collision.sdf
--rw-r--r--   0        0        0     1388 2024-03-27 11:26:12.916327 manipulation-2024.4.8/manipulation/models/simple_2d_cspace.xml
--rw-r--r--   0        0        0      462 2024-03-27 10:57:46.553239 manipulation-2024.4.8/manipulation/models/simple_2d_obstacle.obj
--rw-r--r--   0        0        0      778 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/spot/README.md
--rw-r--r--   0        0        0     4816 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/spot/read_spot_camera_intrinsics.py
--rw-r--r--   0        0        0       21 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/spot/requirements.txt
--rw-r--r--   0        0        0    27982 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/spot/spot_with_arm.urdf
--rw-r--r--   0        0        0     3548 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.scenario.yaml
--rw-r--r--   0        0        0    30003 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.urdf
--rw-r--r--   0        0        0      390 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/README.md
--rw-r--r--   0        0        0     6386 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/base.obj
--rw-r--r--   0        0        0     6203 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/head.obj
--rw-r--r--   0        0        0    40367 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/mid.obj
--rw-r--r--   0        0        0     1382 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/suction-base.urdf
--rw-r--r--   0        0        0     3060 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/suction-head.urdf
--rw-r--r--   0        0        0    82673 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/tip.obj
--rw-r--r--   0        0        0      642 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/two_bins.dmd.yaml
--rw-r--r--   0        0        0      686 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/two_bins.sdf
--rw-r--r--   0        0        0     1915 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/two_bins_w_cameras.dmd.yaml
--rw-r--r--   0        0        0     2459 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/two_bins_w_cameras.sdf
--rw-r--r--   0        0        0    16331 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/two_link_iiwa14.urdf
--rw-r--r--   0        0        0     2148 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/mustard_depth_camera_example.py
--rw-r--r--   0        0        0     4190 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/pick.py
--rw-r--r--   0        0        0    26555 2024-04-08 12:21:31.612057 manipulation-2024.4.8/manipulation/scenarios.py
--rw-r--r--   0        0        0       90 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/station.md
--rw-r--r--   0        0        0    50383 2024-04-08 12:21:31.612057 manipulation-2024.4.8/manipulation/station.py
--rw-r--r--   0        0        0       90 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/systems.md
--rw-r--r--   0        0        0     4801 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/systems.py
--rw-r--r--   0        0        0     1547 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/test/test_create_sdf_from_mesh.py
--rw-r--r--   0        0        0     2292 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/test/test_gym.py
--rw-r--r--   0        0        0      425 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/test/test_meshcat_utils.py
--rw-r--r--   0        0        0      561 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/test/test_model_directives.py
--rw-r--r--   0        0        0      314 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/test/test_utils.py
--rw-r--r--   0        0        0       86 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/utils.md
--rw-r--r--   0        0        0     7226 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/utils.py
--rw-r--r--   0        0        0     3284 2024-04-08 12:21:57.004494 manipulation-2024.4.8/pyproject.toml
--rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 manipulation-2024.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1561 2024-02-22 14:57:44.046800 manipulation-2024.5.18/LICENSE.TXT
+-rw-r--r--   0        0        0      536 2024-05-21 02:06:24.674757 manipulation-2024.5.18/README.md
+-rw-r--r--   0        0        0      167 2024-02-22 14:57:44.110801 manipulation-2024.5.18/manipulation/__init__.py
+-rw-r--r--   0        0        0      846 2024-02-22 14:57:44.110801 manipulation-2024.5.18/manipulation/_static/custom.css
+-rw-r--r--   0        0        0     6481 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/clutter.py
+-rw-r--r--   0        0        0      891 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/conf.py
+-rw-r--r--   0        0        0    16339 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/create_sdf_from_mesh.py
+-rw-r--r--   0        0        0      211 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/drake_gym.py
+-rw-r--r--   0        0        0     9221 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/envs/box_flipup.py
+-rw-r--r--   0        0        0     8473 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/envs/planar_gripper_pushing_a_box.py
+-rw-r--r--   0        0        0    32464 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/clutter/normal_solution.npy
+-rw-r--r--   0        0        0     1724 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/clutter/test_analytic_grasp.py
+-rw-r--r--   0        0        0     6751 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/clutter/test_grasp_candidate.py
+-rw-r--r--   0        0        0     1768 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/clutter/test_normal.py
+-rw-r--r--   0        0        0     3978 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/clutter/test_simulation_tuning.py
+-rw-r--r--   0        0        0     3598 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/deep_perception/test_contrastive.py
+-rw-r--r--   0        0        0     1563 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/force/test_hybrid.py
+-rw-r--r--   0        0        0     4758 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/grader.py
+-rw-r--r--   0        0        0     3934 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/mobile/test_mobile_base_ik.py
+-rw-r--r--   0        0        0     1188 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pick/plot_planar_manipulator.py
+-rw-r--r--   0        0        0    26806 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pick/test_differential_ik.py
+-rw-r--r--   0        0        0     3585 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pick/test_planar_manipulator.py
+-rw-r--r--   0        0        0     2874 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pick/test_rigid_transforms.py
+-rw-r--r--   0        0        0     1881 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pick/test_robot_painter.py
+-rw-r--r--   0        0        0     1139 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pick/test_simple_qp.py
+-rw-r--r--   0        0        0     3642 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pose/test_icp.py
+-rw-r--r--   0        0        0     1445 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pose/test_pose_estimation.py
+-rw-r--r--   0        0        0     3240 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/pose/test_ransac.py
+-rw-r--r--   0        0        0     3380 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/rl/test_stochastic_optimization.py
+-rw-r--r--   0        0        0     2825 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/rl/test_vpg.py
+-rw-r--r--   0        0        0      870 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/robot/test_direct_joint_control.py
+-rw-r--r--   0        0        0     1184 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/robot/test_hardware_station_io.py
+-rw-r--r--   0        0        0     2261 2024-02-22 14:57:44.114801 manipulation-2024.5.18/manipulation/exercises/robot/test_reflected_inertia.py
+-rw-r--r--   0        0        0      672 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/robot/test_survey.py
+-rw-r--r--   0        0        0     1372 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/segmentation/test_mask.py
+-rw-r--r--   0        0        0     2271 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/segmentation/test_segmentation_and_grasp.py
+-rw-r--r--   0        0        0        0 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/__init__.py
+-rw-r--r--   0        0        0    23490 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/geometry.py
+-rw-r--r--   0        0        0     3711 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py
+-rw-r--r--   0        0        0     6529 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/robot.py
+-rw-r--r--   0        0        0    14614 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py
+-rw-r--r--   0        0        0     1464 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/test_door_opening.py
+-rw-r--r--   0        0        0     2391 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/test_rrt_planning.py
+-rw-r--r--   0        0        0     5489 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/exercises/trajectories/test_taskspace_iris.py
+-rw-r--r--   0        0        0     3764 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/icp.py
+-rw-r--r--   0        0        0      243 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/index.md
+-rw-r--r--   0        0        0      256 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/meshcat_cpp_utils.py
+-rw-r--r--   0        0        0      102 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/meshcat_utils.md
+-rw-r--r--   0        0        0    17872 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/meshcat_utils.py
+-rw-r--r--   0        0        0     5938 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf
+-rw-r--r--   0        0        0     1656 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/models/book.sdf
+-rw-r--r--   0        0        0     1280 2024-02-22 14:57:44.118801 manipulation-2024.5.18/manipulation/models/bunny/README
+-rw-r--r--   0        0        0   658744 2024-02-22 14:57:44.122801 manipulation-2024.5.18/manipulation/models/bunny/bun_zipper_res2.ply
+-rw-r--r--   0        0        0   196232 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/bunny/bunny.npy
+-rw-r--r--   0        0        0     1496 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/camera_box.sdf
+-rw-r--r--   0        0        0      155 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/clutter.dmd.yaml
+-rw-r--r--   0        0        0     1544 2024-04-08 12:21:31.612057 manipulation-2024.5.18/manipulation/models/clutter.scenarios.yaml
+-rw-r--r--   0        0        0      367 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/clutter_mustard.dmd.yaml
+-rw-r--r--   0        0        0      183 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/clutter_planning.dmd.yaml
+-rw-r--r--   0        0        0      165 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/clutter_w_cameras.dmd.yaml
+-rw-r--r--   0        0        0     1976 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/cupboard.scenario.yaml
+-rw-r--r--   0        0        0     2485 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/double_pendulum.urdf
+-rw-r--r--   0        0        0      215 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/floating_joint.urdf
+-rw-r--r--   0        0        0     1407 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/floor.sdf
+-rw-r--r--   0        0        0     1472 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/hydro/003_cracker_box.sdf
+-rw-r--r--   0        0        0     1470 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/hydro/004_sugar_box.sdf
+-rw-r--r--   0        0        0     1631 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/hydro/005_tomato_soup_can.sdf
+-rw-r--r--   0        0        0     4991 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/hydro/006_mustard_bottle.sdf
+-rw-r--r--   0        0        0     1480 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/hydro/009_gelatin_box.sdf
+-rw-r--r--   0        0        0     1476 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/hydro/010_potted_meat_can.sdf
+-rw-r--r--   0        0        0     1104 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/061_foam_brick.sdf
+-rw-r--r--   0        0        0      246 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/README.md
+-rw-r--r--   0        0        0     4709 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/bin.sdf
+-rw-r--r--   0        0        0     9110 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/cupboard.sdf
+-rw-r--r--   0        0        0     6069 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/extra_heavy_duty_table_surface_only_collision.sdf
+-rw-r--r--   0        0        0     5708 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/schunk_wsg_50_with_tip.sdf
+-rw-r--r--   0        0        0    21069 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_000.obj
+-rw-r--r--   0        0        0    21659 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_001.obj
+-rw-r--r--   0        0        0    23842 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_002.obj
+-rw-r--r--   0        0        0    24252 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_003.obj
+-rw-r--r--   0        0        0    26183 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_004.obj
+-rw-r--r--   0        0        0    15215 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_005.obj
+-rw-r--r--   0        0        0    18773 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_006.obj
+-rw-r--r--   0        0        0    23818 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_007.obj
+-rw-r--r--   0        0        0    24964 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_008.obj
+-rw-r--r--   0        0        0      643 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/iiwa_and_wsg.dmd.yaml
+-rw-r--r--   0        0        0      943 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/mecanum/README.md
+-rw-r--r--   0        0        0     1126 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/mecanum/drake_obstacles.dmd.yaml
+-rw-r--r--   0        0        0     3138 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/mecanum/ground.sdf
+-rw-r--r--   0        0        0    61205 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/mecanum/mecanum_base.urdf
+-rw-r--r--   0        0        0      673 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/mecanum/obstacle_boxes.sdf
+-rw-r--r--   0        0        0      663 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/mecanum/obstacles.sdf
+-rw-r--r--   0        0        0    19606 2024-04-22 09:52:20.076913 manipulation-2024.5.18/manipulation/models/mobile_iiwa14_primitive_collision.urdf
+-rw-r--r--   0        0        0     1645 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/mustard_w_cameras.dmd.yaml
+-rw-r--r--   0        0        0      374 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/package.xml
+-rw-r--r--   0        0        0     2574 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/planar_bin.sdf
+-rw-r--r--   0        0        0     3716 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/planar_foam_brick_collision_as_visual.sdf
+-rw-r--r--   0        0        0    12699 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/planar_iiwa14_no_collision.urdf
+-rw-r--r--   0        0        0     1185 2024-02-22 14:57:44.126801 manipulation-2024.5.18/manipulation/models/planar_joint.sdf
+-rw-r--r--   0        0        0     1114 2024-04-08 12:21:31.612057 manipulation-2024.5.18/manipulation/models/planar_manipulation_station.scenario.yaml
+-rw-r--r--   0        0        0   140342 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/pr2_collision_fixed.urdf
+-rw-r--r--   0        0        0     1791 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/pr2_shelves.dmd.yaml
+-rw-r--r--   0        0        0    49209 2024-03-17 12:35:12.475299 manipulation-2024.5.18/manipulation/models/rubiks_cube.sdf
+-rw-r--r--   0        0        0    15864 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/rubiks_cube_2_by_2.sdf
+-rw-r--r--   0        0        0      111 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/schunk_wsg_50_welded_fingers.dmd.yaml
+-rw-r--r--   0        0        0     2963 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/schunk_wsg_50_welded_fingers.sdf
+-rw-r--r--   0        0        0     2660 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf
+-rw-r--r--   0        0        0     2299 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/segmentation_and_grasp_scene.dmd.yaml
+-rw-r--r--   0        0        0     2784 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/shelves.sdf
+-rw-r--r--   0        0        0     2876 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/shelves_w_ellipsoid_collision.sdf
+-rw-r--r--   0        0        0     1388 2024-03-27 11:26:12.916327 manipulation-2024.5.18/manipulation/models/simple_2d_cspace.xml
+-rw-r--r--   0        0        0      462 2024-03-27 10:57:46.553239 manipulation-2024.5.18/manipulation/models/simple_2d_obstacle.obj
+-rw-r--r--   0        0        0      778 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/spot/README.md
+-rw-r--r--   0        0        0     4816 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/spot/read_spot_camera_intrinsics.py
+-rw-r--r--   0        0        0       21 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/spot/requirements.txt
+-rw-r--r--   0        0        0    27982 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/spot/spot_with_arm.urdf
+-rw-r--r--   0        0        0     3866 2024-05-21 02:06:24.674757 manipulation-2024.5.18/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.scenario.yaml
+-rw-r--r--   0        0        0    30003 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.urdf
+-rw-r--r--   0        0        0      390 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/README.md
+-rw-r--r--   0        0        0     6386 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/base.obj
+-rw-r--r--   0        0        0     6203 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/head.obj
+-rw-r--r--   0        0        0    40367 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/mid.obj
+-rw-r--r--   0        0        0     1382 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/suction-base.urdf
+-rw-r--r--   0        0        0     3060 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/suction-head.urdf
+-rw-r--r--   0        0        0    82673 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/suction/tip.obj
+-rw-r--r--   0        0        0      642 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/two_bins.dmd.yaml
+-rw-r--r--   0        0        0      668 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/two_bins.sdf
+-rw-r--r--   0        0        0     1915 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/models/two_bins_w_cameras.dmd.yaml
+-rw-r--r--   0        0        0     2441 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/two_bins_w_cameras.sdf
+-rw-r--r--   0        0        0    16346 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/models/two_link_iiwa14.urdf
+-rw-r--r--   0        0        0     2148 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/mustard_depth_camera_example.py
+-rw-r--r--   0        0        0     4190 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/pick.py
+-rw-r--r--   0        0        0    26538 2024-04-22 09:52:20.080913 manipulation-2024.5.18/manipulation/scenarios.py
+-rw-r--r--   0        0        0       90 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/station.md
+-rw-r--r--   0        0        0    51887 2024-05-21 02:06:24.674757 manipulation-2024.5.18/manipulation/station.py
+-rw-r--r--   0        0        0       90 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/systems.md
+-rw-r--r--   0        0        0     4801 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/systems.py
+-rw-r--r--   0        0        0     1547 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/test/test_create_sdf_from_mesh.py
+-rw-r--r--   0        0        0     2292 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/test/test_gym.py
+-rw-r--r--   0        0        0      425 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/test/test_meshcat_utils.py
+-rw-r--r--   0        0        0      561 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/test/test_model_directives.py
+-rw-r--r--   0        0        0      314 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/test/test_utils.py
+-rw-r--r--   0        0        0       86 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/utils.md
+-rw-r--r--   0        0        0     7226 2024-02-22 14:57:44.130802 manipulation-2024.5.18/manipulation/utils.py
+-rw-r--r--   0        0        0     3284 2024-05-21 02:06:24.674757 manipulation-2024.5.18/pyproject.toml
+-rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 manipulation-2024.5.18/PKG-INFO
```

### Comparing `manipulation-2024.4.8/LICENSE.TXT` & `manipulation-2024.5.18/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/_static/custom.css` & `manipulation-2024.5.18/manipulation/_static/custom.css`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/clutter.py` & `manipulation-2024.5.18/manipulation/clutter.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/conf.py` & `manipulation-2024.5.18/manipulation/conf.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/create_sdf_from_mesh.py` & `manipulation-2024.5.18/manipulation/create_sdf_from_mesh.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/envs/box_flipup.py` & `manipulation-2024.5.18/manipulation/envs/box_flipup.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/envs/planar_gripper_pushing_a_box.py` & `manipulation-2024.5.18/manipulation/envs/planar_gripper_pushing_a_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         FixedOffsetFrame(
             "planar_joint_frame",
             plant.world_frame(),
             RigidTransform(RotationMatrix.MakeXRotation(np.pi / 2)),
         )
     )
     box = parser.AddModelsFromUrl(
-        "package://drake/examples/manipulation_station/models/061_foam_brick.sdf"
+        "package://drake_models/manipulation_station/061_foam_brick.sdf"
     )[0]
     box_frame = plant.AddFrame(
         FixedOffsetFrame(
             "box_frame",
             plant.GetFrameByName("base_link", box),
             RigidTransform(RotationMatrix.MakeXRotation(np.pi / 2)),
         )
```

### Comparing `manipulation-2024.4.8/manipulation/exercises/clutter/normal_solution.npy` & `manipulation-2024.5.18/manipulation/exercises/clutter/normal_solution.npy`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/clutter/test_analytic_grasp.py` & `manipulation-2024.5.18/manipulation/exercises/clutter/test_analytic_grasp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/clutter/test_grasp_candidate.py` & `manipulation-2024.5.18/manipulation/exercises/clutter/test_grasp_candidate.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/clutter/test_normal.py` & `manipulation-2024.5.18/manipulation/exercises/clutter/test_normal.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/clutter/test_simulation_tuning.py` & `manipulation-2024.5.18/manipulation/exercises/clutter/test_simulation_tuning.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/deep_perception/test_contrastive.py` & `manipulation-2024.5.18/manipulation/exercises/deep_perception/test_contrastive.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/force/test_hybrid.py` & `manipulation-2024.5.18/manipulation/exercises/force/test_hybrid.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/grader.py` & `manipulation-2024.5.18/manipulation/exercises/grader.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/mobile/test_mobile_base_ik.py` & `manipulation-2024.5.18/manipulation/exercises/mobile/test_mobile_base_ik.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/pick/plot_planar_manipulator.py` & `manipulation-2024.5.18/manipulation/exercises/pick/plot_planar_manipulator.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/pick/test_differential_ik.py` & `manipulation-2024.5.18/manipulation/exercises/pick/test_differential_ik.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/pick/test_planar_manipulator.py` & `manipulation-2024.5.18/manipulation/exercises/pick/test_planar_manipulator.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/pick/test_rigid_transforms.py` & `manipulation-2024.5.18/manipulation/exercises/pick/test_rigid_transforms.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/pick/test_robot_painter.py` & `manipulation-2024.5.18/manipulation/exercises/pick/test_robot_painter.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/pick/test_simple_qp.py` & `manipulation-2024.5.18/manipulation/exercises/pick/test_simple_qp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/pose/test_icp.py` & `manipulation-2024.5.18/manipulation/exercises/pose/test_icp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/pose/test_pose_estimation.py` & `manipulation-2024.5.18/manipulation/exercises/pose/test_pose_estimation.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/pose/test_ransac.py` & `manipulation-2024.5.18/manipulation/exercises/pose/test_ransac.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/rl/test_stochastic_optimization.py` & `manipulation-2024.5.18/manipulation/exercises/rl/test_stochastic_optimization.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/rl/test_vpg.py` & `manipulation-2024.5.18/manipulation/exercises/rl/test_vpg.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/robot/test_direct_joint_control.py` & `manipulation-2024.5.18/manipulation/exercises/robot/test_direct_joint_control.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/robot/test_hardware_station_io.py` & `manipulation-2024.5.18/manipulation/exercises/robot/test_hardware_station_io.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/robot/test_reflected_inertia.py` & `manipulation-2024.5.18/manipulation/exercises/robot/test_reflected_inertia.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/robot/test_survey.py` & `manipulation-2024.5.18/manipulation/exercises/robot/test_survey.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/segmentation/test_mask.py` & `manipulation-2024.5.18/manipulation/exercises/segmentation/test_mask.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/segmentation/test_segmentation_and_grasp.py` & `manipulation-2024.5.18/manipulation/exercises/segmentation/test_segmentation_and_grasp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/geometry.py` & `manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/geometry.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py` & `manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/robot.py` & `manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/robot.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py` & `manipulation-2024.5.18/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/trajectories/test_door_opening.py` & `manipulation-2024.5.18/manipulation/exercises/trajectories/test_door_opening.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/trajectories/test_rrt_planning.py` & `manipulation-2024.5.18/manipulation/exercises/trajectories/test_rrt_planning.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/exercises/trajectories/test_taskspace_iris.py` & `manipulation-2024.5.18/manipulation/exercises/trajectories/test_taskspace_iris.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/icp.py` & `manipulation-2024.5.18/manipulation/icp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/meshcat_utils.py` & `manipulation-2024.5.18/manipulation/meshcat_utils.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf` & `manipulation-2024.5.18/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/book.sdf` & `manipulation-2024.5.18/manipulation/models/book.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/bunny/README` & `manipulation-2024.5.18/manipulation/models/bunny/README`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/bunny/bun_zipper_res2.ply` & `manipulation-2024.5.18/manipulation/models/bunny/bun_zipper_res2.ply`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/bunny/bunny.npy` & `manipulation-2024.5.18/manipulation/models/bunny/bunny.npy`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/camera_box.sdf` & `manipulation-2024.5.18/manipulation/models/camera_box.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/clutter.scenarios.yaml` & `manipulation-2024.5.18/manipulation/models/clutter.scenarios.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/cupboard.scenario.yaml` & `manipulation-2024.5.18/manipulation/models/cupboard.scenario.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 directives:
 - add_model:
     name: iiwa
-    file: package://drake/manipulation/models/iiwa_description/iiwa7/iiwa7_no_collision.sdf
+    file: package://drake_models/iiwa_description/sdf/iiwa7_no_collision.sdf
     default_joint_positions:
         iiwa_joint_1: [0]
         iiwa_joint_2: [0.6]
         iiwa_joint_3: [0]
         iiwa_joint_4: [-1.75]
         iiwa_joint_5: [0]
         iiwa_joint_6: [ 1.0]
@@ -20,15 +20,15 @@
     parent: iiwa::iiwa_link_7
     child: wsg::body
     X_PC:
         translation: [0, 0, 0.114]
         rotation: !Rpy { deg: [90, 0, 90]}
 - add_model:
     name: table
-    file: package://drake/examples/manipulation_station/models/amazon_table_simplified.sdf
+    file: package://drake_models/manipulation_station/amazon_table_simplified.sdf
 - add_weld:
     parent: world
     child: table::amazon_table
     X_PC:
         translation: [0.3257, 0, -0.0127]
 - add_model:
     name: cupboard
```

### Comparing `manipulation-2024.4.8/manipulation/models/double_pendulum.urdf` & `manipulation-2024.5.18/manipulation/models/double_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/floor.sdf` & `manipulation-2024.5.18/manipulation/models/floor.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/003_cracker_box.sdf` & `manipulation-2024.5.18/manipulation/models/hydro/003_cracker_box.sdf`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
           <izz>0.002481</izz>
         </inertia>
       </inertial>
       <visual name="base_link_cracker">
         <pose>-0.014 0.103 0.013 1.57 -1.57 0</pose>
         <geometry>
           <mesh>
-            <uri>package://drake_models/ycb/meshes/003_cracker_box_textured.obj</uri>
+            <uri>package://drake_models/ycb/meshes/003_cracker_box_textured.gltf</uri>
           </mesh>
         </geometry>
       </visual>
       <collision name="box_collision">
         <geometry>
           <box>
             <size>0.158000 0.207400 0.065800</size>
```

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/004_sugar_box.sdf` & `manipulation-2024.5.18/manipulation/models/hydro/004_sugar_box.sdf`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
           <izz>0.001699</izz>
         </inertia>
       </inertial>
       <visual name="base_link_sugar">
         <pose>-0.018  0.088  0.0039 -0.77 -1.52 2.36</pose>
         <geometry>
           <mesh>
-            <uri>package://drake_models/ycb/meshes/004_sugar_box_textured.obj</uri>
+            <uri>package://drake_models/ycb/meshes/004_sugar_box_textured.gltf</uri>
           </mesh>
         </geometry>
       </visual>
       <collision name="box_collision">
         <geometry>
           <box>
             <size>0.0900 0.170300 0.039100</size>
```

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/005_tomato_soup_can.sdf` & `manipulation-2024.5.18/manipulation/models/hydro/005_tomato_soup_can.sdf`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
           <izz>0.000402</izz>
         </inertia>
       </inertial>
       <visual name="base_link_soup">
         <pose>-0.0018  0.051 -0.084 1.57 0.13 0.0</pose>
         <geometry>
           <mesh>
-            <uri>package://drake_models/ycb/meshes/005_tomato_soup_can_textured.obj</uri>
+            <uri>package://drake_models/ycb/meshes/005_tomato_soup_can_textured.gltf</uri>
           </mesh>
         </geometry>
       </visual>
       <collision name="cylinder_collision">
         <pose>0 0 0 -1.57 0 0</pose>
         <geometry>
           <cylinder>
```

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/006_mustard_bottle.sdf` & `manipulation-2024.5.18/manipulation/models/hydro/006_mustard_bottle.sdf`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         <mass>0.435</mass>
         <pose>-0.015 -0.0231 0.0751 0 0 0</pose>
       </inertial>
 
       <visual name="visual">
         <geometry>
           <mesh>
-            <uri>package://drake_models/ycb/meshes/006_mustard_bottle_textured.obj</uri>
+            <uri>package://drake_models/ycb/meshes/006_mustard_bottle_textured.gltf</uri>
           </mesh>
         </geometry>
       </visual>
 
       <collision name="collision_0">
         <geometry>
           <mesh>
```

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/009_gelatin_box.sdf` & `manipulation-2024.5.18/manipulation/models/hydro/009_gelatin_box.sdf`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
           <izz>0.000108</izz>
         </inertia>
       </inertial>
       <visual name="base_link_gelatin">
         <pose>-0.0029 0.024 -0.015 -0.0085 -0.002 1.34</pose>
         <geometry>
           <mesh>
-            <uri>package://drake_models/ycb/meshes/009_gelatin_box_textured.obj</uri>
+            <uri>package://drake_models/ycb/meshes/009_gelatin_box_textured.gltf</uri>
           </mesh>
         </geometry>
       </visual>
       <collision name="box_collision">
         <geometry>
           <box>
             <size>0.08700 0.0700 0.026000</size>
```

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/010_potted_meat_can.sdf` & `manipulation-2024.5.18/manipulation/models/hydro/010_potted_meat_can.sdf`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
           <izz>0.000533</izz>
         </inertia>
       </inertial>
       <visual name="base_link_meat">
         <pose>0.034 0.039 0.025 1.57 0.052 0.0</pose>
         <geometry>
           <mesh>
-            <uri>package://drake_models/ycb/meshes/010_potted_meat_can_textured.obj</uri>
+            <uri>package://drake_models/ycb/meshes/010_potted_meat_can_textured.gltf</uri>
           </mesh>
         </geometry>
       </visual>
       <collision name="box_collision">
         <geometry>
           <box>
             <size>0.095 0.082 0.052600</size>
```

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/061_foam_brick.sdf` & `manipulation-2024.5.18/manipulation/models/hydro/061_foam_brick.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/bin.sdf` & `manipulation-2024.5.18/manipulation/models/hydro/bin.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/cupboard.sdf` & `manipulation-2024.5.18/manipulation/models/hydro/cupboard.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/extra_heavy_duty_table_surface_only_collision.sdf` & `manipulation-2024.5.18/manipulation/models/hydro/extra_heavy_duty_table_surface_only_collision.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/schunk_wsg_50_with_tip.sdf` & `manipulation-2024.5.18/manipulation/models/hydro/schunk_wsg_50_with_tip.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_000.obj` & `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_000.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_001.obj` & `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_001.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_002.obj` & `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_002.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_003.obj` & `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_003.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_004.obj` & `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_004.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_005.obj` & `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_005.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_006.obj` & `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_006.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_007.obj` & `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_007.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_008.obj` & `manipulation-2024.5.18/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_008.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/iiwa_and_wsg.dmd.yaml` & `manipulation-2024.5.18/manipulation/models/iiwa_and_wsg.dmd.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 directives:
 - add_model:
     name: iiwa
-    file: package://drake/manipulation/models/iiwa_description/iiwa7/iiwa7_no_collision.sdf
+    file: package://drake_models/iiwa_description/sdf/iiwa7_no_collision.sdf
     default_joint_positions:
         iiwa_joint_1: [-1.57]
         iiwa_joint_2: [0.1]
         iiwa_joint_3: [0]
         iiwa_joint_4: [-1.2]
         iiwa_joint_5: [0]
         iiwa_joint_6: [ 1.6]
```

### Comparing `manipulation-2024.4.8/manipulation/models/mecanum/README.md` & `manipulation-2024.5.18/manipulation/models/mecanum/README.md`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/mecanum/drake_obstacles.dmd.yaml` & `manipulation-2024.5.18/manipulation/models/mecanum/drake_obstacles.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/mecanum/ground.sdf` & `manipulation-2024.5.18/manipulation/models/mecanum/ground.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/mecanum/mecanum_base.urdf` & `manipulation-2024.5.18/manipulation/models/mecanum/mecanum_base.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/mecanum/obstacle_boxes.sdf` & `manipulation-2024.5.18/manipulation/models/mecanum/obstacle_boxes.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/mecanum/obstacles.sdf` & `manipulation-2024.5.18/manipulation/models/mecanum/obstacles.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/mobile_iiwa14_primitive_collision.urdf` & `manipulation-2024.5.18/manipulation/models/mobile_iiwa14_primitive_collision.urdf`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0"?>
 <!-- =================================================================================== -->
-<!-- |    This document was forked from drake/manipulation/models/iiwa_description/iiwa14_primitive_collision.urdf
+<!-- |    This document was forked from drake_models/iiwa_description/urdf/iiwa14_primitive_collision.urdf
 
 I've added a prismatic xyz base, and removed the joint position limits from the first revolute joint.
 <!-- =================================================================================== -->
 <!-- ===================================================================== -->
 <!-- Collision models: complex meshes can drastically affect run time.
      Therefore some collision models are represented as simple cylinders
      instead of meshes. However it's important to have accurate collision
@@ -81,15 +81,15 @@
       <origin rpy="0 0 0" xyz="-0.1 0 0.07"/>
       <mass value="5"/>
       <inertia ixx="0.05" ixy="0" ixz="0" iyy="0.06" iyz="0" izz="0.03"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_0.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_0.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="-0.015 0 0.07"/>
       <geometry>
         <cylinder length="0.17" radius="0.139"/>
@@ -117,15 +117,15 @@
       <origin rpy="0 0 0" xyz="0 -0.03 0.12"/>
       <mass value="5.76"/>
       <inertia ixx="0.033" ixy="0" ixz="0" iyy="0.0333" iyz="0" izz="0.0123"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_1.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_1.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 -0.014 0.14"/>
       <geometry>
         <cylinder length="0.29" radius="0.101"/>
@@ -149,22 +149,22 @@
       <!-- 3.95 kuka CAD value-->
       <!--4 Original Drake URDF value-->
       <inertia ixx="0.0305" ixy="0" ixz="0" iyy="0.011" iyz="0" izz="0.0304"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_orange.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_orange.gltf"/>
       </geometry>
       <material name="Orange"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_grey.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_grey.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="1.570796326794897 0 0" xyz="0 0.056 0.035"/>
       <geometry>
         <cylinder length="0.29" radius="0.101"/>
@@ -188,29 +188,29 @@
       <!--3.18 kuka CAD value-->
       <!--3 Original Drake URDF value-->
       <inertia ixx="0.025" ixy="0" ixz="0" iyy="0.0238" iyz="0" izz="0.0076"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_3.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_3.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.gltf"/>
       </geometry>
       <material name="Silver"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.gltf"/>
       </geometry>
       <material name="Black"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0.025 0.137"/>
       <geometry>
         <cylinder length="0.29" radius="0.092"/>
@@ -234,22 +234,22 @@
       <!--2.74 kuka CAD value-->
       <!--2.7 Original Drake URDF value-->
       <inertia ixx="0.017" ixy="0" ixz="0" iyy="0.006" iyz="0" izz="0.0164"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_orange.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_orange.gltf"/>
       </geometry>
       <material name="Orange"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_grey.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_grey.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="1.570796326794897 0 0" xyz="0 0.056 0.025"/>
       <geometry>
         <cylinder length="0.25" radius="0.092"/>
@@ -273,29 +273,29 @@
       <!--1.69 kuka CAD value-->
       <!--1.7 Original Drake URDF value-->
       <inertia ixx="0.01" ixy="0" ixz="0" iyy="0.0087" iyz="0" izz="0.00449"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_5.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_5.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.gltf"/>
       </geometry>
       <material name="Silver"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.gltf"/>
       </geometry>
       <material name="Black"/>
     </visual>
     <collision>
       <origin rpy="-0.3 0 0" xyz="0 0.03 0.13"/>
       <geometry>
         <cylinder length="0.29" radius="0.07"/>
@@ -319,22 +319,22 @@
       <!--1.8 kuka CAD value-->
       <!--1.8 Original Drake URDF value-->
       <inertia ixx="0.0049" ixy="0" ixz="0" iyy="0.0047" iyz="0" izz="0.0036"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_orange.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_orange.gltf"/>
       </geometry>
       <material name="Orange"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_grey.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_grey.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
         <!-- Note that the mesh-based collision model is intentionally being
@@ -360,15 +360,15 @@
       <!--0.31 kuka CAD value-->
       <!--0.3 Original Drake URDF value-->
       <inertia ixx="0.001" ixy="0" ixz="0" iyy="0.001" iyz="0" izz="0.001"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_7.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_7.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
         <!-- Note that the mesh-based collision model is intentionally being
```

### Comparing `manipulation-2024.4.8/manipulation/models/mustard_w_cameras.dmd.yaml` & `manipulation-2024.5.18/manipulation/models/mustard_w_cameras.dmd.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     X_PF:
         base_frame: world
         rotation: !Rpy { deg: [-90.0, 0.0, -90.0 ]}
         translation: [0, 0, 0.09515]
 
 - add_model:
     name: mustard
-    file: package://drake/manipulation/models/ycb/sdf/006_mustard_bottle.sdf
+    file: package://drake_models/ycb/006_mustard_bottle.sdf
 
 - add_weld:
     parent: mustard_origin
     child: mustard::base_link_mustard
 
 - add_frame:
     name: camera0_staging
```

### Comparing `manipulation-2024.4.8/manipulation/models/planar_bin.sdf` & `manipulation-2024.5.18/manipulation/models/planar_bin.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/planar_foam_brick_collision_as_visual.sdf` & `manipulation-2024.5.18/manipulation/models/planar_foam_brick_collision_as_visual.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/planar_iiwa14_no_collision.urdf` & `manipulation-2024.5.18/manipulation/models/planar_iiwa14_no_collision.urdf`

 * *Files 2% similar despite different names*

#### Comparing `manipulation-2024.4.8/manipulation/models/planar_iiwa14_no_collision.urdf` & `manipulation-2024.5.18/manipulation/models/planar_iiwa14_no_collision.urdf`

```diff
@@ -28,15 +28,15 @@
       <origin rpy="0 0 0" xyz="-0.1 0 0.07"/>
       <mass value="5"/>
       <inertia ixx="0.05" ixy="0" ixz="0" iyy="0.06" iyz="0" izz="0.03"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_0.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_0.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
   </link>
   <!-- joint between link_0 and link_1 -->
   <joint name="iiwa_joint_1" type="fixed">
     <parent link="iiwa_link_0"/>
@@ -48,15 +48,15 @@
       <origin rpy="0 0 0" xyz="0 -0.03 0.12"/>
       <mass value="5.76"/>
       <inertia ixx="0.033" ixy="0" ixz="0" iyy="0.0333" iyz="0" izz="0.0123"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_1.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_1.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
   </link>
   <!-- joint between link_1 and link_2 -->
   <joint name="iiwa_joint_2" type="revolute">
     <parent link="iiwa_link_1"/>
@@ -73,22 +73,22 @@
       <!-- 3.95 kuka CAD value-->
       <!--4 Original Drake URDF value-->
       <inertia ixx="0.0305" ixy="0" ixz="0" iyy="0.011" iyz="0" izz="0.0304"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_orange.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_orange.gltf"/>
       </geometry>
       <material name="Orange"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_grey.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_grey.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
   </link>
   <!-- joint between link_2 and link_3 -->
   <joint name="iiwa_joint_3" type="fixed">
     <parent link="iiwa_link_2"/>
@@ -102,29 +102,29 @@
       <!--3.18 kuka CAD value-->
       <!--3 Original Drake URDF value-->
       <inertia ixx="0.025" ixy="0" ixz="0" iyy="0.0238" iyz="0" izz="0.0076"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_3.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_3.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.gltf"/>
       </geometry>
       <material name="Silver"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.gltf"/>
       </geometry>
       <material name="Black"/>
     </visual>
   </link>
   <!-- joint between link_3 and link_4 -->
   <joint name="iiwa_joint_4" type="revolute">
     <parent link="iiwa_link_3"/>
@@ -141,22 +141,22 @@
       <!--2.74 kuka CAD value-->
       <!--2.7 Original Drake URDF value-->
       <inertia ixx="0.017" ixy="0" ixz="0" iyy="0.006" iyz="0" izz="0.0164"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_orange.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_orange.gltf"/>
       </geometry>
       <material name="Orange"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_grey.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_grey.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
   </link>
   <!-- joint between link_4 and link_5 -->
   <joint name="iiwa_joint_5" type="fixed">
     <parent link="iiwa_link_4"/>
@@ -170,29 +170,29 @@
       <!--1.69 kuka CAD value-->
       <!--1.7 Original Drake URDF value-->
       <inertia ixx="0.01" ixy="0" ixz="0" iyy="0.0087" iyz="0" izz="0.00449"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_5.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_5.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.gltf"/>
       </geometry>
       <material name="Silver"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.gltf"/>
       </geometry>
       <material name="Black"/>
     </visual>
   </link>
   <!-- joint between link_5 and link_6 -->
   <joint name="iiwa_joint_6" type="revolute">
     <parent link="iiwa_link_5"/>
@@ -209,22 +209,22 @@
       <!--1.8 kuka CAD value-->
       <!--1.8 Original Drake URDF value-->
       <inertia ixx="0.0049" ixy="0" ixz="0" iyy="0.0047" iyz="0" izz="0.0036"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_orange.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_orange.gltf"/>
       </geometry>
       <material name="Orange"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_grey.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_grey.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
   </link>
   <!-- joint between link_6 and link_7 -->
   <joint name="iiwa_joint_7" type="fixed">
     <parent link="iiwa_link_6"/>
@@ -238,15 +238,15 @@
       <!--0.31 kuka CAD value-->
       <!--0.3 Original Drake URDF value-->
       <inertia ixx="0.001" ixy="0" ixz="0" iyy="0.001" iyz="0" izz="0.001"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_7.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_7.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
   </link>
   <joint name="iiwa_joint_ee" type="fixed">
     <parent link="iiwa_link_7"/>
     <child link="iiwa_link_ee_kuka"/>
```

### Comparing `manipulation-2024.4.8/manipulation/models/planar_joint.sdf` & `manipulation-2024.5.18/manipulation/models/planar_joint.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/planar_manipulation_station.scenario.yaml` & `manipulation-2024.5.18/manipulation/models/planar_manipulation_station.scenario.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/pr2_collision_fixed.urdf` & `manipulation-2024.5.18/manipulation/models/pr2_collision_fixed.urdf`

 * *Files 3% similar despite different names*

#### Comparing `manipulation-2024.4.8/manipulation/models/pr2_collision_fixed.urdf` & `manipulation-2024.5.18/manipulation/models/pr2_collision_fixed.urdf`

```diff
@@ -145,22 +145,22 @@
       <mass value="116.0"/>
       <origin xyz="-0.061 0.0 0.293"/>
       <inertia ixx="5.652232699207" ixy="-0.009719934438" ixz="1.293988226423" iyy="5.669473158652" iyz="-0.007379583694" izz="3.683196351726"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/base.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/base.obj"/>
       </geometry>
       <material name="White"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/base_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/base_L.obj"/>
       </geometry>
     </collision>
   </link>
   <link name="base_footprint">
     <inertial>
       <mass value="1.0"/>
       <origin xyz="0 0 0"/>
@@ -251,22 +251,22 @@
       <mass value="3.473082"/>
       <origin xyz="0 0 0.07"/>
       <inertia ixx="0.012411765597" ixy="-0.000711733678" ixz="0.00050272983" iyy="0.015218160428" iyz="-0.000004273467" izz="0.011763977943"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/caster.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/caster.obj"/>
       </geometry>
       <material name="Caster"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/caster_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/caster_L.obj"/>
       </geometry>
     </collision> -->
   </link>
   <!-- <transmission name="fl_caster_rotation_trans" type="SimpleTransmission">
     <actuator name="fl_caster_rotation_motor"/>
     <joint name="fl_caster_rotation_joint"/>
   </transmission> -->
@@ -284,15 +284,15 @@
       <mass value="0.44036"/>
       <origin xyz="0 0 0"/>
       <inertia ixx="0.012411765597" ixy="-0.000711733678" ixz="0.00050272983" iyy="0.015218160428" iyz="-0.000004273467" izz="0.011763977943"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/wheel.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/wheel.obj"/>
       </geometry>
       <material name="Wheel_l"/>
     </visual>
     <!-- <collision>
       <origin rpy="1.57079632679 0 0" xyz="0 0 0"/>
       rotation because cyl. geom primitive has symmetry axis in +x direction
       <geometry>
@@ -325,15 +325,15 @@
       <mass value="0.44036"/>
       <origin xyz="0 0 0"/>
       <inertia ixx="0.012411765597" ixy="-0.000711733678" ixz="0.00050272983" iyy="0.015218160428" iyz="-0.000004273467" izz="0.011763977943"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/wheel.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/wheel.obj"/>
       </geometry>
       <material name="Wheel_r"/>
     </visual>
     <!-- <collision>
       <origin rpy="1.57079632679 0 0" xyz="0 0 0"/>
       rotation because cyl. geom primitive has symmetry axis in +x direction
       <geometry>
@@ -370,22 +370,22 @@
       <mass value="3.473082"/>
       <origin xyz="0 0 0.07"/>
       <inertia ixx="0.012411765597" ixy="-0.000711733678" ixz="0.00050272983" iyy="0.015218160428" iyz="-0.000004273467" izz="0.011763977943"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/caster.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/caster.obj"/>
       </geometry>
       <material name="Caster"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/caster_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/caster_L.obj"/>
       </geometry>
     </collision> -->
   </link>
   <!-- <transmission name="fr_caster_rotation_trans" type="SimpleTransmission">
     <actuator name="fr_caster_rotation_motor"/>
     <joint name="fr_caster_rotation_joint"/>
   </transmission> -->
@@ -403,15 +403,15 @@
       <mass value="0.44036"/>
       <origin xyz="0 0 0"/>
       <inertia ixx="0.012411765597" ixy="-0.000711733678" ixz="0.00050272983" iyy="0.015218160428" iyz="-0.000004273467" izz="0.011763977943"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/wheel.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/wheel.obj"/>
       </geometry>
       <material name="Wheel_l"/>
     </visual>
     <!-- <collision>
       <origin rpy="1.57079632679 0 0" xyz="0 0 0"/>
       rotation because cyl. geom primitive has symmetry axis in +x direction
       <geometry>
@@ -444,15 +444,15 @@
       <mass value="0.44036"/>
       <origin xyz="0 0 0"/>
       <inertia ixx="0.012411765597" ixy="-0.000711733678" ixz="0.00050272983" iyy="0.015218160428" iyz="-0.000004273467" izz="0.011763977943"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/wheel.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/wheel.obj"/>
       </geometry>
       <material name="Wheel_r"/>
     </visual>
     <!-- <collision>
       <origin rpy="1.57079632679 0 0" xyz="0 0 0"/>
       rotation because cyl. geom primitive has symmetry axis in +x direction
       <geometry>
@@ -489,22 +489,22 @@
       <mass value="3.473082"/>
       <origin xyz="0 0 0.07"/>
       <inertia ixx="0.012411765597" ixy="-0.000711733678" ixz="0.00050272983" iyy="0.015218160428" iyz="-0.000004273467" izz="0.011763977943"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/caster.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/caster.obj"/>
       </geometry>
       <material name="Caster"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/caster_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/caster_L.obj"/>
       </geometry>
     </collision> -->
   </link>
   <!-- <transmission name="bl_caster_rotation_trans" type="SimpleTransmission">
     <actuator name="bl_caster_rotation_motor"/>
     <joint name="bl_caster_rotation_joint"/>
   </transmission> -->
@@ -522,15 +522,15 @@
       <mass value="0.44036"/>
       <origin xyz="0 0 0"/>
       <inertia ixx="0.012411765597" ixy="-0.000711733678" ixz="0.00050272983" iyy="0.015218160428" iyz="-0.000004273467" izz="0.011763977943"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/wheel.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/wheel.obj"/>
       </geometry>
       <material name="Wheel_l"/>
     </visual>
     <!-- <collision>
       <origin rpy="1.57079632679 0 0" xyz="0 0 0"/>
       rotation because cyl. geom primitive has symmetry axis in +x direction
       <geometry>
@@ -563,15 +563,15 @@
       <mass value="0.44036"/>
       <origin xyz="0 0 0"/>
       <inertia ixx="0.012411765597" ixy="-0.000711733678" ixz="0.00050272983" iyy="0.015218160428" iyz="-0.000004273467" izz="0.011763977943"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/wheel.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/wheel.obj"/>
       </geometry>
       <material name="Wheel_r"/>
     </visual>
     <!-- <collision>
       <origin rpy="1.57079632679 0 0" xyz="0 0 0"/>
       rotation because cyl. geom primitive has symmetry axis in +x direction
       <geometry>
@@ -608,22 +608,22 @@
       <mass value="3.473082"/>
       <origin xyz="0 0 0.07"/>
       <inertia ixx="0.012411765597" ixy="-0.000711733678" ixz="0.00050272983" iyy="0.015218160428" iyz="-0.000004273467" izz="0.011763977943"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/caster.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/caster.obj"/>
       </geometry>
       <material name="Caster"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/caster_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/caster_L.obj"/>
       </geometry>
     </collision> -->
   </link>
   <!-- <transmission name="br_caster_rotation_trans" type="SimpleTransmission">
     <actuator name="br_caster_rotation_motor"/>
     <joint name="br_caster_rotation_joint"/>
   </transmission> -->
@@ -641,15 +641,15 @@
       <mass value="0.44036"/>
       <origin xyz="0 0 0"/>
       <inertia ixx="0.012411765597" ixy="-0.000711733678" ixz="0.00050272983" iyy="0.015218160428" iyz="-0.000004273467" izz="0.011763977943"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/wheel.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/wheel.obj"/>
       </geometry>
       <material name="Wheel_l"/>
     </visual>
     <!-- <collision>
       <origin rpy="1.57079632679 0 0" xyz="0 0 0"/>
       rotation because cyl. geom primitive has symmetry axis in +x direction
       <geometry>
@@ -682,15 +682,15 @@
       <mass value="0.44036"/>
       <origin xyz="0 0 0"/>
       <inertia ixx="0.012411765597" ixy="-0.000711733678" ixz="0.00050272983" iyy="0.015218160428" iyz="-0.000004273467" izz="0.011763977943"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/base_v0/wheel.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/base_v0/wheel.obj"/>
       </geometry>
       <material name="Wheel_r"/>
     </visual>
     <!-- <collision>
       <origin rpy="1.57079632679 0 0" xyz="0 0 0"/>
       rotation because cyl. geom primitive has symmetry axis in +x direction
       <geometry>
@@ -757,22 +757,22 @@
       <mass value="36.248046"/>
       <origin xyz="-0.1 0 -0.0885"/>
       <inertia ixx="2.771653750257" ixy="0.004284522609" ixz="-0.160418504506" iyy="2.510019507959" iyz="0.029664468704" izz="0.526432355569"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/torso_v0/torso_lift.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/torso_v0/torso_lift.obj"/>
       </geometry>
       <material name="Grey2"/>
     </visual>
     <collision name="torso_lift_collision">
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/torso_v0/torso_lift_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/torso_v0/torso_lift_L.obj"/>
       </geometry>
     </collision>
   </link>
   <gazebo reference="torso_lift_link">
     <sensor:contact name="torso_lift_contact_sensor">
       <geom>torso_lift_link_geom</geom>
       <updateRate>100.0</updateRate>
@@ -844,22 +844,22 @@
       <mass value="1.611118"/>
       <origin rpy="0 0 0" xyz="-0.005717  0.010312 -0.029649"/>
       <inertia ixx="0.00482611007" ixy="-0.000144683999" ixz="0.000110076136" iyy="0.005218991412" iyz="-0.000314239509" izz="0.008618784925"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0 " xyz="0 0 0.0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/head_v0/head_pan.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/head_v0/head_pan.obj"/>
       </geometry>
       <material name="Blue"/>
     </visual>
     <collision>
       <origin rpy="0 0 0 " xyz="0 0 0.0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/head_v0/head_pan_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/head_v0/head_pan_L.obj"/>
       </geometry>
     </collision>
   </link>
   <gazebo reference="head_pan_link">
     <material value="Gazebo/Black"/>
   </gazebo>
   <!-- <transmission name="head_pan_trans" type="SimpleTransmission">
@@ -881,22 +881,22 @@
       <mass value="1.749727"/>
       <origin rpy="0 0 0" xyz="0.041935 0.003569 0.028143"/>
       <inertia ixx="0.010602303435" ixy="-0.000408814235" ixz="0.00198303894" iyy="0.011874383747" iyz="0.000197908779" izz="0.005516790626"/>
     </inertial>
     <visual>
       <origin rpy="0.0 0.0 0.0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/head_v0/head_tilt.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/head_v0/head_tilt.obj"/>
       </geometry>
       <material name="Green"/>
     </visual>
     <collision>
       <origin rpy="0.0 0.0 0.0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/head_v0/head_tilt_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/head_v0/head_tilt_L.obj"/>
       </geometry>
     </collision>
   </link>
   <gazebo reference="head_tilt_link">
     <material value="Gazebo/White"/>
   </gazebo>
   <!-- <transmission name="head_tilt_trans" type="SimpleTransmission">
@@ -1413,22 +1413,22 @@
       <mass value="0.05"/>
       <origin rpy="0 0 0" xyz="-0.03 0 -0.03"/>
       <inertia ixx="0.0001" ixy="0" ixz="0" iyy="0.00001" iyz="0" izz="0.0001"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/tilting_laser_v0/tilting_hokuyo.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/tilting_laser_v0/tilting_hokuyo.obj"/>
       </geometry>
       <material name="Red"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/tilting_laser_v0/tilting_hokuyo_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/tilting_laser_v0/tilting_hokuyo_L.obj"/>
       </geometry>
     </collision> -->
   </link>
   <joint name="laser_tilt_joint" type="fixed">
     <axis xyz="0 1 0"/>
     <origin rpy="0 0 0" xyz="0 0 0.03"/>
     <parent link="laser_tilt_mount_link"/>
@@ -1502,22 +1502,22 @@
       <mass value="25.799322"/>
       <origin rpy="0 0 0" xyz="-0.001201 0.024513 -0.098231"/>
       <inertia ixx="0.866179142480" ixy="-0.06086507933" ixz="-0.12118061183" iyy="0.87421714893" iyz="-0.05886609911" izz="0.27353821674"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/shoulder_v0/shoulder_pan.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/shoulder_v0/shoulder_pan.obj"/>
       </geometry>
       <material name="Blue"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0.0 0 0.0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/shoulder_v0/shoulder_pan.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/shoulder_v0/shoulder_pan.obj"/>
       </geometry>
     </collision>
   </link>
   <joint name="r_shoulder_lift_joint" type="revolute">
     <axis xyz="0 1 0"/>
     <!-- Limits updated from Function's CAD values as of 2009_02_24 (link_data.xls) -->
     <limit effort="30" lower="-0.5236" upper="1.3963" velocity="2.082"/>
@@ -1533,22 +1533,22 @@
       <mass value="2.74988"/>
       <origin rpy="0 0 0" xyz="0.02195 -0.02664 -0.03127"/>
       <inertia ixx="0.02105584615" ixy="0.00496704022" ixz="-0.00194808955" iyy="0.02127223737" iyz="0.00110425490" izz="0.01975753814"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/shoulder_v0/shoulder_lift.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/shoulder_v0/shoulder_lift.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/shoulder_v0/shoulder_lift.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/shoulder_v0/shoulder_lift.obj"/>
       </geometry>
     </collision> -->
   </link>
   <joint name="r_upper_arm_roll_joint" type="revolute">
     <axis xyz="1 0 0"/>
     <origin rpy="0 0 0" xyz="0 0 0"/>
     <parent link="r_shoulder_lift_link"/>
@@ -1565,22 +1565,22 @@
       <origin rpy="0 0 0" xyz="0.0 0 0"/>
       <inertia ixx="0.01" ixy="0.00" ixz="0.00" iyy="0.01" iyz="0.00" izz="0.01"/>
     </inertial>
     <visual>
       <!-- TODO: This component doesn't actually have a mesh -->
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/shoulder_v0/upper_arm_roll.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/shoulder_v0/upper_arm_roll.obj"/>
       </geometry>
       <material name="RollLinks"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/shoulder_v0/upper_arm_roll_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/shoulder_v0/upper_arm_roll_L.obj"/>
       </geometry>
     </collision> -->
   </link>
   <gazebo reference="r_upper_arm_roll_link">
     <material value="PR2/RollLinks"/>
     <turnGravityOff>true</turnGravityOff>
   </gazebo>
@@ -1647,22 +1647,22 @@
       <mass value="6.01769"/>
       <origin xyz="0.21398 -0.01621 -0.0002"/>
       <inertia ixx="0.01537748957" ixy="0.00375711247" ixz="-0.00070852914" iyy="0.0747367044" iyz="-0.0001793645" izz="0.07608763307"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/upper_arm_v0/upper_arm.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/upper_arm_v0/upper_arm.obj"/>
       </geometry>
       <material name="Green"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/upper_arm_v0/upper_arm.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/upper_arm_v0/upper_arm.obj"/>
       </geometry>
     </collision>
   </link>
   <gazebo reference="r_upper_arm_link">
     <sensor:contact name="r_upper_arm_contact_sensor">
       <geom>r_upper_arm_link_geom</geom>
       <!-- TODO -->
@@ -1693,23 +1693,23 @@
       <mass value="0.1"/>
       <origin xyz="0 0 0"/>
       <inertia ixx="0.01" ixy="0.00" ixz="0.00" iyy="0.01" iyz="0.00" izz="0.01"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/upper_arm_v0/forearm_roll.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/upper_arm_v0/forearm_roll.obj"/>
       </geometry>
       <material name="RollLinks"/>
     </visual>
     <!-- TODO: collision tag should be optional -->
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/upper_arm_v0/forearm_roll_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/upper_arm_v0/forearm_roll_L.obj"/>
       </geometry>
     </collision> -->
   </link>
   <gazebo reference="r_forearm_roll_link">
     <material value="PR2/RollLinks"/>
     <turnGravityOff>true</turnGravityOff>
   </gazebo>
@@ -1736,22 +1736,22 @@
       <mass value="1.90327"/>
       <origin xyz="0.01014 0.00032 -0.01211"/>
       <inertia ixx="0.00346541989" ixy="0.00004066825" ixz="0.00043171614" iyy="0.00441606455" iyz="-0.00003968914" izz="0.00359156824"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/upper_arm_v0/elbow_flex.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/upper_arm_v0/elbow_flex.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/upper_arm_v0/elbow_flex.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/upper_arm_v0/elbow_flex.obj"/>
       </geometry>
     </collision> -->
   </link>
   <gazebo reference="r_elbow_flex_joint">
     <initial_joint_position>-1.0</initial_joint_position>
   </gazebo>
   <gazebo reference="r_elbow_flex_link">
@@ -1787,22 +1787,22 @@
       <mass value="2.57968"/>
       <origin xyz="0.18791 -0.00017 -0.00912"/>
       <inertia ixx="0.00364857222" ixy="0.00005215877" ixz="0.00071534842" iyy="0.01507736897" iyz="-0.00001310770" izz="0.01659310749"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/forearm_v0/forearm.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/forearm_v0/forearm.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/forearm_v0/forearm.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/forearm_v0/forearm.obj"/>
       </geometry>
     </collision>
   </link>
   <joint name="r_wrist_flex_joint" type="revolute">
     <axis xyz="0 1 0"/>
     <limit effort="10" lower="-2.094" upper="0.0" velocity="3.078"/>
     <!-- alpha tested velocity and effort limits -->
@@ -1817,22 +1817,22 @@
       <mass value="0.61402"/>
       <origin xyz="-0.00157 0.0 -0.00075"/>
       <inertia ixx="0.00065165722" ixy="0.00000028864" ixz="0.00000303477" iyy="0.00019824443" iyz="-0.00000022645" izz="0.00064450498"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/forearm_v0/wrist_flex.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/forearm_v0/wrist_flex.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/forearm_v0/wrist_flex.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/forearm_v0/wrist_flex.obj"/>
       </geometry>
     </collision> -->
   </link>
   <joint name="r_wrist_roll_joint" type="continuous">
     <axis xyz="1 0 0"/>
     <limit effort="10" velocity="3.6"/>
     <!-- alpha tested velocity and effort limits -->
@@ -1848,22 +1848,22 @@
       <mass value="0.1"/>
       <origin xyz="0 0 0"/>
       <inertia ixx="0.01" ixy="0" ixz="0" iyy="0.01" iyz="0" izz="0.01"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/forearm_v0/wrist_roll.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/forearm_v0/wrist_roll.obj"/>
       </geometry>
       <material name="RollLinks"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/forearm_v0/wrist_roll_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/forearm_v0/wrist_roll_L.obj"/>
       </geometry>
     </collision> -->
   </link>
   <gazebo reference="r_forearm_link">
     <turnGravityOff>true</turnGravityOff>
     <sensor:contact name="r_forearm_contact_sensor">
       <geom>r_forearm_link_geom</geom>
@@ -1937,22 +1937,22 @@
       <mass value="0.58007"/>
       <origin rpy="0 0 0" xyz="0.06623 0.00053 -0.00119"/>
       <inertia ixx="0.00035223921" ixy="-0.00001580476" ixz="-0.00000091750" iyy="0.00067741312" iyz="-0.00000059554" izz="0.00086563316"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/gripper_palm.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/gripper_palm.obj"/>
       </geometry>
       <material name="Red"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/gripper_palm.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/gripper_palm.obj"/>
       </geometry>
     </collision>
   </link>
   <joint name="r_gripper_led_joint" type="fixed">
     <!--  Need to check if we need a positive or negative Z term -->
     <origin xyz="0.0513 0.0 .0244"/>
     <parent link="r_gripper_palm_link"/>
@@ -2002,22 +2002,22 @@
       <mass value="0.17126"/>
       <origin rpy="0 0 0" xyz="0.03598 0.01730 -0.00164"/>
       <inertia ixx="0.00007756198" ixy="0.00000149095" ixz="-0.00000983385" iyy="0.00019708305" iyz="-0.00000306125" izz="0.00018105446"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
       </geometry>
     </collision>
   </link>
   <joint name="r_gripper_r_finger_joint" type="fixed">
     <axis xyz="0 0 -1"/>
     <origin rpy="0 0 0" xyz="0.07691 -0.01 0"/>
     <limit effort="1000.0" lower="0.0" upper="0.548" velocity="0.5"/>
@@ -2030,22 +2030,22 @@
       <mass value="0.17389"/>
       <origin rpy="0 0 0" xyz="0.03576 -0.01736 -0.00095"/>
       <inertia ixx="0.00007738410" ixy="-0.00000209309" ixz="-0.00000836228" iyy="0.00019847383" iyz="0.00000246110" izz="0.00018106988"/>
     </inertial>
     <visual>
       <origin rpy="3.14159265359 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="3.14159265359 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
       </geometry>
     </collision>
   </link>
   <joint name="r_gripper_l_parallel_root_joint" type="fixed">
     <axis xyz="0 0 1"/>
     <origin rpy="0 0 0" xyz="0.05891 0.031 0"/>
     <dynamics damping="0.2"/>
@@ -2118,22 +2118,22 @@
       <mass value="0.04419"/>
       <origin rpy="0 0 0" xyz="0.00423 0.00284 0.0"/>
       <inertia ixx="0.00000837047" ixy="0.00000583632" ixz="0.0" iyy="0.00000987067" iyz="0.0" izz="0.00001541768"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
       </geometry>
       <material name="Green"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
       </geometry>
     </collision>
   </link>
   <joint name="r_gripper_r_finger_tip_joint" type="fixed">
     <axis xyz="0 0 1"/>
     <origin rpy="0 0 0" xyz="0.09137 -0.00495 0"/>
     <limit effort="1000.0" lower="0.0" upper="0.548" velocity="0.5"/>
@@ -2146,22 +2146,22 @@
       <mass value="0.04419"/>
       <origin rpy="0 0 0" xyz="0.00423 -0.00284 0.0"/>
       <inertia ixx="0.00000837047" ixy="-0.00000583632" ixz="0.0" iyy="0.00000987067" iyz="0.0" izz="0.00001541768"/>
     </inertial>
     <visual>
       <origin rpy="3.14159265359 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
       </geometry>
       <material name="Green"/>
     </visual>
     <collision>
       <origin rpy="3.14159265359 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
       </geometry>
     </collision>
   </link>
   <gazebo reference="r_gripper_l_finger_link">
     <turnGravityOff>true</turnGravityOff>
     <sensor:contact name="r_gripper_l_finger_contact_sensor">
       <geom>r_gripper_l_finger_link_geom</geom>
@@ -2400,22 +2400,22 @@
       <mass value="25.799322"/>
       <origin rpy="0 0 0" xyz="-0.001201 0.024513 -0.098231"/>
       <inertia ixx="0.866179142480" ixy="-0.06086507933" ixz="-0.12118061183" iyy="0.87421714893" iyz="-0.05886609911" izz="0.27353821674"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/shoulder_v0/shoulder_pan.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/shoulder_v0/shoulder_pan.obj"/>
       </geometry>
       <material name="Blue"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0.0 0 0.0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/shoulder_v0/shoulder_pan.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/shoulder_v0/shoulder_pan.obj"/>
       </geometry>
     </collision>
   </link>
   <joint name="l_shoulder_lift_joint" type="revolute">
     <axis xyz="0 1 0"/>
     <!-- Limits updated from Function's CAD values as of 2009_02_24 (link_data.xls) -->
     <limit effort="30" lower="-0.5236" upper="1.3963" velocity="2.082"/>
@@ -2431,22 +2431,22 @@
       <mass value="2.74988"/>
       <origin rpy="0 0 0" xyz="0.02195 -0.02664 -0.03127"/>
       <inertia ixx="0.02105584615" ixy="0.00496704022" ixz="-0.00194808955" iyy="0.02127223737" iyz="0.00110425490" izz="0.01975753814"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/shoulder_v0/shoulder_lift.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/shoulder_v0/shoulder_lift.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/shoulder_v0/shoulder_lift.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/shoulder_v0/shoulder_lift.obj"/>
       </geometry>
     </collision> -->
   </link>
   <joint name="l_upper_arm_roll_joint" type="revolute">
     <axis xyz="1 0 0"/>
     <origin rpy="0 0 0" xyz="0 0 0"/>
     <parent link="l_shoulder_lift_link"/>
@@ -2463,22 +2463,22 @@
       <origin rpy="0 0 0" xyz="0.0 0 0"/>
       <inertia ixx="0.01" ixy="0.00" ixz="0.00" iyy="0.01" iyz="0.00" izz="0.01"/>
     </inertial>
     <visual>
       <!-- TODO: This component doesn't actually have a mesh -->
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/shoulder_v0/upper_arm_roll.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/shoulder_v0/upper_arm_roll.obj"/>
       </geometry>
       <material name="RollLinks"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/shoulder_v0/upper_arm_roll_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/shoulder_v0/upper_arm_roll_L.obj"/>
       </geometry>
     </collision> -->
   </link>
   <gazebo reference="l_upper_arm_roll_link">
     <material value="PR2/RollLinks"/>
     <turnGravityOff>true</turnGravityOff>
   </gazebo>
@@ -2545,22 +2545,22 @@
       <mass value="6.01769"/>
       <origin xyz="0.21405 0.01658 -0.00057"/>
       <inertia ixx="0.01530603856" ixy="-0.00339324862" ixz="0.00060765455" iyy="0.07473694455" iyz="-0.00019953729" izz="0.07601594191"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/upper_arm_v0/upper_arm.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/upper_arm_v0/upper_arm.obj"/>
       </geometry>
       <material name="Green"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/upper_arm_v0/upper_arm.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/upper_arm_v0/upper_arm.obj"/>
       </geometry>
     </collision>
   </link>
   <gazebo reference="l_upper_arm_link">
     <sensor:contact name="l_upper_arm_contact_sensor">
       <geom>l_upper_arm_link_geom</geom>
       <!-- TODO -->
@@ -2591,23 +2591,23 @@
       <mass value="0.1"/>
       <origin xyz="0 0 0"/>
       <inertia ixx="0.01" ixy="0.00" ixz="0.00" iyy="0.01" iyz="0.00" izz="0.01"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/upper_arm_v0/forearm_roll.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/upper_arm_v0/forearm_roll.obj"/>
       </geometry>
       <material name="RollLinks"/>
     </visual>
     <!-- TODO: collision tag should be optional -->
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/upper_arm_v0/forearm_roll_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/upper_arm_v0/forearm_roll_L.obj"/>
       </geometry>
     </collision> -->
   </link>
   <gazebo reference="l_forearm_roll_link">
     <material value="PR2/RollLinks"/>
     <turnGravityOff>true</turnGravityOff>
   </gazebo>
@@ -2634,22 +2634,22 @@
       <mass value="1.90327"/>
       <origin xyz="0.01014 0.00032 -0.01211"/>
       <inertia ixx="0.00346541989" ixy="0.00004066825" ixz="0.00043171614" iyy="0.00441606455" iyz="-0.00003968914" izz="0.00359156824"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/upper_arm_v0/elbow_flex.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/upper_arm_v0/elbow_flex.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/upper_arm_v0/elbow_flex.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/upper_arm_v0/elbow_flex.obj"/>
       </geometry>
     </collision> -->
   </link>
   <gazebo reference="l_elbow_flex_joint">
     <initial_joint_position>-1.0</initial_joint_position>
   </gazebo>
   <gazebo reference="l_elbow_flex_link">
@@ -2685,22 +2685,22 @@
       <mass value="2.57968"/>
       <origin xyz="0.18791 -0.00017 -0.00912"/>
       <inertia ixx="0.00364857222" ixy="0.00005215877" ixz="0.00071534842" iyy="0.01507736897" iyz="-0.00001310770" izz="0.01659310749"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/forearm_v0/forearm.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/forearm_v0/forearm.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/forearm_v0/forearm.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/forearm_v0/forearm.obj"/>
       </geometry>
     </collision>
   </link>
   <joint name="l_wrist_flex_joint" type="revolute">
     <axis xyz="0 1 0"/>
     <limit effort="10" lower="-2.094" upper="0.0" velocity="3.078"/>
     <!-- alpha tested velocity and effort limits -->
@@ -2715,22 +2715,22 @@
       <mass value="0.61402"/>
       <origin xyz="-0.00157 0.0 -0.00075"/>
       <inertia ixx="0.00065165722" ixy="0.00000028864" ixz="0.00000303477" iyy="0.00019824443" iyz="-0.00000022645" izz="0.00064450498"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/forearm_v0/wrist_flex.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/forearm_v0/wrist_flex.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/forearm_v0/wrist_flex.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/forearm_v0/wrist_flex.obj"/>
       </geometry>
     </collision> -->
   </link>
   <joint name="l_wrist_roll_joint" type="continuous">
     <axis xyz="1 0 0"/>
     <limit effort="10" velocity="3.6"/>
     <!-- alpha tested velocity and effort limits -->
@@ -2746,22 +2746,22 @@
       <mass value="0.1"/>
       <origin xyz="0 0 0"/>
       <inertia ixx="0.01" ixy="0" ixz="0" iyy="0.01" iyz="0" izz="0.01"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/forearm_v0/wrist_roll.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/forearm_v0/wrist_roll.obj"/>
       </geometry>
       <material name="RollLinks"/>
     </visual>
     <!-- <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/forearm_v0/wrist_roll_L.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/forearm_v0/wrist_roll_L.obj"/>
       </geometry>
     </collision> -->
   </link>
   <gazebo reference="l_forearm_link">
     <turnGravityOff>true</turnGravityOff>
     <sensor:contact name="l_forearm_contact_sensor">
       <geom>l_forearm_link_geom</geom>
@@ -2836,22 +2836,22 @@
       <mass value="0.58007"/>
       <origin rpy="0 0 0" xyz="0.06623 0.00053 -0.00119"/>
       <inertia ixx="0.00035223921" ixy="-0.00001580476" ixz="-0.00000091750" iyy="0.00067741312" iyz="-0.00000059554" izz="0.00086563316"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/gripper_palm.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/gripper_palm.obj"/>
       </geometry>
       <material name="Red"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/gripper_palm.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/gripper_palm.obj"/>
       </geometry>
     </collision>
   </link>
   <joint name="l_gripper_led_joint" type="fixed">
     <!--  Need to check if we need a positive or negative Z term -->
     <origin xyz="0.0513 0.0 .0244"/>
     <parent link="l_gripper_palm_link"/>
@@ -2901,22 +2901,22 @@
       <mass value="0.17126"/>
       <origin rpy="0 0 0" xyz="0.03598 0.01730 -0.00164"/>
       <inertia ixx="0.00007756198" ixy="0.00000149095" ixz="-0.00000983385" iyy="0.00019708305" iyz="-0.00000306125" izz="0.00018105446"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
       </geometry>
     </collision>
   </link>
   <joint name="l_gripper_r_finger_joint" type="fixed">
     <axis xyz="0 0 -1"/>
     <origin rpy="0 0 0" xyz="0.07691 -0.01 0"/>
     <limit effort="1000.0" lower="0.0" upper="0.548" velocity="0.5"/>
@@ -2929,22 +2929,22 @@
       <mass value="0.17389"/>
       <origin rpy="0 0 0" xyz="0.03576 -0.01736 -0.00095"/>
       <inertia ixx="0.00007738410" ixy="-0.00000209309" ixz="-0.00000836228" iyy="0.00019847383" iyz="0.00000246110" izz="0.00018106988"/>
     </inertial>
     <visual>
       <origin rpy="3.14159265359 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="3.14159265359 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger.obj"/>
       </geometry>
     </collision>
   </link>
   <joint name="l_gripper_l_parallel_root_joint" type="fixed">
     <axis xyz="0 0 1"/>
     <origin rpy="0 0 0" xyz="0.05891 0.031 0"/>
     <dynamics damping="0.2"/>
@@ -3017,22 +3017,22 @@
       <mass value="0.04419"/>
       <origin rpy="0 0 0" xyz="0.00423 0.00284 0.0"/>
       <inertia ixx="0.00000837047" ixy="0.00000583632" ixz="0.0" iyy="0.00000987067" iyz="0.0" izz="0.00001541768"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
       </geometry>
       <material name="Green"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
       </geometry>
     </collision>
   </link>
   <joint name="l_gripper_r_finger_tip_joint" type="fixed">
     <axis xyz="0 0 1"/>
     <origin rpy="0 0 0" xyz="0.09137 -0.00495 0"/>
     <limit effort="1000.0" lower="0.0" upper="0.548" velocity="0.5"/>
@@ -3045,22 +3045,22 @@
       <mass value="0.04419"/>
       <origin rpy="0 0 0" xyz="0.00423 -0.00284 0.0"/>
       <inertia ixx="0.00000837047" ixy="-0.00000583632" ixz="0.0" iyy="0.00000987067" iyz="0.0" izz="0.00001541768"/>
     </inertial>
     <visual>
       <origin rpy="3.14159265359 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
       </geometry>
       <material name="Green"/>
     </visual>
     <collision>
       <origin rpy="3.14159265359 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/examples/pr2/models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
+        <mesh filename="package://drake_models/pr2_description/meshes/gripper_v0/l_finger_tip.obj"/>
       </geometry>
     </collision>
   </link>
   <gazebo reference="l_gripper_l_finger_link">
     <turnGravityOff>true</turnGravityOff>
     <sensor:contact name="l_gripper_l_finger_contact_sensor">
       <geom>l_gripper_l_finger_link_geom</geom>
```

### Comparing `manipulation-2024.4.8/manipulation/models/pr2_shelves.dmd.yaml` & `manipulation-2024.5.18/manipulation/models/pr2_shelves.dmd.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -5,60 +5,60 @@
 - add_model:
     name: pr2
     file: package://manipulation/pr2_collision_fixed.urdf
 
 # Add shelves
 - add_model:
     name: shelves_1
-    file: package://drake/examples/manipulation_station/models/shelves.sdf
+    file: package://drake_models/manipulation_station/shelves.sdf
 
 - add_frame:
     name: shelf_1_origin
     X_PF:
       base_frame: world
       translation: [0.55, 0, 1.396706]
       rotation: !Rpy { deg: [0, 0, 0] }
 
 - add_weld:
     parent: shelf_1_origin
     child: shelves_1::shelves_body
 
 - add_model:
     name: shelves_2
-    file: package://drake/examples/manipulation_station/models/shelves.sdf
+    file: package://drake_models/manipulation_station/shelves.sdf
 
 - add_frame:
     name: shelf_2_origin
     X_PF:
       base_frame: world
       translation: [0, 0.85, 1.396706]
       rotation: !Rpy { deg: [0, 0, 90] }
 
 - add_weld:
     parent: shelf_2_origin
     child: shelves_2::shelves_body
 
 - add_model:
     name: shelves_3
-    file: package://drake/examples/manipulation_station/models/shelves.sdf
+    file: package://drake_models/manipulation_station/shelves.sdf
 
 - add_frame:
     name: shelf_3_origin
     X_PF:
       base_frame: world
       translation: [-0.55, 0, 1.396706]
       rotation: !Rpy { deg: [0, 0, 180] }
 
 - add_weld:
     parent: shelf_3_origin
     child: shelves_3::shelves_body
 
 - add_model:
     name: shelves_4
-    file: package://drake/examples/manipulation_station/models/shelves.sdf
+    file: package://drake_models/manipulation_station/shelves.sdf
 
 - add_frame:
     name: shelf_4_origin
     X_PF:
       base_frame: world
       translation: [0, -0.85, 1.396706]
       rotation: !Rpy { deg: [0, 0, -90] }
@@ -66,15 +66,15 @@
 - add_weld:
     parent: shelf_4_origin
     child: shelves_4::shelves_body
 
 # Add table
 - add_model:
     name: table
-    file: package://drake/examples/manipulation_station/models/table_wide.sdf
+    file: package://drake_models/manipulation_station/table_wide.sdf
 
 - add_frame:
     name: table_origin
     X_PF:
       base_frame: world
       translation: [0, 0, 0.996706]
```

### Comparing `manipulation-2024.4.8/manipulation/models/rubiks_cube.sdf` & `manipulation-2024.5.18/manipulation/models/rubiks_cube.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/rubiks_cube_2_by_2.sdf` & `manipulation-2024.5.18/manipulation/models/rubiks_cube_2_by_2.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/schunk_wsg_50_welded_fingers.sdf` & `manipulation-2024.5.18/manipulation/models/schunk_wsg_50_welded_fingers.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf` & `manipulation-2024.5.18/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/segmentation_and_grasp_scene.dmd.yaml` & `manipulation-2024.5.18/manipulation/models/segmentation_and_grasp_scene.dmd.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -6,45 +6,45 @@
     X_PF:
         base_frame: world
         rotation: !Rpy { deg: [0.0, 90, 0.0 ]}
         translation: [-0.1, -0.1, 0.079]
 
 - add_model:
     name: cracker
-    file: package://drake/manipulation/models/ycb/sdf/003_cracker_box.sdf
+    file: package://drake_models/ycb/003_cracker_box.sdf
 
 - add_weld:
     parent: cracker_origin
     child: cracker::base_link_cracker
 
 - add_frame:
     name: soup_origin
     X_PF:
         base_frame: world
         rotation: !Rpy { deg: [0.0, 00, 0.0 ]}
         translation: [0.05, 0.05, 0.033]
 
 - add_model:
     name: soup
-    file: package://drake/manipulation/models/ycb/sdf/005_tomato_soup_can.sdf
+    file: package://drake_models/ycb/005_tomato_soup_can.sdf
 
 - add_weld:
     parent: soup_origin
     child: soup::base_link_soup
 
 - add_frame:
     name: mustard_origin
     X_PF:
         base_frame: world
         rotation: !Rpy { deg: [-90.0, 0.0, -90.0 ]}
         translation: [-0.05, 0.1, 0.09515]
 
 - add_model:
     name: mustard
-    file: package://drake/manipulation/models/ycb/sdf/006_mustard_bottle.sdf
+    file: package://drake_models/ycb/006_mustard_bottle.sdf
 
 - add_weld:
     parent: mustard_origin
     child: mustard::base_link_mustard
 
 - add_frame:
     name: camera0_staging
```

### Comparing `manipulation-2024.4.8/manipulation/models/shelves.sdf` & `manipulation-2024.5.18/manipulation/models/shelves.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/shelves_w_ellipsoid_collision.sdf` & `manipulation-2024.5.18/manipulation/models/shelves_w_ellipsoid_collision.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/simple_2d_cspace.xml` & `manipulation-2024.5.18/manipulation/models/simple_2d_cspace.xml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/spot/README.md` & `manipulation-2024.5.18/manipulation/models/spot/README.md`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/spot/read_spot_camera_intrinsics.py` & `manipulation-2024.5.18/manipulation/models/spot/read_spot_camera_intrinsics.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/spot/spot_with_arm.urdf` & `manipulation-2024.5.18/manipulation/models/spot/spot_with_arm.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.scenario.yaml` & `manipulation-2024.5.18/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.scenario.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 - add_model:
     name: spot
     file: package://manipulation/spot/spot_with_arm_and_floating_base_actuators.urdf
     default_joint_positions:
         arm_sh1: [-3.1]
         arm_el0: [3.1]
 model_drivers:
-    spot: !InverseDynamicsDriver {}
+    spot: !InverseDynamicsDriver
+      gains:
+        arm_sh0: {kp: 1000, ki: 10, kd: 50}
+        arm_sh1: {kp: 1000, ki: 10, kd: 50}
+        arm_el0: {kp: 1000, ki: 10, kd: 50}
+        arm_el1: {kp: 1000, ki: 10, kd: 50}
+        arm_wr0: {kp: 1000, ki: 10, kd: 50}
+        arm_wr1: {kp: 1000, ki: 10, kd: 50}
+        arm_f1x: {kp: 3000, ki: 20, kd: 50}
 cameras:
   back:
     X_BC:
       rotation: !Rpy
         deg: [-0.46942074654099414, 0.3842180012895529, 0.023779786229513298]
       translation: [0.07679596000000007, -0.0023862200000000083, 0.00245293000000002]
     X_PB:
```

### Comparing `manipulation-2024.4.8/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.urdf` & `manipulation-2024.5.18/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/suction/base.obj` & `manipulation-2024.5.18/manipulation/models/suction/base.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/suction/head.obj` & `manipulation-2024.5.18/manipulation/models/suction/head.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/suction/mid.obj` & `manipulation-2024.5.18/manipulation/models/suction/mid.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/suction/suction-base.urdf` & `manipulation-2024.5.18/manipulation/models/suction/suction-base.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/suction/suction-head.urdf` & `manipulation-2024.5.18/manipulation/models/suction/suction-head.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/suction/tip.obj` & `manipulation-2024.5.18/manipulation/models/suction/tip.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/two_bins.dmd.yaml` & `manipulation-2024.5.18/manipulation/models/two_bins.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/two_bins.sdf` & `manipulation-2024.5.18/manipulation/models/two_bins.sdf`

 * *Files 18% similar despite different names*

#### Comparing `manipulation-2024.4.8/manipulation/models/two_bins.sdf` & `manipulation-2024.5.18/manipulation/models/two_bins.sdf`

```diff
@@ -1,22 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <sdf version="1.9">
   <model name="TwoBins">
     <include>
       <pose degrees="true">-0.05, -0.5, -0.015, 0, 0, 90</pose>
-      <uri>package://drake/examples/manipulation_station/models/bin.sdf</uri>
+      <uri>package://drake_models/manipulation_station/bin.sdf</uri>
       <name>bin0</name>
     </include>
     <joint name="weld0" type="fixed">
       <parent>world</parent>
       <child>bin0</child>
     </joint>
     <include>
       <pose degrees="true">0.5, 0.05, -0.015, 0, 0, 180</pose>
-      <uri>package://drake/examples/manipulation_station/models/bin.sdf</uri>
+      <uri>package://drake_models/manipulation_station/bin.sdf</uri>
       <name>bin1</name>
     </include>
     <joint name="weld1" type="fixed">
       <parent>world</parent>
       <child>bin1</child>
     </joint>
   </model>
```

### Comparing `manipulation-2024.4.8/manipulation/models/two_bins_w_cameras.dmd.yaml` & `manipulation-2024.5.18/manipulation/models/two_bins_w_cameras.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/models/two_bins_w_cameras.sdf` & `manipulation-2024.5.18/manipulation/models/two_bins_w_cameras.sdf`

 * *Files 3% similar despite different names*

#### Comparing `manipulation-2024.4.8/manipulation/models/two_bins_w_cameras.sdf` & `manipulation-2024.5.18/manipulation/models/two_bins_w_cameras.sdf`

```diff
@@ -1,22 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <sdf version="1.9">
   <model name="TwoBinsWCameras">
     <include>
       <pose degrees="true">-0.05, -0.5, -0.015, 0, 0, 90</pose>
-      <uri>package://drake/examples/manipulation_station/models/bin.sdf</uri>
+      <uri>package://drake_models/manipulation_station/bin.sdf</uri>
       <name>bin0</name>
     </include>
     <joint name="weld0" type="fixed">
       <parent>world</parent>
       <child>bin0</child>
     </joint>
     <include>
       <pose degrees="true">0.5, 0.05, -0.015, 0, 0, 180</pose>
-      <uri>package://drake/examples/manipulation_station/models/bin.sdf</uri>
+      <uri>package://drake_models/manipulation_station/bin.sdf</uri>
       <name>bin1</name>
     </include>
     <joint name="weld1" type="fixed">
       <parent>world</parent>
       <child>bin1</child>
     </joint>
     <include>
```

### Comparing `manipulation-2024.4.8/manipulation/models/two_link_iiwa14.urdf` & `manipulation-2024.5.18/manipulation/models/two_link_iiwa14.urdf`

 * *Files 2% similar despite different names*

#### Comparing `manipulation-2024.4.8/manipulation/models/two_link_iiwa14.urdf` & `manipulation-2024.5.18/manipulation/models/two_link_iiwa14.urdf`

```diff
@@ -27,15 +27,15 @@
       <origin rpy="0 0 0" xyz="-0.1 0 0.07"/>
       <mass value="5"/>
       <inertia ixx="0.05" ixy="0" ixz="0" iyy="0.06" iyz="0" izz="0.03"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_0.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_0.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="-0.015 0 0.07"/>
       <geometry>
         <cylinder length="0.17" radius="0.139"/>
@@ -60,15 +60,15 @@
       <origin rpy="0 0 0" xyz="0 -0.03 0.12"/>
       <mass value="5.76"/>
       <inertia ixx="0.033" ixy="0" ixz="0" iyy="0.0333" iyz="0" izz="0.0123"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_1.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_1.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 -0.03344534434 0.1974815417"/>
       <geometry>
         <sphere radius="0.07959901601"/>
@@ -93,22 +93,22 @@
       <!-- 3.95 kuka CAD value-->
       <!--4 Original Drake URDF value-->
       <inertia ixx="0.0305" ixy="0" ixz="0" iyy="0.0304" iyz="0" izz="0.011"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_orange.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_orange.gltf"/>
       </geometry>
       <material name="Orange"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_grey.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_grey.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="-2.488800594e-017 0.203225991 -0.002065464272"/>
       <geometry>
         <sphere radius="0.06602481863"/>
@@ -136,29 +136,29 @@
       <!--3.18 kuka CAD value-->
       <!--3 Original Drake URDF value-->
       <inertia ixx="0.025" ixy="0" ixz="0" iyy="0.0238" iyz="0" izz="0.0076"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_3.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_3.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.gltf"/>
       </geometry>
       <material name="Silver"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.gltf"/>
       </geometry>
       <material name="Black"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0.0355"/>
       <geometry>
         <sphere radius="0.075"/>
@@ -239,22 +239,22 @@
       <!--2.74 kuka CAD value-->
       <!--2.7 Original Drake URDF value-->
       <inertia ixx="0.017" ixy="0" ixz="0" iyy="0.0164" iyz="0" izz="0.006"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_orange.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_orange.gltf"/>
       </geometry>
       <material name="Orange"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_grey.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_grey.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0.01 0.046"/>
       <geometry>
         <sphere radius="0.078"/>
@@ -310,29 +310,29 @@
       <!--1.69 kuka CAD value-->
       <!--1.7 Original Drake URDF value-->
       <inertia ixx="0.01" ixy="0" ixz="0" iyy="0.0087" iyz="0" izz="0.00449"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_5.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_5.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.gltf"/>
       </geometry>
       <material name="Silver"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.gltf"/>
       </geometry>
       <material name="Black"/>
     </visual>
   </link>
   <!-- joint between link_5 and link_6 -->
   <joint name="iiwa_joint_6" type="fixed">
     <parent link="iiwa_link_5"/>
@@ -346,22 +346,22 @@
       <!--1.8 kuka CAD value-->
       <!--1.8 Original Drake URDF value-->
       <inertia ixx="0.0049" ixy="0" ixz="0" iyy="0.0047" iyz="0" izz="0.0036"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_orange.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_orange.gltf"/>
       </geometry>
       <material name="Orange"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_grey.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_grey.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 -0.059"/>
       <geometry>
         <sphere radius="0.055"/>
@@ -389,15 +389,15 @@
       <!--0.31 kuka CAD value-->
       <!--0.3 Original Drake URDF value-->
       <inertia ixx="0.001" ixy="0" ixz="0" iyy="0.001" iyz="0" izz="0.001"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_7.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_7.gltf"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0.001"/>
       <geometry>
         <sphere radius="0.06"/>
```

### Comparing `manipulation-2024.4.8/manipulation/mustard_depth_camera_example.py` & `manipulation-2024.5.18/manipulation/mustard_depth_camera_example.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/pick.py` & `manipulation-2024.5.18/manipulation/pick.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/scenarios.py` & `manipulation-2024.5.18/manipulation/scenarios.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     )
     return ExtractPose(body_index, X_BA)
 
 
 def AddIiwa(plant, collision_model="no_collision"):
     parser = Parser(plant)
     iiwa = parser.AddModelsFromUrl(
-        f"package://drake/manipulation/models/iiwa_description/iiwa7/iiwa7_{collision_model}.sdf"
+        f"package://drake_models/iiwa_description/sdf/iiwa7_{collision_model}.sdf"
     )[0]
     plant.WeldFrames(plant.world_frame(), plant.GetFrameByName("iiwa_link_0"))
 
     # Set default positions:
     q0 = [0.0, 0.1, 0, -1.2, 0, 1.6, 0]
     index = 0
     for joint_index in plant.GetJointIndices(iiwa):
@@ -92,15 +92,15 @@
             joint.set_default_angle(q0[index])
             index += 1
 
     return iiwa
 
 
 def AddPlanarIiwa(plant):
-    urdf = "package://drake/manipulation/models/iiwa_description/urdf/planar_iiwa14_spheres_dense_elbow_collision.urdf"
+    urdf = "package://drake_models/iiwa_description/urdf/planar_iiwa14_spheres_dense_elbow_collision.urdf"
 
     parser = Parser(plant)
     iiwa = parser.AddModelsFromUrl(urdf)[0]
     plant.WeldFrames(plant.world_frame(), plant.GetFrameByName("iiwa_link_0"))
 
     # Set default positions:
     q0 = [0.1, -1.2, 1.6]
@@ -141,15 +141,17 @@
     ConfigureParser(parser)
     if welded:
         if sphere:
             file = "package://manipulation/schunk_wsg_50_welded_fingers_sphere.sdf"
         else:
             file = "package://manipulation/schunk_wsg_50_welded_fingers.sdf"
     else:
-        file = "package://drake/manipulation/models/wsg_50_description/sdf/schunk_wsg_50_with_tip.sdf"
+        file = (
+            "package://drake_models/wsg_50_description/sdf/schunk_wsg_50_with_tip.sdf"
+        )
 
     directives = f"""
 directives:
 - add_model:
     name: gripper
     file: {file}
 """
```

### Comparing `manipulation-2024.4.8/manipulation/station.py` & `manipulation-2024.5.18/manipulation/station.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,21 +72,37 @@
 
 from manipulation.scenarios import AddIiwa, AddPlanarIiwa, AddWsg
 from manipulation.systems import ExtractPose
 from manipulation.utils import ConfigureParser
 
 
 @dc.dataclass
+class JointPidControllerGains:
+    """Defines the Proportional-Integral-Derivative gains for a single joint.
+
+    Args:
+        kp: The proportional gain.
+        ki: The integral gain.
+        kd: The derivative gain.
+    """
+
+    kp: float = 100  # Position gain
+    ki: float = 1  # Integral gain
+    kd: float = 20  # Velocity gain
+
+
+@dc.dataclass
 class InverseDynamicsDriver:
     """A simulation-only driver that adds the InverseDynamicsController to the
     station and exports the output ports. Multiple model instances can be driven with a
     single controller using `instance_name1+instance_name2` as the key; the output ports
     will be named similarly."""
 
-    # TODO(russt): Support setting the gains.
+    # Must have one element for every (named) actuator in the model_instance.
+    gains: typing.Mapping[str, JointPidControllerGains] = dc.field(default_factory=dict)
 
 
 @dc.dataclass
 class JointPdControllerGains:
     """Defines the Proportional-Derivative gains for a single joint.
 
     Args:
@@ -690,21 +706,41 @@
         ProcessModelDirectives(
             directives=ModelDirectives(directives=controller_directives),
             parser=parser,
         )
         controller_plant.Finalize()
 
         # Add the controller
-        # TODO(russt): Take the gains as parameters.
+
+        # When using multiple model instances, the model instance name must be prefixed.
+        # The strings should take the form {model_instance_name}_{joint_actuator_name}, as
+        # prescribed by MultiBodyPlant::GetActuatorNames().
+        add_model_instance_prefix = len(model_instance_names) > 1
+        actuator_names = controller_plant.GetActuatorNames(add_model_instance_prefix)
+
+        # Check that all actuator names are valid.
+        for actuator_name in driver_config.gains.keys():
+            if actuator_name not in actuator_names:
+                raise ValueError(
+                    f"Actuator '{actuator_name}' not found. Valid names are: {actuator_names}"
+                )
+
+        # Get gains for each joint from the config. Use default gains if it doesn't exist in the config.
+        default_gains = JointPidControllerGains()
+        gains: typing.List[JointPidControllerGains] = []
+        for actuator_name in actuator_names:
+            joint_gains = driver_config.gains.get(actuator_name, default_gains)
+            gains.append(joint_gains)
+
         controller = builder.AddSystem(
             InverseDynamicsController(
                 controller_plant,
-                kp=[100] * controller_plant.num_positions(),
-                ki=[1] * controller_plant.num_positions(),
-                kd=[20] * controller_plant.num_positions(),
+                kp=[joint_gains.kp for joint_gains in gains],
+                ki=[joint_gains.ki for joint_gains in gains],
+                kd=[joint_gains.kd for joint_gains in gains],
                 has_reference_acceleration=False,
             )
         )
         controller.set_name(model_instance_name + ".controller")
         if len(model_instances) == 1:
             builder.Connect(
                 sim_plant.get_state_output_port(model_instances[0]),
```

### Comparing `manipulation-2024.4.8/manipulation/systems.py` & `manipulation-2024.5.18/manipulation/systems.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/test/test_create_sdf_from_mesh.py` & `manipulation-2024.5.18/manipulation/test/test_create_sdf_from_mesh.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/test/test_gym.py` & `manipulation-2024.5.18/manipulation/test/test_gym.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/test/test_model_directives.py` & `manipulation-2024.5.18/manipulation/test/test_model_directives.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/manipulation/utils.py` & `manipulation-2024.5.18/manipulation/utils.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.4.8/pyproject.toml` & `manipulation-2024.5.18/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "manipulation"
 # Use e.g. 2023.10.4.rc0 if I need to release a release candidate.
 # Use e.g. 2023.10.4.post1 if I need to rerelease on the same day.
-version = "2024.04.08"
+version = "2024.05.18"
 description = "MIT 6.421 - Robotic Manipulation"
 authors = ["Russ Tedrake <russt@mit.edu>"]
 license = "BSD License"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License"
@@ -43,15 +43,15 @@
 url = "https://drake-packages.csail.mit.edu/whl/nightly/"
 priority = "explicit"
 
 [tool.poetry.dependencies]
 python = "<4.0,>=3.10"
 cloudpickle = "2.2.1"  # needs to be pinned for stored files to remain compatible.
 #drake = { version = "==0.0.20240302", source = "drake-nightly" }
-drake = ">=1.27.0"
+drake = ">=1.28.0"
 gradescope-utils = ">=0.4.0"
 mpld3  = ">=0.5.6"
 nevergrad = ">=0.4.3"  # TODO: avoid expensive bayesian optimization dep
 psutil = ">=5.9.*"
 #pymcubes = ">=0.0.9"
 pyzmq = ">=25.0.0" # seems to be needed on python 3.11
 scipy = ">=1.10.0"  # From github dependabot
@@ -65,15 +65,15 @@
 
 [tool.poetry.group.docs]
 optional = true
 
 # Must include all dependencies required to build the docs with sphinx + autodoc.
 [tool.poetry.group.docs.dependencies]
 #drake = { version = ">=0.0.20240302", source = "drake-nightly" }
-drake = ">=1.27.0"
+drake = ">=1.28.0"
 ipython = ">=7.8.0"
 sphinx = ">=7.2.6"
 myst-parser = ">=2.0.0"
 sphinx_rtd_theme = ">=2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 beautifulsoup4 = ">=4.6.3"
```

### Comparing `manipulation-2024.4.8/PKG-INFO` & `manipulation-2024.5.18/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: manipulation
-Version: 2024.4.8
+Version: 2024.5.18
 Summary: MIT 6.421 - Robotic Manipulation
 License: BSD License
 Author: Russ Tedrake
 Author-email: russt@mit.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cloudpickle (==2.2.1)
-Requires-Dist: drake (>=1.27.0)
+Requires-Dist: drake (>=1.28.0)
 Requires-Dist: gradescope-utils (>=0.4.0)
 Requires-Dist: mpld3 (>=0.5.6)
 Requires-Dist: nevergrad (>=0.4.3)
 Requires-Dist: psutil (>=5.9)
 Requires-Dist: pyzmq (>=25.0.0)
 Requires-Dist: scipy (>=1.10.0)
 Requires-Dist: stable-baselines3 (>=2.0.0)
@@ -33,12 +33,14 @@
 # Robotic Manipulation
 
 *Perception, Planning, and Control*
 
 This is the companion software for the textbook available at:
 https://manipulation.mit.edu/
 
+For contributions, please see [developer instructions](Developers.md).
+
 To cite this software (or the corresponding textbook), please use:
 
 Russ Tedrake. _Robotic Manipulation: Perception, Planning, and Control (Course
 Notes for MIT 6.421)._ Downloaded on [date] from <https://manipulation.mit.edu/>.
```

