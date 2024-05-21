# Comparing `tmp/gymnasium-0.29.1.tar.gz` & `tmp/gymnasium-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium-0.29.1.tar", last modified: Mon Aug 21 13:06:42 2023, max compression
+gzip compressed data, was "gymnasium-1.0.0a1.tar", last modified: Tue Feb 13 16:56:00 2024, max compression
```

## Comparing `gymnasium-0.29.1.tar` & `gymnasium-1.0.0a1.tar`

### file list

```diff
@@ -1,292 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.557651 gymnasium-0.29.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-21 13:06:26.000000 gymnasium-0.29.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-08-21 13:06:42.557651 gymnasium-0.29.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-08-21 13:06:26.000000 gymnasium-0.29.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.521651 gymnasium-0.29.1/gymnasium/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27785 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.525651 gymnasium-0.29.1/gymnasium/envs/
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.525651 gymnasium-0.29.1/gymnasium/envs/box2d/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/box2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31316 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/box2d/bipedal_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/box2d/car_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)    29145 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/box2d/car_racing.py
--rw-r--r--   0 runner    (1001) docker     (123)    32721 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/box2d/lunar_lander.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.525651 gymnasium-0.29.1/gymnasium/envs/classic_control/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/classic_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/classic_control/acrobot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.525651 gymnasium-0.29.1/gymnasium/envs/classic_control/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/classic_control/assets/clockwise.png
--rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/classic_control/cartpole.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/classic_control/continuous_mountain_car.py
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/classic_control/mountain_car.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/classic_control/pendulum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/classic_control/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.529651 gymnasium-0.29.1/gymnasium/envs/mujoco/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/ant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/ant_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/ant_v4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.533651 gymnasium-0.29.1/gymnasium/envs/mujoco/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/assets/ant.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/assets/half_cheetah.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/assets/hopper.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/assets/humanoid.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/assets/humanoidstandup.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/assets/inverted_double_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/assets/inverted_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/assets/point.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/assets/pusher.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/assets/reacher.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/assets/swimmer.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/assets/walker2d.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/half_cheetah.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/half_cheetah_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/half_cheetah_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/hopper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/hopper_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/hopper_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/humanoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/humanoid_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/humanoid_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/humanoidstandup.py
--rw-r--r--   0 runner    (1001) docker     (123)    23799 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/humanoidstandup_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/inverted_double_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/inverted_double_pendulum_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/inverted_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/inverted_pendulum_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/mujoco_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25376 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/mujoco_rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/pusher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/pusher_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/reacher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/reacher_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/swimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/swimmer_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/swimmer_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/walker2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/walker2d_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/mujoco/walker2d_v4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.533651 gymnasium-0.29.1/gymnasium/envs/phys2d/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/phys2d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.533651 gymnasium-0.29.1/gymnasium/envs/phys2d/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/phys2d/assets/clockwise.png
--rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/phys2d/cartpole.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/phys2d/pendulum.py
--rw-r--r--   0 runner    (1001) docker     (123)    43653 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.533651 gymnasium-0.29.1/gymnasium/envs/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17206 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/tabular/blackjack.py
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/tabular/cliffwalking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.533651 gymnasium-0.29.1/gymnasium/envs/toy_text/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/blackjack.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/cliffwalking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.533651 gymnasium-0.29.1/gymnasium/envs/toy_text/font/
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/font/Minecraft.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    15756 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/frozen_lake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.545651 gymnasium-0.29.1/gymnasium/envs/toy_text/img/
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/C2.png
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/C3.png
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/C4.png
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/C5.png
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/C6.png
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/C7.png
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/C8.png
--rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/C9.png
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/CA.png
--rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/CJ.png
--rw-r--r--   0 runner    (1001) docker     (123)    19498 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/CK.png
--rw-r--r--   0 runner    (1001) docker     (123)    18772 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/CQ.png
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/CT.png
--rw-r--r--   0 runner    (1001) docker     (123)    44172 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/Card.png
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/D2.png
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/D3.png
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/D4.png
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/D5.png
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/D6.png
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/D7.png
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/D8.png
--rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/D9.png
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/DA.png
--rw-r--r--   0 runner    (1001) docker     (123)    18468 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/DJ.png
--rw-r--r--   0 runner    (1001) docker     (123)    19118 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/DK.png
--rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/DQ.png
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/DT.png
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/H2.png
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/H3.png
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/H4.png
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/H5.png
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/H6.png
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/H7.png
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/H8.png
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/H9.png
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/HA.png
--rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/HJ.png
--rw-r--r--   0 runner    (1001) docker     (123)    19561 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/HK.png
--rw-r--r--   0 runner    (1001) docker     (123)    20159 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/HQ.png
--rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/HT.png
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/S2.png
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/S3.png
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/S4.png
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/S5.png
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/S6.png
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/S7.png
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/S8.png
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/S9.png
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/SA.png
--rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/SJ.png
--rw-r--r--   0 runner    (1001) docker     (123)    19256 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/SK.png
--rw-r--r--   0 runner    (1001) docker     (123)    19809 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/SQ.png
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/ST.png
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/cab_front.png
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/cab_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/cab_rear.png
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/cab_right.png
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/cookie.png
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/cracked_hole.png
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/elf_down.png
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/elf_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/elf_right.png
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/elf_up.png
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/goal.png
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/gridworld_median_bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/gridworld_median_horiz.png
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/gridworld_median_left.png
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/gridworld_median_right.png
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/gridworld_median_top.png
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/gridworld_median_vert.png
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/hole.png
--rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/hotel.png
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/ice.png
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/mountain_bg1.png
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/mountain_bg2.png
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/mountain_cliff.png
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/mountain_near-cliff1.png
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/mountain_near-cliff2.png
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/passenger.png
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/stool.png
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/img/taxi_background.png
--rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/taxi.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/envs/toy_text/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.545651 gymnasium-0.29.1/gymnasium/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/functional_jax_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.545651 gymnasium-0.29.1/gymnasium/experimental/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26861 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/vector/async_vector_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/vector/sync_vector_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.545651 gymnasium-0.29.1/gymnasium/experimental/vector/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/vector/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/vector/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/vector/utils/shared_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/vector/utils/space_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18213 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/vector/vector_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.549651 gymnasium-0.29.1/gymnasium/experimental/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/atari_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/jax_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/jax_to_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/lambda_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    23855 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/lambda_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/lambda_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/numpy_to_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/stateful_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/stateful_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/stateful_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.549651 gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/dict_info_to_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/jax_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/jax_to_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/numpy_to_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/record_episode_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/vectorize_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/vectorize_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/vectorize_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.549651 gymnasium-0.29.1/gymnasium/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/spaces/box.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/spaces/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/spaces/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/spaces/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/spaces/multi_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/spaces/multi_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/spaces/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/spaces/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/spaces/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/spaces/tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)    18914 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/spaces/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.553651 gymnasium-0.29.1/gymnasium/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/utils/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/utils/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/utils/env_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/utils/ezpickle.py
--rw-r--r--   0 runner    (1001) docker     (123)    16641 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/utils/passive_env_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/utils/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/utils/play.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/utils/record_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/utils/save_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/utils/seeding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/utils/step_api_compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.553651 gymnasium-0.29.1/gymnasium/vector/
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27833 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/vector/async_vector_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/vector/sync_vector_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.553651 gymnasium-0.29.1/gymnasium/vector/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/vector/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/vector/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/vector/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/vector/utils/shared_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/vector/utils/spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/vector/vector_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.557651 gymnasium-0.29.1/gymnasium/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/atari_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/autoreset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/clip_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/filter_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/flatten_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/frame_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/gray_scale_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/human_rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.557651 gymnasium-0.29.1/gymnasium/wrappers/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/monitoring/video_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/order_enforcing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/pixel_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/record_episode_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/record_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/render_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/rescale_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/resize_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/step_api_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/time_aware_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/transform_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/transform_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-08-21 13:06:27.000000 gymnasium-0.29.1/gymnasium/wrappers/vector_list_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.525651 gymnasium-0.29.1/gymnasium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-08-21 13:06:42.000000 gymnasium-0.29.1/gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-08-21 13:06:42.000000 gymnasium-0.29.1/gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 13:06:42.000000 gymnasium-0.29.1/gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-21 13:06:42.000000 gymnasium-0.29.1/gymnasium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-21 13:06:42.000000 gymnasium-0.29.1/gymnasium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-08-21 13:06:27.000000 gymnasium-0.29.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-21 13:06:42.557651 gymnasium-0.29.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-21 13:06:27.000000 gymnasium-0.29.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 13:06:42.557651 gymnasium-0.29.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-08-21 13:06:27.000000 gymnasium-0.29.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-08-21 13:06:27.000000 gymnasium-0.29.1/tests/testing_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.087967 gymnasium-1.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-13 16:55:48.000000 gymnasium-1.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-02-13 16:56:00.087967 gymnasium-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-02-13 16:55:48.000000 gymnasium-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.043967 gymnasium-1.0.0a1/gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26983 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.043967 gymnasium-1.0.0a1/gymnasium/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.047967 gymnasium-1.0.0a1/gymnasium/envs/box2d/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/box2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31524 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/box2d/bipedal_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/box2d/car_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29468 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/box2d/car_racing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32867 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/box2d/lunar_lander.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.047967 gymnasium-1.0.0a1/gymnasium/envs/classic_control/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/classic_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17322 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/classic_control/acrobot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.047967 gymnasium-1.0.0a1/gymnasium/envs/classic_control/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/classic_control/assets/clockwise.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21888 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/classic_control/cartpole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/classic_control/continuous_mountain_car.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/classic_control/mountain_car.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/classic_control/pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/classic_control/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/functional_jax_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.055967 gymnasium-1.0.0a1/gymnasium/envs/mujoco/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/ant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/ant_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/ant_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28443 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/ant_v5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.055967 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/ant.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/half_cheetah.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/hopper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/humanoid.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/humanoidstandup.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/inverted_double_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/inverted_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/point.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/pusher.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/reacher.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/swimmer.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/walker2d.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/walker2d_v5.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/half_cheetah.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/half_cheetah_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/half_cheetah_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15794 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/half_cheetah_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/hopper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/hopper_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/hopper_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19598 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/hopper_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/humanoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/humanoid_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/humanoid_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39634 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/humanoid_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/humanoidstandup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/humanoidstandup_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36157 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/humanoidstandup_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/inverted_double_pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/inverted_double_pendulum_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/inverted_double_pendulum_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/inverted_pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/inverted_pendulum_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/inverted_pendulum_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14493 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/mujoco_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/mujoco_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/pusher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/pusher_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15087 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/pusher_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/reacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/reacher_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12814 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/reacher_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/swimmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/swimmer_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/swimmer_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/swimmer_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/walker2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/walker2d_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/walker2d_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20321 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/mujoco/walker2d_v5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.055967 gymnasium-1.0.0a1/gymnasium/envs/phys2d/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/phys2d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.055967 gymnasium-1.0.0a1/gymnasium/envs/phys2d/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/phys2d/assets/clockwise.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/phys2d/cartpole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/phys2d/pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40630 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.059967 gymnasium-1.0.0a1/gymnasium/envs/tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17452 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/tabular/blackjack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13498 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/tabular/cliffwalking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.059967 gymnasium-1.0.0a1/gymnasium/envs/toy_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/blackjack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/cliffwalking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.059967 gymnasium-1.0.0a1/gymnasium/envs/toy_text/font/
+-rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/font/Minecraft.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    15857 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/frozen_lake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.071967 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C5.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C6.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C7.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C8.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C9.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/CA.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18635 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/CJ.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19498 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/CK.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18772 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/CQ.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/CT.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44172 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/Card.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D5.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D6.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D7.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D8.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D9.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/DA.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18468 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/DJ.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/DK.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18375 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/DQ.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/DT.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H5.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H6.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H7.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H8.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H9.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/HA.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18394 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/HJ.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19561 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/HK.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/HQ.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/HT.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S5.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S6.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S7.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S8.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S9.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/SA.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18175 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/SJ.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19256 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/SK.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/SQ.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/ST.png
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/cab_front.png
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/cab_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/cab_rear.png
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/cab_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/cookie.png
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/cracked_hole.png
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/elf_down.png
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/elf_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/elf_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/elf_up.png
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/goal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/gridworld_median_bottom.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/gridworld_median_horiz.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/gridworld_median_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/gridworld_median_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/gridworld_median_top.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/gridworld_median_vert.png
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/hole.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21682 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/hotel.png
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/ice.png
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/mountain_bg1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/mountain_bg2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/mountain_cliff.png
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/mountain_near-cliff1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/mountain_near-cliff2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/passenger.png
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/stool.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/taxi_background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19675 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/taxi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/envs/toy_text/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.075967 gymnasium-1.0.0a1/gymnasium/spaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13173 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/spaces/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/spaces/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/spaces/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/spaces/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/spaces/multi_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/spaces/multi_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/spaces/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/spaces/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/spaces/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/spaces/tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18925 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/spaces/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.075967 gymnasium-1.0.0a1/gymnasium/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/utils/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14120 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/utils/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/utils/env_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/utils/ezpickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16698 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/utils/passive_env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15855 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/utils/play.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/utils/record_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/utils/save_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/utils/seeding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/utils/step_api_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.079967 gymnasium-1.0.0a1/gymnasium/vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28269 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/vector/async_vector_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10218 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/vector/sync_vector_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.079967 gymnasium-1.0.0a1/gymnasium/vector/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/vector/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/vector/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/vector/utils/shared_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/vector/utils/space_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20193 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/vector/vector_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.079967 gymnasium-1.0.0a1/gymnasium/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/atari_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21533 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7181 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/jax_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/jax_to_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/numpy_to_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22146 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/stateful_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25234 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/stateful_observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/stateful_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/transform_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27536 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/transform_observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/transform_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.083967 gymnasium-1.0.0a1/gymnasium/wrappers/vector/
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/vector/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/vector/dict_info_to_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/vector/jax_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/vector/jax_to_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/vector/numpy_to_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/vector/stateful_observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/vector/stateful_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9591 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/vector/vectorize_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15104 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/vector/vectorize_observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/gymnasium/wrappers/vector/vectorize_reward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.083967 gymnasium-1.0.0a1/gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-02-13 16:56:00.000000 gymnasium-1.0.0a1/gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-02-13 16:56:00.000000 gymnasium-1.0.0a1/gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 16:56:00.000000 gymnasium-1.0.0a1/gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-02-13 16:56:00.000000 gymnasium-1.0.0a1/gymnasium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-13 16:56:00.000000 gymnasium-1.0.0a1/gymnasium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 16:56:00.087967 gymnasium-1.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 16:56:00.083967 gymnasium-1.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-02-13 16:55:49.000000 gymnasium-1.0.0a1/tests/testing_env.py
```

### Comparing `gymnasium-0.29.1/LICENSE` & `gymnasium-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/PKG-INFO` & `gymnasium-1.0.0a1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,18 @@
-Metadata-Version: 2.1
-Name: gymnasium
-Version: 0.29.1
-Summary: A standard API for reinforcement learning and a diverse set of reference environments (formerly Gym).
-Author-email: Farama Foundation <contact@farama.org>
-License: MIT License
-Project-URL: Homepage, https://farama.org
-Project-URL: Repository, https://github.com/Farama-Foundation/Gymnasium
-Project-URL: Documentation, https://gymnasium.farama.org
-Project-URL: Bug Report, https://github.com/Farama-Foundation/Gymnasium/issues
-Keywords: Reinforcement Learning,game,RL,AI,gymnasium
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: atari
-Provides-Extra: accept-rom-license
-Provides-Extra: box2d
-Provides-Extra: classic-control
-Provides-Extra: classic_control
-Provides-Extra: mujoco-py
-Provides-Extra: mujoco_py
-Provides-Extra: mujoco
-Provides-Extra: toy-text
-Provides-Extra: toy_text
-Provides-Extra: jax
-Provides-Extra: other
-Provides-Extra: all
-Provides-Extra: testing
-License-File: LICENSE
-
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8127025.svg)](https://doi.org/10.5281/zenodo.8127025)
-
+[![Python](https://img.shields.io/pypi/pyversions/gymnasium.svg)](https://badge.fury.io/py/gymnasium)
+[![PyPI](https://badge.fury.io/py/gymnasium.svg)](https://badge.fury.io/py/gymnasium)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8127025.svg)](https://doi.org/10.5281/zenodo.8127025)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/Farama-Foundation/Gymnasium/main/gymnasium-text.png" width="500px"/>
 </p>
 
-Gymnasium is an open source Python library for developing and comparing reinforcement learning algorithms by providing a standard API to communicate between learning algorithms and environments, as well as a standard set of environments compliant with that API. This is a fork of OpenAI's [Gym](https://github.com/openai/gym) library by it's maintainers (OpenAI handed over maintenance a few years ago to an outside team), and is where future maintenance will occur going forward.
+Gymnasium is an open source Python library for developing and comparing reinforcement learning algorithms by providing a standard API to communicate between learning algorithms and environments, as well as a standard set of environments compliant with that API. This is a fork of OpenAI's [Gym](https://github.com/openai/gym) library by its maintainers (OpenAI handed over maintenance a few years ago to an outside team), and is where future maintenance will occur going forward.
 
 The documentation website is at [gymnasium.farama.org](https://gymnasium.farama.org), and we have a public discord server (which we also use to coordinate development work) that you can join here: https://discord.gg/bnJ6kubTg6
 
 ## Environments
 
 Gymnasium includes the following families of environments along with a wide variety of third-party environments
 * [Classic Control](https://gymnasium.farama.org/environments/classic_control/) - These are classic reinforcement learning based on real-world problems and physics.
```

### Comparing `gymnasium-0.29.1/gymnasium/__init__.py` & `gymnasium-1.0.0a1/gymnasium/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 from gymnasium.envs.registration import (
     make,
     spec,
     register,
     registry,
     pprint_registry,
     make_vec,
+    VectorizeMode,
     register_envs,
 )
 
 # necessary for `envs.__init__` which registers all gymnasium environments and loads plugins
 from gymnasium import envs
-from gymnasium import spaces, utils, vector, wrappers, error, logger
-from gymnasium import experimental
+from gymnasium import spaces, utils, vector, wrappers, error, logger, functional
 
 
 __all__ = [
     # core classes
     "Env",
     "Wrapper",
     "ObservationWrapper",
@@ -35,27 +35,28 @@
     "Space",
     # registration
     "make",
     "make_vec",
     "spec",
     "register",
     "registry",
+    "VectorizeMode",
     "pprint_registry",
     "register_envs",
     # module folders
     "envs",
-    "experimental",
     "spaces",
     "utils",
     "vector",
     "wrappers",
     "error",
     "logger",
+    "functional",
 ]
-__version__ = "0.29.1"
+__version__ = "1.0.0a1"
 
 
 # Initializing pygame initializes audio connections through SDL. SDL uses alsa by default on all Linux systems
 # SDL connecting to alsa frequently create these giant lists of warnings every time you import an environment using
 #   pygame
 # DSP is far more benign (and should probably be the default in SDL anyways)
```

### Comparing `gymnasium-0.29.1/gymnasium/core.py` & `gymnasium-1.0.0a1/gymnasium/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,21 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import TYPE_CHECKING, Any, Generic, SupportsFloat, TypeVar
 
 import numpy as np
 
-from gymnasium import logger, spaces
+from gymnasium import spaces
 from gymnasium.utils import RecordConstructorArgs, seeding
 
 
 if TYPE_CHECKING:
     from gymnasium.envs.registration import EnvSpec, WrapperSpec
 
-
-__all__ = [
-    "Env",
-    "Wrapper",
-    "ObservationWrapper",
-    "RewardWrapper",
-    "ActionWrapper",
-    "ObsType",
-    "ActType",
-    "RenderFrame",
-    "WrapperObsType",
-    "WrapperActType",
-]
-
 ObsType = TypeVar("ObsType")
 ActType = TypeVar("ActType")
 RenderFrame = TypeVar("RenderFrame")
 
 
 class Env(Generic[ObsType, ActType]):
     r"""The main Gymnasium class for implementing Reinforcement Learning Agents environments.
@@ -47,32 +33,35 @@
     - :meth:`render` - Renders the environments to help visualise what the agent see, examples modes are "human", "rgb_array", "ansi" for text.
     - :meth:`close` - Closes the environment, important when external software is used, i.e. pygame for rendering, databases
 
     Environments have additional attributes for users to understand the implementation
 
     - :attr:`action_space` - The Space object corresponding to valid actions, all valid actions should be contained within the space.
     - :attr:`observation_space` - The Space object corresponding to valid observations, all valid observations should be contained within the space.
-    - :attr:`reward_range` - A tuple corresponding to the minimum and maximum possible rewards for an agent over an episode.
-      The default reward range is set to :math:`(-\infty,+\infty)`.
     - :attr:`spec` - An environment spec that contains the information used to initialize the environment from :meth:`gymnasium.make`
     - :attr:`metadata` - The metadata of the environment, i.e. render modes, render fps
     - :attr:`np_random` - The random number generator for the environment. This is automatically assigned during
-      ``super().reset(seed=seed)`` and when assessing ``self.np_random``.
+      ``super().reset(seed=seed)`` and when assessing :attr:`np_random`.
 
-    .. seealso:: For modifying or extending environments use the :py:class:`gymnasium.Wrapper` class
+    .. seealso:: For modifying or extending environments use the :class:`gymnasium.Wrapper` class
 
     Note:
         To get reproducible sampling of actions, a seed can be set with ``env.action_space.seed(123)``.
+
+    Note:
+        For strict type checking (e.g., mypy or pyright), :class:`Env` is a generic class with two parameterized types: ``ObsType`` and ``ActType``.
+        The ``ObsType`` and ``ActType`` are the expected types of the observations and actions used in :meth:`reset` and :meth:`step`.
+        The environment's :attr:`observation_space` and :attr:`action_space` should have type ``Space[ObsType]`` and ``Space[ActType]``,
+        see a space's implementation to find its parameterized type.
     """
 
     # Set this in SOME subclasses
     metadata: dict[str, Any] = {"render_modes": []}
     # define render_mode if your environment supports rendering
     render_mode: str | None = None
-    reward_range = (-float("inf"), float("inf"))
     spec: EnvSpec | None = None
 
     # Set these in ALL subclasses
     action_space: spaces.Space[ActType]
     observation_space: spaces.Space[ObsType]
 
     # Created
@@ -248,14 +237,18 @@
         # propagate exception
         return False
 
     def get_wrapper_attr(self, name: str) -> Any:
         """Gets the attribute `name` from the environment."""
         return getattr(self, name)
 
+    def set_wrapper_attr(self, name: str, value: Any):
+        """Sets the attribute `name` on the environment with `value`."""
+        setattr(self, name, value)
+
 
 WrapperObsType = TypeVar("WrapperObsType")
 WrapperActType = TypeVar("WrapperActType")
 
 
 class Wrapper(
     Env[WrapperObsType, WrapperActType],
@@ -278,64 +271,49 @@
     def __init__(self, env: Env[ObsType, ActType]):
         """Wraps an environment to allow a modular transformation of the :meth:`step` and :meth:`reset` methods.
 
         Args:
             env: The environment to wrap
         """
         self.env = env
+        assert isinstance(env, Env)
 
         self._action_space: spaces.Space[WrapperActType] | None = None
         self._observation_space: spaces.Space[WrapperObsType] | None = None
-        self._reward_range: tuple[SupportsFloat, SupportsFloat] | None = None
         self._metadata: dict[str, Any] | None = None
 
         self._cached_spec: EnvSpec | None = None
 
-    def __getattr__(self, name: str) -> Any:
-        """Returns an attribute with ``name``, unless ``name`` starts with an underscore.
-
-        Args:
-            name: The variable name
+    def step(
+        self, action: WrapperActType
+    ) -> tuple[WrapperObsType, SupportsFloat, bool, bool, dict[str, Any]]:
+        """Uses the :meth:`step` of the :attr:`env` that can be overwritten to change the returned data."""
+        return self.env.step(action)
 
-        Returns:
-            The value of the variable in the wrapper stack
+    def reset(
+        self, *, seed: int | None = None, options: dict[str, Any] | None = None
+    ) -> tuple[WrapperObsType, dict[str, Any]]:
+        """Uses the :meth:`reset` of the :attr:`env` that can be overwritten to change the returned data."""
+        return self.env.reset(seed=seed, options=options)
 
-        Warnings:
-            This feature is deprecated and removed in v1.0 and replaced with `env.get_attr(name})`
-        """
-        if name == "_np_random":
-            raise AttributeError(
-                "Can't access `_np_random` of a wrapper, use `self.unwrapped._np_random` or `self.np_random`."
-            )
-        elif name.startswith("_"):
-            raise AttributeError(f"accessing private attribute '{name}' is prohibited")
-        logger.warn(
-            f"env.{name} to get variables from other wrappers is deprecated and will be removed in v1.0, "
-            f"to get this variable you can do `env.unwrapped.{name}` for environment variables or `env.get_wrapper_attr('{name}')` that will search the reminding wrappers."
-        )
-        return getattr(self.env, name)
+    def render(self) -> RenderFrame | list[RenderFrame] | None:
+        """Uses the :meth:`render` of the :attr:`env` that can be overwritten to change the returned data."""
+        return self.env.render()
 
-    def get_wrapper_attr(self, name: str) -> Any:
-        """Gets an attribute from the wrapper and lower environments if `name` doesn't exist in this object.
+    def close(self):
+        """Closes the wrapper and :attr:`env`."""
+        return self.env.close()
 
-        Args:
-            name: The variable name to get
+    @property
+    def unwrapped(self) -> Env[ObsType, ActType]:
+        """Returns the base environment of the wrapper.
 
-        Returns:
-            The variable with name in wrapper or lower environments
+        This will be the bare :class:`gymnasium.Env` environment, underneath all layers of wrappers.
         """
-        if name in self.__dir__():  # todo change in v1.0.0 to `hasattr`
-            return getattr(self, name)
-        else:
-            try:
-                return self.env.get_wrapper_attr(name)
-            except AttributeError as e:
-                raise AttributeError(
-                    f"wrapper {self.class_name()} has no attribute {name!r}"
-                ) from e
+        return self.env.unwrapped
 
     @property
     def spec(self) -> EnvSpec | None:
         """Returns the :attr:`Env` :attr:`spec` attribute with the `WrapperSpec` if the wrapper inherits from `EzPickle`."""
         if self._cached_spec is not None:
             return self._cached_spec
 
@@ -372,14 +350,61 @@
 
         return WrapperSpec(
             name=cls.class_name(),
             entry_point=f"{cls.__module__}:{cls.__name__}",
             kwargs=kwargs,
         )
 
+    def get_wrapper_attr(self, name: str) -> Any:
+        """Gets an attribute from the wrapper and lower environments if `name` doesn't exist in this object.
+
+        Args:
+            name: The variable name to get
+
+        Returns:
+            The variable with name in wrapper or lower environments
+        """
+        if hasattr(self, name):
+            return getattr(self, name)
+        else:
+            try:
+                return self.env.get_wrapper_attr(name)
+            except AttributeError as e:
+                raise AttributeError(
+                    f"wrapper {self.class_name()} has no attribute {name!r}"
+                ) from e
+
+    def set_wrapper_attr(self, name: str, value: Any):
+        """Sets an attribute on this wrapper or lower environment if `name` is already defined.
+
+        Args:
+            name: The variable name
+            value: The new variable value
+        """
+        sub_env = self.env
+        attr_set = False
+
+        while attr_set is False and isinstance(sub_env, Wrapper):
+            if hasattr(sub_env, name):
+                setattr(sub_env, name, value)
+                attr_set = True
+            else:
+                sub_env = sub_env.env
+
+        if attr_set is False:
+            setattr(sub_env, name, value)
+
+    def __str__(self):
+        """Returns the wrapper name and the :attr:`env` representation string."""
+        return f"<{type(self).__name__}{self.env}>"
+
+    def __repr__(self):
+        """Returns the string representation of the wrapper."""
+        return str(self)
+
     @classmethod
     def class_name(cls) -> str:
         """Returns the class name of the wrapper."""
         return cls.__name__
 
     @property
     def action_space(
@@ -404,26 +429,14 @@
         return self._observation_space
 
     @observation_space.setter
     def observation_space(self, space: spaces.Space[WrapperObsType]):
         self._observation_space = space
 
     @property
-    def reward_range(self) -> tuple[SupportsFloat, SupportsFloat]:
-        """Return the :attr:`Env` :attr:`reward_range` unless overwritten then the wrapper :attr:`reward_range` is used."""
-        if self._reward_range is None:
-            return self.env.reward_range
-        logger.warn("The `reward_range` is deprecated and will be removed in v1.0")
-        return self._reward_range
-
-    @reward_range.setter
-    def reward_range(self, value: tuple[SupportsFloat, SupportsFloat]):
-        self._reward_range = value
-
-    @property
     def metadata(self) -> dict[str, Any]:
         """Returns the :attr:`Env` :attr:`metadata`."""
         if self._metadata is None:
             return self.env.metadata
         return self._metadata
 
     @metadata.setter
@@ -450,66 +463,31 @@
 
         It seems that @property overwrites the variable (`_np_random`) meaning that __getattr__ gets called with the missing variable.
         """
         raise AttributeError(
             "Can't access `_np_random` of a wrapper, use `.unwrapped._np_random` or `.np_random`."
         )
 
-    def step(
-        self, action: WrapperActType
-    ) -> tuple[WrapperObsType, SupportsFloat, bool, bool, dict[str, Any]]:
-        """Uses the :meth:`step` of the :attr:`env` that can be overwritten to change the returned data."""
-        return self.env.step(action)
-
-    def reset(
-        self, *, seed: int | None = None, options: dict[str, Any] | None = None
-    ) -> tuple[WrapperObsType, dict[str, Any]]:
-        """Uses the :meth:`reset` of the :attr:`env` that can be overwritten to change the returned data."""
-        return self.env.reset(seed=seed, options=options)
-
-    def render(self) -> RenderFrame | list[RenderFrame] | None:
-        """Uses the :meth:`render` of the :attr:`env` that can be overwritten to change the returned data."""
-        return self.env.render()
-
-    def close(self):
-        """Closes the wrapper and :attr:`env`."""
-        return self.env.close()
-
-    def __str__(self):
-        """Returns the wrapper name and the :attr:`env` representation string."""
-        return f"<{type(self).__name__}{self.env}>"
-
-    def __repr__(self):
-        """Returns the string representation of the wrapper."""
-        return str(self)
-
-    @property
-    def unwrapped(self) -> Env[ObsType, ActType]:
-        """Returns the base environment of the wrapper.
-
-        This will be the bare :class:`gymnasium.Env` environment, underneath all layers of wrappers.
-        """
-        return self.env.unwrapped
-
 
 class ObservationWrapper(Wrapper[WrapperObsType, ActType, ObsType, ActType]):
-    """Superclass of wrappers that can modify observations using :meth:`observation` for :meth:`reset` and :meth:`step`.
+    """Modify observations from :meth:`Env.reset` and :meth:`Env.step` using :meth:`observation` function.
 
     If you would like to apply a function to only the observation before
     passing it to the learning code, you can simply inherit from :class:`ObservationWrapper` and overwrite the method
     :meth:`observation` to implement that transformation. The transformation defined in that method must be
     reflected by the :attr:`env` observation space. Otherwise, you need to specify the new observation space of the
     wrapper by setting :attr:`self.observation_space` in the :meth:`__init__` method of your wrapper.
-
-    Among others, Gymnasium provides the observation wrapper :class:`TimeAwareObservation`, which adds information about the
-    index of the timestep to the observation.
     """
 
     def __init__(self, env: Env[ObsType, ActType]):
-        """Constructor for the observation wrapper."""
+        """Constructor for the observation wrapper.
+
+        Args:
+            env: Environment to be wrapped.
+        """
         Wrapper.__init__(self, env)
 
     def reset(
         self, *, seed: int | None = None, options: dict[str, Any] | None = None
     ) -> tuple[WrapperObsType, dict[str, Any]]:
         """Modifies the :attr:`env` after calling :meth:`reset`, returning a modified observation using :meth:`self.observation`."""
         obs, info = self.env.reset(seed=seed, options=options)
@@ -541,15 +519,19 @@
     passing it to learning code, you can simply inherit from :class:`RewardWrapper` and overwrite the method
     :meth:`reward` to implement that transformation.
     This transformation might change the :attr:`reward_range`; to specify the :attr:`reward_range` of your wrapper,
     you can simply define :attr:`self.reward_range` in :meth:`__init__`.
     """
 
     def __init__(self, env: Env[ObsType, ActType]):
-        """Constructor for the Reward wrapper."""
+        """Constructor for the Reward wrapper.
+
+        Args:
+            env: Environment to be wrapped.
+        """
         Wrapper.__init__(self, env)
 
     def step(
         self, action: ActType
     ) -> tuple[ObsType, SupportsFloat, bool, bool, dict[str, Any]]:
         """Modifies the :attr:`env` :meth:`step` reward using :meth:`self.reward`."""
         observation, reward, terminated, truncated, info = self.env.step(action)
@@ -564,38 +546,43 @@
         Returns:
             The modified `reward`
         """
         raise NotImplementedError
 
 
 class ActionWrapper(Wrapper[ObsType, WrapperActType, ObsType, ActType]):
-    """Superclass of wrappers that can modify the action before :meth:`env.step`.
+    """Superclass of wrappers that can modify the action before :meth:`step`.
 
     If you would like to apply a function to the action before passing it to the base environment,
     you can simply inherit from :class:`ActionWrapper` and overwrite the method :meth:`action` to implement
     that transformation. The transformation defined in that method must take values in the base environment’s
     action space. However, its domain might differ from the original action space.
-    In that case, you need to specify the new action space of the wrapper by setting :attr:`self.action_space` in
+    In that case, you need to specify the new action space of the wrapper by setting :attr:`action_space` in
     the :meth:`__init__` method of your wrapper.
 
-    Among others, Gymnasium provides the action wrappers :class:`ClipAction` and :class:`RescaleAction` for clipping and rescaling actions.
+    Among others, Gymnasium provides the action wrappers :class:`gymnasium.wrappers.ClipAction` and
+    :class:`gymnasium.wrappers.RescaleAction` for clipping and rescaling actions.
     """
 
     def __init__(self, env: Env[ObsType, ActType]):
-        """Constructor for the action wrapper."""
+        """Constructor for the action wrapper.
+
+        Args:
+            env: Environment to be wrapped.
+        """
         Wrapper.__init__(self, env)
 
     def step(
         self, action: WrapperActType
     ) -> tuple[ObsType, SupportsFloat, bool, bool, dict[str, Any]]:
         """Runs the :attr:`env` :meth:`env.step` using the modified ``action`` from :meth:`self.action`."""
         return self.env.step(self.action(action))
 
     def action(self, action: WrapperActType) -> ActType:
-        """Returns a modified action before :meth:`env.step` is called.
+        """Returns a modified action before :meth:`step` is called.
 
         Args:
             action: The original :meth:`step` actions
 
         Returns:
             The modified actions
         """
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/__init__.py` & `gymnasium-1.0.0a1/gymnasium/envs/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 """Registers the internal gym envs then loads the env plugins for module using the entry point."""
 from typing import Any
 
-from gymnasium.envs.registration import (
-    load_plugin_envs,
-    make,
-    pprint_registry,
-    register,
-    registry,
-    spec,
-)
+from gymnasium.envs.registration import make, pprint_registry, register, registry, spec
 
 
 # Classic
 # ----------------------------------------
 
 register(
     id="CartPole-v0",
@@ -164,87 +157,118 @@
 
 # Tabular
 # ----------------------------------------
 
 register(
     id="tabular/Blackjack-v0",
     entry_point="gymnasium.envs.tabular.blackjack:BlackJackJaxEnv",
-    kwargs={"sutton_and_barto": True, "natural": False},
 )
 
 register(
     id="tabular/CliffWalking-v0",
     entry_point="gymnasium.envs.tabular.cliffwalking:CliffWalkingJaxEnv",
 )
 
 
 # Mujoco
 # ----------------------------------------
 
-# 2D
+# manipulation
 
 register(
     id="Reacher-v2",
-    entry_point="gymnasium.envs.mujoco:ReacherEnv",
+    entry_point="gymnasium.envs.mujoco.reacher:ReacherEnv",
     max_episode_steps=50,
     reward_threshold=-3.75,
 )
 
 register(
     id="Reacher-v4",
     entry_point="gymnasium.envs.mujoco.reacher_v4:ReacherEnv",
     max_episode_steps=50,
     reward_threshold=-3.75,
 )
 
 register(
+    id="Reacher-v5",
+    entry_point="gymnasium.envs.mujoco.reacher_v5:ReacherEnv",
+    max_episode_steps=50,
+    reward_threshold=-3.75,
+)
+
+register(
     id="Pusher-v2",
-    entry_point="gymnasium.envs.mujoco:PusherEnv",
+    entry_point="gymnasium.envs.mujoco.pucher:PusherEnv",
     max_episode_steps=100,
     reward_threshold=0.0,
 )
 
 register(
     id="Pusher-v4",
     entry_point="gymnasium.envs.mujoco.pusher_v4:PusherEnv",
     max_episode_steps=100,
     reward_threshold=0.0,
 )
 
 register(
+    id="Pusher-v5",
+    entry_point="gymnasium.envs.mujoco.pusher_v5:PusherEnv",
+    max_episode_steps=100,
+    reward_threshold=0.0,
+)
+
+# balance
+
+register(
     id="InvertedPendulum-v2",
-    entry_point="gymnasium.envs.mujoco:InvertedPendulumEnv",
+    entry_point="gymnasium.envs.mujoco.inverted_pendulum:InvertedPendulumEnv",
     max_episode_steps=1000,
     reward_threshold=950.0,
 )
 
 register(
     id="InvertedPendulum-v4",
     entry_point="gymnasium.envs.mujoco.inverted_pendulum_v4:InvertedPendulumEnv",
     max_episode_steps=1000,
     reward_threshold=950.0,
 )
 
 register(
+    id="InvertedPendulum-v5",
+    entry_point="gymnasium.envs.mujoco.inverted_pendulum_v5:InvertedPendulumEnv",
+    max_episode_steps=1000,
+    reward_threshold=950.0,
+)
+
+register(
     id="InvertedDoublePendulum-v2",
-    entry_point="gymnasium.envs.mujoco:InvertedDoublePendulumEnv",
+    entry_point="gymnasium.envs.mujoco.inverted_double_pendulum:InvertedDoublePendulumEnv",
     max_episode_steps=1000,
     reward_threshold=9100.0,
 )
 
 register(
     id="InvertedDoublePendulum-v4",
     entry_point="gymnasium.envs.mujoco.inverted_double_pendulum_v4:InvertedDoublePendulumEnv",
     max_episode_steps=1000,
     reward_threshold=9100.0,
 )
 
 register(
+    id="InvertedDoublePendulum-v5",
+    entry_point="gymnasium.envs.mujoco.inverted_double_pendulum_v5:InvertedDoublePendulumEnv",
+    max_episode_steps=1000,
+    reward_threshold=9100.0,
+)
+
+# runners
+
+register(
     id="HalfCheetah-v2",
-    entry_point="gymnasium.envs.mujoco:HalfCheetahEnv",
+    entry_point="gymnasium.envs.mujoco.half_cheetah:HalfCheetahEnv",
     max_episode_steps=1000,
     reward_threshold=4800.0,
 )
 
 register(
     id="HalfCheetah-v3",
     entry_point="gymnasium.envs.mujoco.half_cheetah_v3:HalfCheetahEnv",
@@ -256,16 +280,23 @@
     id="HalfCheetah-v4",
     entry_point="gymnasium.envs.mujoco.half_cheetah_v4:HalfCheetahEnv",
     max_episode_steps=1000,
     reward_threshold=4800.0,
 )
 
 register(
+    id="HalfCheetah-v5",
+    entry_point="gymnasium.envs.mujoco.half_cheetah_v5:HalfCheetahEnv",
+    max_episode_steps=1000,
+    reward_threshold=4800.0,
+)
+
+register(
     id="Hopper-v2",
-    entry_point="gymnasium.envs.mujoco:HopperEnv",
+    entry_point="gymnasium.envs.mujoco.hopper:HopperEnv",
     max_episode_steps=1000,
     reward_threshold=3800.0,
 )
 
 register(
     id="Hopper-v3",
     entry_point="gymnasium.envs.mujoco.hopper_v3:HopperEnv",
@@ -277,16 +308,23 @@
     id="Hopper-v4",
     entry_point="gymnasium.envs.mujoco.hopper_v4:HopperEnv",
     max_episode_steps=1000,
     reward_threshold=3800.0,
 )
 
 register(
+    id="Hopper-v5",
+    entry_point="gymnasium.envs.mujoco.hopper_v5:HopperEnv",
+    max_episode_steps=1000,
+    reward_threshold=3800.0,
+)
+
+register(
     id="Swimmer-v2",
-    entry_point="gymnasium.envs.mujoco:SwimmerEnv",
+    entry_point="gymnasium.envs.mujoco.swimmer:SwimmerEnv",
     max_episode_steps=1000,
     reward_threshold=360.0,
 )
 
 register(
     id="Swimmer-v3",
     entry_point="gymnasium.envs.mujoco.swimmer_v3:SwimmerEnv",
@@ -298,17 +336,24 @@
     id="Swimmer-v4",
     entry_point="gymnasium.envs.mujoco.swimmer_v4:SwimmerEnv",
     max_episode_steps=1000,
     reward_threshold=360.0,
 )
 
 register(
+    id="Swimmer-v5",
+    entry_point="gymnasium.envs.mujoco.swimmer_v5:SwimmerEnv",
+    max_episode_steps=1000,
+    reward_threshold=360.0,
+)
+
+register(
     id="Walker2d-v2",
     max_episode_steps=1000,
-    entry_point="gymnasium.envs.mujoco:Walker2dEnv",
+    entry_point="gymnasium.envs.mujoco.walker2d:Walker2dEnv",
 )
 
 register(
     id="Walker2d-v3",
     max_episode_steps=1000,
     entry_point="gymnasium.envs.mujoco.walker2d_v3:Walker2dEnv",
 )
@@ -316,16 +361,22 @@
 register(
     id="Walker2d-v4",
     max_episode_steps=1000,
     entry_point="gymnasium.envs.mujoco.walker2d_v4:Walker2dEnv",
 )
 
 register(
+    id="Walker2d-v5",
+    max_episode_steps=1000,
+    entry_point="gymnasium.envs.mujoco.walker2d_v5:Walker2dEnv",
+)
+
+register(
     id="Ant-v2",
-    entry_point="gymnasium.envs.mujoco:AntEnv",
+    entry_point="gymnasium.envs.mujoco.ant:AntEnv",
     max_episode_steps=1000,
     reward_threshold=6000.0,
 )
 
 register(
     id="Ant-v3",
     entry_point="gymnasium.envs.mujoco.ant_v3:AntEnv",
@@ -337,16 +388,23 @@
     id="Ant-v4",
     entry_point="gymnasium.envs.mujoco.ant_v4:AntEnv",
     max_episode_steps=1000,
     reward_threshold=6000.0,
 )
 
 register(
+    id="Ant-v5",
+    entry_point="gymnasium.envs.mujoco.ant_v5:AntEnv",
+    max_episode_steps=1000,
+    reward_threshold=6000.0,
+)
+
+register(
     id="Humanoid-v2",
-    entry_point="gymnasium.envs.mujoco:HumanoidEnv",
+    entry_point="gymnasium.envs.mujoco.humanoid:HumanoidEnv",
     max_episode_steps=1000,
 )
 
 register(
     id="Humanoid-v3",
     entry_point="gymnasium.envs.mujoco.humanoid_v3:HumanoidEnv",
     max_episode_steps=1000,
@@ -355,33 +413,41 @@
 register(
     id="Humanoid-v4",
     entry_point="gymnasium.envs.mujoco.humanoid_v4:HumanoidEnv",
     max_episode_steps=1000,
 )
 
 register(
+    id="Humanoid-v5",
+    entry_point="gymnasium.envs.mujoco.humanoid_v5:HumanoidEnv",
+    max_episode_steps=1000,
+)
+
+register(
     id="HumanoidStandup-v2",
-    entry_point="gymnasium.envs.mujoco:HumanoidStandupEnv",
+    entry_point="gymnasium.envs.mujoco.humanoidstandup:HumanoidStandupEnv",
     max_episode_steps=1000,
 )
 
 register(
     id="HumanoidStandup-v4",
     entry_point="gymnasium.envs.mujoco.humanoidstandup_v4:HumanoidStandupEnv",
     max_episode_steps=1000,
 )
 
+register(
+    id="HumanoidStandup-v5",
+    entry_point="gymnasium.envs.mujoco.humanoidstandup_v5:HumanoidStandupEnv",
+    max_episode_steps=1000,
+)
+
 
 # --- For shimmy compatibility
 def _raise_shimmy_error(*args: Any, **kwargs: Any):
     raise ImportError(
         "To use the gym compatibility environments, run `pip install shimmy[gym-v21]` or `pip install shimmy[gym-v26]`"
     )
 
 
 # When installed, shimmy will re-register these environments with the correct entry_point
 register(id="GymV21Environment-v0", entry_point=_raise_shimmy_error)
 register(id="GymV26Environment-v0", entry_point=_raise_shimmy_error)
-
-
-# Hook to load plugins from entry points
-load_plugin_envs()
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/box2d/bipedal_walker.py` & `gymnasium-1.0.0a1/gymnasium/envs/box2d/bipedal_walker.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,19 +138,23 @@
     horizontal, and both legs in the same position with a slight knee angle.
 
     ## Episode Termination
     The episode will terminate if the hull gets in contact with the ground or
     if the walker exceeds the right end of the terrain length.
 
     ## Arguments
-    To use to the _hardcore_ environment, you need to specify the
-    `hardcore=True` argument like below:
+
+    To use the _hardcore_ environment, you need to specify the `hardcore=True`:
+
     ```python
-    import gymnasium as gym
-    env = gym.make("BipedalWalker-v3", hardcore=True)
+    >>> import gymnasium as gym
+    >>> env = gym.make("BipedalWalker-v3", hardcore=True, render_mode="rgb_array")
+    >>> env
+    <TimeLimit<OrderEnforcing<PassiveEnvChecker<BipedalWalker<BipedalWalker-v3>>>>>
+
     ```
 
     ## Version History
     - v3: Returns the closest lidar trace instead of furthest;
         faster video recording
     - v2: Count energy spent
     - v1: Legs now report contact with ground; motors have higher torque and
@@ -602,14 +606,15 @@
             reward = -100
             terminated = True
         if pos[0] > (TERRAIN_LENGTH - TERRAIN_GRASS) * TERRAIN_STEP:
             terminated = True
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return np.array(state, dtype=np.float32), reward, terminated, False, {}
 
     def render(self):
         if self.render_mode is None:
             assert self.spec is not None
             gym.logger.warn(
                 "You are calling render method without specifying any render mode. "
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/box2d/car_dynamics.py` & `gymnasium-1.0.0a1/gymnasium/envs/box2d/car_dynamics.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/box2d/car_racing.py` & `gymnasium-1.0.0a1/gymnasium/envs/box2d/car_racing.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     The easiest control task to learn from pixels - a top-down
     racing environment. The generated track is random every episode.
 
     Some indicators are shown at the bottom of the window along with the
     state RGB buffer. From left to right: true speed, four ABS sensors,
     steering wheel position, and gyroscope.
     To play yourself (it's rather fast for humans), type:
-    ```
+    ```shell
     python gymnasium/envs/box2d/car_racing.py
     ```
     Remember: it's a powerful rear-wheel drive car - don't press the accelerator
     and turn at the same time.
 
     ## Action Space
     If continuous there are 3 actions :
@@ -135,54 +135,62 @@
     - 4: brake
 
     ## Observation Space
 
     A top-down 96x96 RGB image of the car and race track.
 
     ## Rewards
-    The reward is -0.1 every frame and +1000/N for every track tile visited,
-    where N is the total number of tiles visited in the track. For example,
-    if you have finished in 732 frames, your reward is
-    1000 - 0.1*732 = 926.8 points.
+    The reward is -0.1 every frame and +1000/N for every track tile visited, where N is the total number of tiles
+     visited in the track. For example, if you have finished in 732 frames, your reward is 1000 - 0.1*732 = 926.8 points.
 
     ## Starting State
     The car starts at rest in the center of the road.
 
     ## Episode Termination
-    The episode finishes when all the tiles are visited. The car can also go
-    outside the playfield - that is, far off the track, in which case it will
-    receive -100 reward and die.
+    The episode finishes when all the tiles are visited. The car can also go outside the playfield -
+     that is, far off the track, in which case it will receive -100 reward and die.
 
     ## Arguments
-    `lap_complete_percent` dictates the percentage of tiles that must be visited by
-    the agent before a lap is considered complete.
 
-    Passing `domain_randomize=True` enables the domain randomized variant of the environment.
-    In this scenario, the background and track colours are different on every reset.
+    ```python
+    >>> import gymnasium as gym
+    >>> env = gym.make("CarRacing-v2", render_mode="rgb_array", lap_complete_percent=0.95, domain_randomize=False, continuous=False)
+    >>> env
+    <TimeLimit<OrderEnforcing<PassiveEnvChecker<CarRacing<CarRacing-v2>>>>>
+
+    ```
+
+    * `lap_complete_percent=0.95` dictates the percentage of tiles that must be visited by
+     the agent before a lap is considered complete.
 
-    Passing `continuous=False` converts the environment to use discrete action space.
-    The discrete action space has 5 actions: [do nothing, left, right, gas, brake].
+    * `domain_randomize=False` enables the domain randomized variant of the environment.
+     In this scenario, the background and track colours are different on every reset.
+
+    * `continuous=True` converts the environment to use discrete action space.
+     The discrete action space has 5 actions: [do nothing, left, right, gas, brake].
 
     ## Reset Arguments
+
     Passing the option `options["randomize"] = True` will change the current colour of the environment on demand.
     Correspondingly, passing the option `options["randomize"] = False` will not change the current colour of the environment.
     `domain_randomize` must be `True` on init for this argument to work.
-    Example usage:
+
     ```python
-    import gymnasium as gym
-    env = gym.make("CarRacing-v1", domain_randomize=True)
+    >>> import gymnasium as gym
+    >>> env = gym.make("CarRacing-v2", domain_randomize=True)
 
     # normal reset, this changes the colour scheme by default
-    env.reset()
+    >>> obs, _ = env.reset()
 
     # reset with colour scheme change
-    env.reset(options={"randomize": True})
+    >>> randomize_obs, _ = env.reset(options={"randomize": True})
 
     # reset with no colour scheme change
-    env.reset(options={"randomize": False})
+    >>> non_random_obs, _ = env.reset(options={"randomize": False})
+
     ```
 
     ## Version History
     - v1: Change track completion logic and add domain randomization (0.24.0)
     - v0: Original version
 
     ## References
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/box2d/lunar_lander.py` & `gymnasium-1.0.0a1/gymnasium/envs/box2d/lunar_lander.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     There are two environment versions: discrete or continuous.
     The landing pad is always at coordinates (0,0). The coordinates are the
     first two numbers in the state vector.
     Landing outside of the landing pad is possible. Fuel is infinite, so an agent
     can learn to fly and then land on its first attempt.
 
     To see a heuristic landing, run:
-    ```
+    ```shell
     python gymnasium/envs/box2d/lunar_lander.py
     ```
     <!-- To play yourself, run: -->
     <!-- python examples/agents/keyboard_agent.py LunarLander-v2 -->
 
     ## Action Space
     There are four discrete actions available:
@@ -141,82 +141,68 @@
     > When Box2D determines that a body (or group of bodies) has come to rest,
     > the body enters a sleep state which has very little CPU overhead. If a
     > body is awake and collides with a sleeping body, then the sleeping body
     > wakes up. Bodies will also wake up if a joint or contact attached to
     > them is destroyed.
 
     ## Arguments
-    To use to the _continuous_ environment, you need to specify the
-    `continuous=True` argument like below:
+
+    Lunar Lander has a large number of arguments
+
     ```python
-    import gymnasium as gym
-    env = gym.make(
-        "LunarLander-v2",
-        continuous: bool = False,
-        gravity: float = -10.0,
-        enable_wind: bool = False,
-        wind_power: float = 15.0,
-        turbulence_power: float = 1.5,
-    )
+    >>> import gymnasium as gym
+    >>> env = gym.make("LunarLander-v2", continuous=False, gravity=-10.0,
+    ...                enable_wind=False, wind_power=15.0, turbulence_power=1.5)
+    >>> env
+    <TimeLimit<OrderEnforcing<PassiveEnvChecker<LunarLander<LunarLander-v2>>>>>
+
     ```
-    If `continuous=True` is passed, continuous actions (corresponding to the throttle of the engines) will be used and the
-    action space will be `Box(-1, +1, (2,), dtype=np.float32)`.
-    The first coordinate of an action determines the throttle of the main engine, while the second
-    coordinate specifies the throttle of the lateral boosters.
-    Given an action `np.array([main, lateral])`, the main engine will be turned off completely if
-    `main < 0` and the throttle scales affinely from 50% to 100% for `0 <= main <= 1` (in particular, the
-    main engine doesn't work  with less than 50% power).
-    Similarly, if `-0.5 < lateral < 0.5`, the lateral boosters will not fire at all. If `lateral < -0.5`, the left
-    booster will fire, and if `lateral > 0.5`, the right booster will fire. Again, the throttle scales affinely
-    from 50% to 100% between -1 and -0.5 (and 0.5 and 1, respectively).
-
-    `gravity` dictates the gravitational constant, this is bounded to be within 0 and -12.
-
-    If `enable_wind=True` is passed, there will be wind effects applied to the lander.
-    The wind is generated using the function `tanh(sin(2 k (t+C)) + sin(pi k (t+C)))`.
-    `k` is set to 0.01.
-    `C` is sampled randomly between -9999 and 9999.
 
-    `wind_power` dictates the maximum magnitude of linear wind applied to the craft. The recommended value for `wind_power` is between 0.0 and 20.0.
-    `turbulence_power` dictates the maximum magnitude of rotational wind applied to the craft. The recommended value for `turbulence_power` is between 0.0 and 2.0.
+     * `continuous` determines if discrete or continuous actions (corresponding to the throttle of the engines) will be used with the
+     action space being `Discrete(4)` or `Box(-1, +1, (2,), dtype=np.float32)` respectively.
+     For continuous actions, the first coordinate of an action determines the throttle of the main engine, while the second
+     coordinate specifies the throttle of the lateral boosters. Given an action `np.array([main, lateral])`, the main
+     engine will be turned off completely if `main < 0` and the throttle scales affinely from 50% to 100% for
+     `0 <= main <= 1` (in particular, the main engine doesn't work  with less than 50% power).
+     Similarly, if `-0.5 < lateral < 0.5`, the lateral boosters will not fire at all. If `lateral < -0.5`, the left
+     booster will fire, and if `lateral > 0.5`, the right booster will fire. Again, the throttle scales affinely
+     from 50% to 100% between -1 and -0.5 (and 0.5 and 1, respectively).
+
+    * `gravity` dictates the gravitational constant, this is bounded to be within 0 and -12. Default is -10.0
+
+    * `enable_wind` determines if there will be wind effects applied to the lander. The wind is generated using
+     the function `tanh(sin(2 k (t+C)) + sin(pi k (t+C)))` where `k` is set to 0.01 and `C` is sampled randomly between -9999 and 9999.
+
+    * `wind_power` dictates the maximum magnitude of linear wind applied to the craft. The recommended value for
+     `wind_power` is between 0.0 and 20.0.
+
+    * `turbulence_power` dictates the maximum magnitude of rotational wind applied to the craft.
+     The recommended value for `turbulence_power` is between 0.0 and 2.0.
 
     ## Version History
     - v2: Count energy spent and in v0.24, added turbulence with wind power and turbulence_power parameters
-    - v1: Legs contact with ground added in state vector; contact with ground
-        give +10 reward points, and -10 if then lose contact; reward
-        renormalized to 200; harder initial random push.
+    - v1: Legs contact with ground added in state vector; contact with ground give +10 reward points,
+          and -10 if then lose contact; reward renormalized to 200; harder initial random push.
     - v0: Initial version
 
-
     ## Notes
 
     There are several unexpected bugs with the implementation of the environment.
 
-    1. The position of the side thursters on the body of the lander changes, depending on the orientation of the lander.
-    This in turn results in an orientation depentant torque being applied to the lander.
+    1. The position of the side thrusters on the body of the lander changes, depending on the orientation of the lander.
+    This in turn results in an orientation dependent torque being applied to the lander.
 
     2. The units of the state are not consistent. I.e.
     * The angular velocity is in units of 0.4 radians per second. In order to convert to radians per second, the value needs to be multiplied by a factor of 2.5.
 
     For the default values of VIEWPORT_W, VIEWPORT_H, SCALE, and FPS, the scale factors equal:
-    'x': 10
-    'y': 6.666
-    'vx': 5
-    'vy': 7.5
-    'angle': 1
-    'angular velocity': 2.5
+    'x': 10, 'y': 6.666, 'vx': 5, 'vy': 7.5, 'angle': 1, 'angular velocity': 2.5
 
     After the correction has been made, the units of the state are as follows:
-    'x': (units)
-    'y': (units)
-    'vx': (units/second)
-    'vy': (units/second)
-    'angle': (radians)
-    'angular velocity': (radians/second)
-
+    'x': (units), 'y': (units), 'vx': (units/second), 'vy': (units/second), 'angle': (radians), 'angular velocity': (radians/second)
 
     <!-- ## References -->
 
     ## Credits
     Created by Oleg Klimov
     """
 
@@ -669,14 +655,15 @@
             reward = -100
         if not self.lander.awake:
             terminated = True
             reward = +100
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return np.array(state, dtype=np.float32), reward, terminated, False, {}
 
     def render(self):
         if self.render_mode is None:
             assert self.spec is not None
             gym.logger.warn(
                 "You are calling render method without specifying any render mode. "
@@ -836,15 +823,15 @@
 
     if s[6] or s[7]:  # legs have contact
         angle_todo = 0
         hover_todo = (
             -(s[3]) * 0.5
         )  # override to reduce fall speed, that's all we need after contact
 
-    if env.continuous:
+    if env.unwrapped.continuous:
         a = np.array([hover_todo * 20 - 1, -angle_todo * 20])
         a = np.clip(a, -1, +1)
     else:
         a = 0
         if hover_todo > np.abs(angle_todo) and hover_todo > 0.05:
             a = 2
         elif angle_todo < -0.05:
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/classic_control/acrobot.py` & `gymnasium-1.0.0a1/gymnasium/envs/classic_control/acrobot.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,50 +92,51 @@
     The episode ends if one of the following occurs:
     1. Termination: The free end reaches the target height, which is constructed as:
     `-cos(theta1) - cos(theta2 + theta1) > 1.0`
     2. Truncation: Episode length is greater than 500 (200 for v0)
 
     ## Arguments
 
-    No additional arguments are currently supported during construction.
+    Acrobot only has `render_mode` as a keyword for `gymnasium.make`.
+    On reset, the `options` parameter allows the user to change the bounds used to determine the new random state.
 
     ```python
-    import gymnasium as gym
-    env = gym.make('Acrobot-v1')
-    ```
+    >>> import gymnasium as gym
+    >>> env = gym.make('Acrobot-v1', render_mode="rgb_array")
+    >>> env
+    <TimeLimit<OrderEnforcing<PassiveEnvChecker<AcrobotEnv<Acrobot-v1>>>>>
+    >>> env.reset(seed=123, options={"low": -0.2, "high": 0.2})  # default low=-0.1, high=0.1
+    (array([ 0.997341  ,  0.07287608,  0.9841162 , -0.17752565, -0.11185605,
+           -0.12625128], dtype=float32), {})
 
-    On reset, the `options` parameter allows the user to change the bounds used to determine
-    the new random state.
+    ```
 
     By default, the dynamics of the acrobot follow those described in Sutton and Barto's book
     [Reinforcement Learning: An Introduction](http://incompleteideas.net/book/11/node4.html).
     However, a `book_or_nips` parameter can be modified to change the pendulum dynamics to those described
     in the original [NeurIPS paper](https://papers.nips.cc/paper/1995/hash/8f1d43620bc6bb580df6e80b0dc05c48-Abstract.html).
 
     ```python
     # To change the dynamics as described above
     env.unwrapped.book_or_nips = 'nips'
     ```
 
     See the following note for details:
 
-    > The dynamics equations were missing some terms in the NIPS paper which
-            are present in the book. R. Sutton confirmed in personal correspondence
-            that the experimental results shown in the paper and the book were
-            generated with the equations shown in the book.
-            However, there is the option to run the domain with the paper equations
-            by setting `book_or_nips = 'nips'`
-
+    > The dynamics equations were missing some terms in the NIPS paper which are present in the book.
+      R. Sutton confirmed in personal correspondence that the experimental results shown in the paper and the book were
+      generated with the equations shown in the book. However, there is the option to run the domain with the paper equations
+      by setting `book_or_nips = 'nips'`
 
     ## Version History
 
     - v1: Maximum number of steps increased from 200 to 500. The observation space for v0 provided direct readings of
     `theta1` and `theta2` in radians, having a range of `[-pi, pi]`. The v1 observation space as described here provides the
     sine and cosine of each angle instead.
-    - v0: Initial versions release (1.0.0) (removed from gymnasium for v1)
+    - v0: Initial versions release
 
     ## References
     - Sutton, R. S. (1996). Generalization in Reinforcement Learning: Successful Examples Using Sparse Coarse Coding.
         In D. Touretzky, M. C. Mozer, & M. Hasselmo (Eds.), Advances in Neural Information Processing Systems (Vol. 8).
         MIT Press. https://proceedings.neurips.cc/paper/1995/file/8f1d43620bc6bb580df6e80b0dc05c48-Paper.pdf
     - Sutton, R. S., Barto, A. G. (2018 ). Reinforcement Learning: An Introduction. The MIT Press.
     """
@@ -221,15 +222,16 @@
         ns[3] = bound(ns[3], -self.MAX_VEL_2, self.MAX_VEL_2)
         self.state = ns
         terminated = self._terminal()
         reward = -1.0 if not terminated else 0.0
 
         if self.render_mode == "human":
             self.render()
-        return (self._get_ob(), reward, terminated, False, {})
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
+        return self._get_ob(), reward, terminated, False, {}
 
     def _get_ob(self):
         s = self.state
         assert s is not None, "Call reset before using AcrobotEnv object."
         return np.array(
             [cos(s[0]), sin(s[0]), cos(s[1]), sin(s[1]), s[2], s[3]], dtype=np.float32
         )
@@ -378,16 +380,16 @@
 
             pygame.display.quit()
             pygame.quit()
             self.isopen = False
 
 
 def wrap(x, m, M):
-    """Wraps ``x`` so m <= x <= M; but unlike ``bound()`` which
-    truncates, ``wrap()`` wraps x around the coordinate system defined by m,M.\n
+    """Wraps `x` so m <= x <= M; but unlike `bound()` which
+    truncates, `wrap()` wraps x around the coordinate system defined by m,M.\n
     For example, m = -180, M = 180 (degrees), x = 360 --> returns 0.
 
     Args:
         x: a scalar
         m: minimum possible value in range
         M: maximum possible value in range
 
@@ -434,15 +436,15 @@
 
         >>> dt = 0.0005
         >>> t = np.arange(0.0, 2.0, dt)
         >>> y0 = (1,2)
         >>> yout = rk4(derivs, y0, t)
 
     Args:
-        derivs: the derivative of the system and has the signature ``dy = derivs(yi)``
+        derivs: the derivative of the system and has the signature `dy = derivs(yi)`
         y0: initial state vector
         t: sample times
 
     Returns:
         yout: Runge-Kutta approximation of the ODE
     """
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/classic_control/assets/clockwise.png` & `gymnasium-1.0.0a1/gymnasium/envs/classic_control/assets/clockwise.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/classic_control/cartpole.py` & `gymnasium-1.0.0a1/gymnasium/envs/classic_control/cartpole.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import numpy as np
 
 import gymnasium as gym
 from gymnasium import logger, spaces
 from gymnasium.envs.classic_control import utils
 from gymnasium.error import DependencyNotInstalled
-from gymnasium.experimental.vector import VectorEnv
+from gymnasium.vector import VectorEnv
 from gymnasium.vector.utils import batch_space
 
 
 class CartPoleEnv(gym.Env[np.ndarray, Union[int, np.ndarray]]):
     """
     ## Description
 
@@ -70,21 +70,41 @@
 
     1. Termination: Pole Angle is greater than ±12°
     2. Termination: Cart Position is greater than ±2.4 (center of the cart reaches the edge of the display)
     3. Truncation: Episode length is greater than 500 (200 for v0)
 
     ## Arguments
 
+    Cartpole only has `render_mode` as a keyword for `gymnasium.make`.
+    On reset, the `options` parameter allows the user to change the bounds used to determine the new random state.
+
     ```python
-    import gymnasium as gym
-    gym.make('CartPole-v1')
+    >>> import gymnasium as gym
+    >>> env = gym.make("CartPole-v1", render_mode="rgb_array")
+    >>> env
+    <TimeLimit<OrderEnforcing<PassiveEnvChecker<CartPoleEnv<CartPole-v1>>>>>
+    >>> env.reset(seed=123, options={"low": -0.1, "high": 0.1})  # default low=-0.05, high=0.05
+    (array([ 0.03647037, -0.0892358 , -0.05592803, -0.06312564], dtype=float32), {})
+
     ```
 
-    On reset, the `options` parameter allows the user to change the bounds used to determine
-    the new random state.
+    ## Vectorized environment
+
+    To increase steps per seconds, users can use a custom vector environment or with an environment vectorizor.
+
+    ```python
+    >>> import gymnasium as gym
+    >>> envs = gym.make_vec("CartPole-v1", num_envs=3, vectorization_mode="vector_entry_point")
+    >>> envs
+    CartPoleVectorEnv(CartPole-v1, num_envs=3)
+    >>> envs = gym.make_vec("CartPole-v1", num_envs=3, vectorization_mode="sync")
+    >>> envs
+    SyncVectorEnv(CartPole-v1, num_envs=3)
+
+    ```
     """
 
     metadata = {
         "render_modes": ["human", "rgb_array"],
         "render_fps": 50,
     }
 
@@ -184,14 +204,15 @@
                     "True' -- any further steps are undefined behavior."
                 )
             self.steps_beyond_terminated += 1
             reward = 0.0
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return np.array(self.state, dtype=np.float32), reward, terminated, False, {}
 
     def reset(
         self,
         *,
         seed: Optional[int] = None,
         options: Optional[dict] = None,
@@ -324,26 +345,27 @@
 
     def __init__(
         self,
         num_envs: int = 2,
         max_episode_steps: int = 500,
         render_mode: Optional[str] = None,
     ):
-        super().__init__()
         self.num_envs = num_envs
+        self.max_episode_steps = max_episode_steps
+        self.render_mode = render_mode
+
         self.gravity = 9.8
         self.masscart = 1.0
         self.masspole = 0.1
         self.total_mass = self.masspole + self.masscart
         self.length = 0.5  # actually half the pole's length
         self.polemass_length = self.masspole * self.length
         self.force_mag = 10.0
         self.tau = 0.02  # seconds between state updates
         self.kinematics_integrator = "euler"
-        self.max_episode_steps = max_episode_steps
 
         self.steps = np.zeros(num_envs, dtype=np.int32)
 
         # Angle at which to fail the episode
         self.theta_threshold_radians = 12 * 2 * math.pi / 360
         self.x_threshold = 2.4
 
@@ -363,16 +385,14 @@
         self.high = 0.05
 
         self.single_action_space = spaces.Discrete(2)
         self.action_space = batch_space(self.single_action_space, num_envs)
         self.single_observation_space = spaces.Box(-high, high, dtype=np.float32)
         self.observation_space = batch_space(self.single_observation_space, num_envs)
 
-        self.render_mode = render_mode
-
         self.screen_width = 600
         self.screen_height = 400
         self.screens = None
         self.clocks = None
         self.isopen = True
         self.state = None
 
@@ -453,21 +473,23 @@
         self.low, self.high = utils.maybe_parse_reset_bounds(
             options, -0.05, 0.05  # default low
         )  # default high
         self.state = self.np_random.uniform(
             low=self.low, high=self.high, size=(4, self.num_envs)
         ).astype(np.float32)
         self.steps_beyond_terminated = None
+        self.steps = np.zeros(self.num_envs, dtype=np.int32)
 
         if self.render_mode == "human":
             self.render()
         return self.state.T, {}
 
     def render(self):
         if self.render_mode is None:
+            assert self.spec is not None
             gym.logger.warn(
                 "You are calling render method without specifying any render mode. "
                 "You can specify the render_mode at initialization, "
                 f'e.g. gym("{self.spec.id}", render_mode="rgb_array")'
             )
             return
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/classic_control/continuous_mountain_car.py` & `gymnasium-1.0.0a1/gymnasium/envs/classic_control/continuous_mountain_car.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,25 +87,30 @@
 
     The episode ends if either of the following happens:
     1. Termination: The position of the car is greater than or equal to 0.45 (the goal position on top of the right hill)
     2. Truncation: The length of the episode is 999.
 
     ## Arguments
 
+    Continuous Mountain Car has two parameters for `gymnasium.make` with `render_mode` and `goal_velocity`.
+    On reset, the `options` parameter allows the user to change the bounds used to determine the new random state.
+
     ```python
-    import gymnasium as gym
-    gym.make('MountainCarContinuous-v0')
-    ```
+    >>> import gymnasium as gym
+    >>> env = gym.make("MountainCarContinuous-v0", render_mode="rgb_array", goal_velocity=0.1)  # default goal_velocity=0
+    >>> env
+    <TimeLimit<OrderEnforcing<PassiveEnvChecker<Continuous_MountainCarEnv<MountainCarContinuous-v0>>>>>
+    >>> env.reset(seed=123, options={"low": -0.7, "high": -0.5})  # default low=-0.6, high=-0.4
+    (array([-0.5635296,  0.       ], dtype=float32), {})
 
-    On reset, the `options` parameter allows the user to change the bounds used to determine
-    the new random state.
+    ```
 
     ## Version History
 
-    * v0: Initial versions release (1.0.0)
+    * v0: Initial versions release
     """
 
     metadata = {
         "render_modes": ["human", "rgb_array"],
         "render_fps": 30,
     }
 
@@ -171,14 +176,15 @@
             reward = 100.0
         reward -= math.pow(action[0], 2) * 0.1
 
         self.state = np.array([position, velocity], dtype=np.float32)
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return self.state, reward, terminated, False, {}
 
     def reset(self, *, seed: Optional[int] = None, options: Optional[dict] = None):
         super().reset(seed=seed)
         # Note that if you use custom reset bounds, it may lead to out-of-bound
         # state/observations.
         low, high = utils.maybe_parse_reset_bounds(options, -0.6, -0.4)
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/classic_control/mountain_car.py` & `gymnasium-1.0.0a1/gymnasium/envs/classic_control/mountain_car.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,28 +76,32 @@
 
     ## Episode End
 
     The episode ends if either of the following happens:
     1. Termination: The position of the car is greater than or equal to 0.5 (the goal position on top of the right hill)
     2. Truncation: The length of the episode is 200.
 
-
     ## Arguments
 
+    Mountain Car has two parameters for `gymnasium.make` with `render_mode` and `goal_velocity`.
+    On reset, the `options` parameter allows the user to change the bounds used to determine the new random state.
+
     ```python
-    import gymnasium as gym
-    gym.make('MountainCar-v0')
-    ```
+    >>> import gymnasium as gym
+    >>> env = gym.make("MountainCar-v0", render_mode="rgb_array", goal_velocity=0.1)  # default goal_velocity=0
+    >>> env
+    <TimeLimit<OrderEnforcing<PassiveEnvChecker<MountainCarEnv<MountainCar-v0>>>>>
+    >>> env.reset(seed=123, options={"x_init": np.pi/2, "y_init": 0.5})  # default x_init=np.pi, y_init=1.0
+    (array([-0.46352962,  0.        ], dtype=float32), {})
 
-    On reset, the `options` parameter allows the user to change the bounds used to determine
-    the new random state.
+    ```
 
     ## Version History
 
-    * v0: Initial versions release (1.0.0)
+    * v0: Initial versions release
     """
 
     metadata = {
         "render_modes": ["human", "rgb_array"],
         "render_fps": 30,
     }
 
@@ -142,14 +146,15 @@
             position >= self.goal_position and velocity >= self.goal_velocity
         )
         reward = -1.0
 
         self.state = (position, velocity)
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return np.array(self.state, dtype=np.float32), reward, terminated, False, {}
 
     def reset(
         self,
         *,
         seed: Optional[int] = None,
         options: Optional[dict] = None,
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/classic_control/pendulum.py` & `gymnasium-1.0.0a1/gymnasium/envs/classic_control/pendulum.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,27 +25,26 @@
     into an upright position, with its center of gravity right above the fixed point.
 
     The diagram below specifies the coordinate system used for the implementation of the pendulum's
     dynamic equations.
 
     ![Pendulum Coordinate System](/_static/diagrams/pendulum.png)
 
-    -  `x-y`: cartesian coordinates of the pendulum's end in meters.
+    - `x-y`: cartesian coordinates of the pendulum's end in meters.
     - `theta` : angle in radians.
     - `tau`: torque in `N m`. Defined as positive _counter-clockwise_.
 
     ## Action Space
 
     The action is a `ndarray` with shape `(1,)` representing the torque applied to free end of the pendulum.
 
     | Num | Action | Min  | Max |
     |-----|--------|------|-----|
     | 0   | Torque | -2.0 | 2.0 |
 
-
     ## Observation Space
 
     The observation is a `ndarray` with shape `(3,)` representing the x-y coordinates of the pendulum's free
     end and its angular velocity.
 
     | Num | Observation      | Min  | Max |
     |-----|------------------|------|-----|
@@ -70,30 +69,35 @@
 
     ## Episode Truncation
 
     The episode truncates at 200 time steps.
 
     ## Arguments
 
-    - `g`: acceleration of gravity measured in *(m s<sup>-2</sup>)* used to calculate the pendulum dynamics.
-      The default value is g = 10.0 .
+    - `g`: .
+
+    Pendulum has two parameters for `gymnasium.make` with `render_mode` and `g` representing
+    the acceleration of gravity measured in *(m s<sup>-2</sup>)* used to calculate the pendulum dynamics.
+    The default value is `g = 10.0`.
+    On reset, the `options` parameter allows the user to change the bounds used to determine the new random state.
 
     ```python
-    import gymnasium as gym
-    gym.make('Pendulum-v1', g=9.81)
-    ```
+    >>> import gymnasium as gym
+    >>> env = gym.make("Pendulum-v1", render_mode="rgb_array", g=9.81)  # default g=10.0
+    >>> env
+    <TimeLimit<OrderEnforcing<PassiveEnvChecker<PendulumEnv<Pendulum-v1>>>>>
+    >>> env.reset(seed=123, options={"low": -0.7, "high": 0.5})  # default low=-0.6, high=-0.5
+    (array([ 0.4123625 ,  0.91101986, -0.89235795], dtype=float32), {})
 
-    On reset, the `options` parameter allows the user to change the bounds used to determine
-    the new random state.
+    ```
 
     ## Version History
 
     * v1: Simplify the math equations, no difference in behavior.
-    * v0: Initial versions release (1.0.0)
-
+    * v0: Initial versions release
     """
 
     metadata = {
         "render_modes": ["human", "rgb_array"],
         "render_fps": 30,
     }
 
@@ -137,14 +141,15 @@
         newthdot = np.clip(newthdot, -self.max_speed, self.max_speed)
         newth = th + newthdot * dt
 
         self.state = np.array([newth, newthdot])
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return self._get_obs(), -costs, False, False, {}
 
     def reset(self, *, seed: Optional[int] = None, options: Optional[dict] = None):
         super().reset(seed=seed)
         if options is None:
             high = np.array([DEFAULT_X, DEFAULT_Y])
         else:
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/classic_control/utils.py` & `gymnasium-1.0.0a1/gymnasium/envs/classic_control/utils.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/ant.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/ant.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,15 @@
             np.isfinite(state).all() and state[2] >= 0.2 and state[2] <= 1.0
         )
         terminated = not not_terminated
         ob = self._get_obs()
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return (
             ob,
             reward,
             terminated,
             False,
             dict(
                 reward_forward=forward_reward,
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/ant_v3.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/ant_v3.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,14 +143,15 @@
             "x_velocity": x_velocity,
             "y_velocity": y_velocity,
             "forward_reward": forward_reward,
         }
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return observation, reward, terminated, False, info
 
     def _get_obs(self):
         position = self.sim.data.qpos.flat.copy()
         velocity = self.sim.data.qvel.flat.copy()
         contact_force = self.contact_forces.flat.copy()
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/ant_v4.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/ant_v5.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,287 +1,329 @@
+__credits__ = ["Kallinteris-Andreas"]
+
+from typing import Dict, Tuple, Union
+
 import numpy as np
 
 from gymnasium import utils
 from gymnasium.envs.mujoco import MujocoEnv
 from gymnasium.spaces import Box
 
 
 DEFAULT_CAMERA_CONFIG = {
     "distance": 4.0,
 }
 
 
 class AntEnv(MujocoEnv, utils.EzPickle):
-    """
+    r"""
     ## Description
+    This environment is based on the one introduced by Schulman, Moritz, Levine, Jordan, and Abbeel in ["High-Dimensional Continuous Control Using Generalized Advantage Estimation"](https://arxiv.org/abs/1506.02438).
+    The ant is a 3D quadruped robot consisting of a torso (free rotational body) with four legs attached to it, where each leg has two body parts.
+    The goal is to coordinate the four legs to move in the forward (right) direction by applying torque to the eight hinges connecting the two body parts of each leg and the torso (nine body parts and eight hinges).
 
-    This environment is based on the environment introduced by Schulman,
-    Moritz, Levine, Jordan and Abbeel in ["High-Dimensional Continuous Control
-    Using Generalized Advantage Estimation"](https://arxiv.org/abs/1506.02438).
-    The ant is a 3D robot consisting of one torso (free rotational body) with
-    four legs attached to it with each leg having two body parts. The goal is to
-    coordinate the four legs to move in the forward (right) direction by applying
-    torques on the eight hinges connecting the two body parts of each leg and the torso
-    (nine body parts and eight hinges).
+    Note: Although the robot is called "Ant", it is actually 75cm tall and weighs 910.88g.
 
     ## Action Space
+    ```{figure} action_space_figures/ant.png
+    :name: ant
+    ```
+
     The action space is a `Box(-1, 1, (8,), float32)`. An action represents the torques applied at the hinge joints.
 
-    | Num | Action                                                            | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit         |
+    | Num | Action                                                            | Control Min | Control Max | Name (in corresponding XML file) | Joint | Type (Unit)  |
     | --- | ----------------------------------------------------------------- | ----------- | ----------- | -------------------------------- | ----- | ------------ |
     | 0   | Torque applied on the rotor between the torso and back right hip  | -1          | 1           | hip_4 (right_back_leg)           | hinge | torque (N m) |
     | 1   | Torque applied on the rotor between the back right two links      | -1          | 1           | angle_4 (right_back_leg)         | hinge | torque (N m) |
     | 2   | Torque applied on the rotor between the torso and front left hip  | -1          | 1           | hip_1 (front_left_leg)           | hinge | torque (N m) |
     | 3   | Torque applied on the rotor between the front left two links      | -1          | 1           | angle_1 (front_left_leg)         | hinge | torque (N m) |
     | 4   | Torque applied on the rotor between the torso and front right hip | -1          | 1           | hip_2 (front_right_leg)          | hinge | torque (N m) |
     | 5   | Torque applied on the rotor between the front right two links     | -1          | 1           | angle_2 (front_right_leg)        | hinge | torque (N m) |
     | 6   | Torque applied on the rotor between the torso and back left hip   | -1          | 1           | hip_3 (back_leg)                 | hinge | torque (N m) |
     | 7   | Torque applied on the rotor between the back left two links       | -1          | 1           | angle_3 (back_leg)               | hinge | torque (N m) |
 
+
     ## Observation Space
-    Observations consist of positional values of different body parts of the ant,
-    followed by the velocities of those individual parts (their derivatives) with all
-    the positions ordered before all the velocities.
-
-    By default, observations do not include the x- and y-coordinates of the ant's torso. These may
-    be included by passing `exclude_current_positions_from_observation=False` during construction.
-    In that case, the observation space will be a `Box(-Inf, Inf, (29,), float64)` where the first two observations
-    represent the x- and y- coordinates of the ant's torso.
-    Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the x- and y-coordinates
-    of the torso will be returned in `info` with keys `"x_position"` and `"y_position"`, respectively.
+    The observation space consists of the following parts (in order):
 
-    However, by default, observation Space is a `Box(-Inf, Inf, (27,), float64)` where the elements correspond to the following:
+    - *qpos (13 elements by default):* Position values of the robot's body parts.
+    - *qvel (14 elements):* The velocities of these individual body parts (their derivatives).
+    - *cfrc_ext (78 elements):* This is the center of mass based external forces on the body parts.
+    It has shape 13 * 6 (*nbody * 6*) and hence adds another 78 elements to the state space.
+    (external forces - force x, y, z and torque x, y, z)
+
+    By default, the observation does not include the x- and y-coordinates of the torso.
+    These can be included by passing `exclude_current_positions_from_observation=False` during construction.
+    In this case, the observation space will be a `Box(-Inf, Inf, (107,), float64)`, where the first two observations are the x- and y-coordinates of the torso.
+    Regardless of whether `exclude_current_positions_from_observation` is set to `True` or `False`, the x- and y-coordinates are returned in `info` with the keys `"x_position"` and `"y_position"`, respectively.
 
-    | Num | Observation                                                  | Min    | Max    | Name (in corresponding XML file)       | Joint | Unit                     |
+    By default, however, the observation space is a `Box(-Inf, Inf, (105,), float64)`, where the position and velocity elements are as follows:
+
+    | Num | Observation                                                  | Min    | Max    | Name (in corresponding XML file)       | Joint | Type (Unit)              |
     |-----|--------------------------------------------------------------|--------|--------|----------------------------------------|-------|--------------------------|
-    | 0   | z-coordinate of the torso (centre)                           | -Inf   | Inf    | torso                                  | free  | position (m)             |
-    | 1   | x-orientation of the torso (centre)                          | -Inf   | Inf    | torso                                  | free  | angle (rad)              |
-    | 2   | y-orientation of the torso (centre)                          | -Inf   | Inf    | torso                                  | free  | angle (rad)              |
-    | 3   | z-orientation of the torso (centre)                          | -Inf   | Inf    | torso                                  | free  | angle (rad)              |
-    | 4   | w-orientation of the torso (centre)                          | -Inf   | Inf    | torso                                  | free  | angle (rad)              |
+    | 0   | z-coordinate of the torso (centre)                           | -Inf   | Inf    | root                                   | free  | position (m)             |
+    | 1   | x-orientation of the torso (centre)                          | -Inf   | Inf    | root                                   | free  | angle (rad)              |
+    | 2   | y-orientation of the torso (centre)                          | -Inf   | Inf    | root                                   | free  | angle (rad)              |
+    | 3   | z-orientation of the torso (centre)                          | -Inf   | Inf    | root                                   | free  | angle (rad)              |
+    | 4   | w-orientation of the torso (centre)                          | -Inf   | Inf    | root                                   | free  | angle (rad)              |
     | 5   | angle between torso and first link on front left             | -Inf   | Inf    | hip_1 (front_left_leg)                 | hinge | angle (rad)              |
     | 6   | angle between the two links on the front left                | -Inf   | Inf    | ankle_1 (front_left_leg)               | hinge | angle (rad)              |
     | 7   | angle between torso and first link on front right            | -Inf   | Inf    | hip_2 (front_right_leg)                | hinge | angle (rad)              |
     | 8   | angle between the two links on the front right               | -Inf   | Inf    | ankle_2 (front_right_leg)              | hinge | angle (rad)              |
     | 9   | angle between torso and first link on back left              | -Inf   | Inf    | hip_3 (back_leg)                       | hinge | angle (rad)              |
     | 10  | angle between the two links on the back left                 | -Inf   | Inf    | ankle_3 (back_leg)                     | hinge | angle (rad)              |
     | 11  | angle between torso and first link on back right             | -Inf   | Inf    | hip_4 (right_back_leg)                 | hinge | angle (rad)              |
     | 12  | angle between the two links on the back right                | -Inf   | Inf    | ankle_4 (right_back_leg)               | hinge | angle (rad)              |
-    | 13  | x-coordinate velocity of the torso                           | -Inf   | Inf    | torso                                  | free  | velocity (m/s)           |
-    | 14  | y-coordinate velocity of the torso                           | -Inf   | Inf    | torso                                  | free  | velocity (m/s)           |
-    | 15  | z-coordinate velocity of the torso                           | -Inf   | Inf    | torso                                  | free  | velocity (m/s)           |
-    | 16  | x-coordinate angular velocity of the torso                   | -Inf   | Inf    | torso                                  | free  | angular velocity (rad/s) |
-    | 17  | y-coordinate angular velocity of the torso                   | -Inf   | Inf    | torso                                  | free  | angular velocity (rad/s) |
-    | 18  | z-coordinate angular velocity of the torso                   | -Inf   | Inf    | torso                                  | free  | angular velocity (rad/s) |
+    | 13  | x-coordinate velocity of the torso                           | -Inf   | Inf    | root                                   | free  | velocity (m/s)           |
+    | 14  | y-coordinate velocity of the torso                           | -Inf   | Inf    | root                                   | free  | velocity (m/s)           |
+    | 15  | z-coordinate velocity of the torso                           | -Inf   | Inf    | root                                   | free  | velocity (m/s)           |
+    | 16  | x-coordinate angular velocity of the torso                   | -Inf   | Inf    | root                                   | free  | angular velocity (rad/s) |
+    | 17  | y-coordinate angular velocity of the torso                   | -Inf   | Inf    | root                                   | free  | angular velocity (rad/s) |
+    | 18  | z-coordinate angular velocity of the torso                   | -Inf   | Inf    | root                                   | free  | angular velocity (rad/s) |
     | 19  | angular velocity of angle between torso and front left link  | -Inf   | Inf    | hip_1 (front_left_leg)                 | hinge | angle (rad)              |
     | 20  | angular velocity of the angle between front left links       | -Inf   | Inf    | ankle_1 (front_left_leg)               | hinge | angle (rad)              |
     | 21  | angular velocity of angle between torso and front right link | -Inf   | Inf    | hip_2 (front_right_leg)                | hinge | angle (rad)              |
     | 22  | angular velocity of the angle between front right links      | -Inf   | Inf    | ankle_2 (front_right_leg)              | hinge | angle (rad)              |
     | 23  | angular velocity of angle between torso and back left link   | -Inf   | Inf    | hip_3 (back_leg)                       | hinge | angle (rad)              |
     | 24  | angular velocity of the angle between back left links        | -Inf   | Inf    | ankle_3 (back_leg)                     | hinge | angle (rad)              |
     | 25  | angular velocity of angle between torso and back right link  | -Inf   | Inf    | hip_4 (right_back_leg)                 | hinge | angle (rad)              |
     | 26  | angular velocity of the angle between back right links       | -Inf   | Inf    | ankle_4 (right_back_leg)               | hinge | angle (rad)              |
-    | excluded | x-coordinate of the torso (centre)                      | -Inf   | Inf    | torso                                  | free  | position (m)             |
-    | excluded | y-coordinate of the torso (centre)                      | -Inf   | Inf    | torso                                  | free  | position (m)             |
+    | excluded | x-coordinate of the torso (centre)                      | -Inf   | Inf    | root                                   | free  | position (m)             |
+    | excluded | y-coordinate of the torso (centre)                      | -Inf   | Inf    | root                                   | free  | position (m)             |
+
+    The body parts are:
 
+    | body part                 | id (for `v2`, `v3`, `v4)` | id (for `v5`) |
+    |  -----------------------  |  ---   |  ---  |
+    | worldbody (note: all values are constant 0) | 0  |excluded|
+    | torso                     | 1  |0       |
+    | front_left_leg            | 2  |1       |
+    | aux_1 (front left leg)    | 3  |2       |
+    | ankle_1 (front left leg)  | 4  |3       |
+    | front_right_leg           | 5  |4       |
+    | aux_2 (front right leg)   | 6  |5       |
+    | ankle_2 (front right leg) | 7  |6       |
+    | back_leg (back left leg)  | 8  |7       |
+    | aux_3 (back left leg)     | 9  |8       |
+    | ankle_3 (back left leg)   | 10 |9       |
+    | right_back_leg            | 11 |10      |
+    | aux_4 (back right leg)    | 12 |11      |
+    | ankle_4 (back right leg)  | 13 |12      |
+
+    The (x,y,z) coordinates are translational DOFs, while the orientations are rotational DOFs expressed as quaternions.
+    One can read more about free joints in the [MuJoCo documentation](https://mujoco.readthedocs.io/en/latest/XMLreference.html).
+
+
+    **Note:**
+    When using Ant-v3 or earlier versions, problems have been reported when using a `mujoco-py` version > 2.0, resulting in  contact forces always being 0.
+    Therefore, it is recommended to use a `mujoco-py` version < 2.0 when using the Ant environment if you want to report results with contact forces (if contact forces are not used in your experiments, you can use version > 2.0).
 
-    If version < `v4` or `use_contact_forces` is `True` then the observation space is extended by 14*6 = 84 elements, which are contact forces
-    (external forces - force x, y, z and torque x, y, z) applied to the
-    center of mass of each of the body parts. The 14 body parts are:
-
-    | id (for `v2`, `v3`, `v4)` | body parts |
-    |  ---  |  ------------  |
-    | 0  | worldbody (note: forces are always full of zeros) |
-    | 1  | torso |
-    | 2  | front_left_leg |
-    | 3  | aux_1 (front left leg) |
-    | 4  | ankle_1 (front left leg) |
-    | 5  | front_right_leg |
-    | 6  | aux_2 (front right leg) |
-    | 7  | ankle_2 (front right leg) |
-    | 8  | back_leg (back left leg) |
-    | 9  | aux_3 (back left leg) |
-    | 10 | ankle_3 (back left leg) |
-    | 11 | right_back_leg |
-    | 12 | aux_4 (back right leg) |
-    | 13 | ankle_4 (back right leg) |
-
-
-    The (x,y,z) coordinates are translational DOFs while the orientations are rotational
-    DOFs expressed as quaternions. One can read more about free joints on the [Mujoco Documentation](https://mujoco.readthedocs.io/en/latest/XMLreference.html).
-
-
-    **Note:** Ant-v4 environment no longer has the following contact forces issue.
-    If using previous Humanoid versions from v4, there have been reported issues that using a Mujoco-Py version > 2.0 results
-    in the contact forces always being 0. As such we recommend to use a Mujoco-Py version < 2.0
-    when using the Ant environment if you would like to report results with contact forces (if
-    contact forces are not used in your experiments, you can use version > 2.0).
 
     ## Rewards
-    The reward consists of three parts:
-    - *healthy_reward*: Every timestep that the ant is healthy (see definition in section "Episode Termination"), it gets a reward of fixed value `healthy_reward`
-    - *forward_reward*: A reward of moving forward which is measured as
-    *(x-coordinate before action - x-coordinate after action)/dt*. *dt* is the time
-    between actions and is dependent on the `frame_skip` parameter (default is 5),
-    where the frametime is 0.01 - making the default *dt = 5 * 0.01 = 0.05*.
-    This reward would be positive if the ant moves forward (in positive x direction).
-    - *ctrl_cost*: A negative reward for penalising the ant if it takes actions
-    that are too large. It is measured as *`ctrl_cost_weight` * sum(action<sup>2</sup>)*
-    where *`ctr_cost_weight`* is a parameter set for the control and has a default value of 0.5.
-    - *contact_cost*: A negative reward for penalising the ant if the external contact
-    force is too large. It is calculated *`contact_cost_weight` * sum(clip(external contact
-    force to `contact_force_range`)<sup>2</sup>)*.
+    The total reward is ***reward*** *=* *healthy_reward + forward_reward - ctrl_cost - contact_cost*.
 
-    The total reward returned is ***reward*** *=* *healthy_reward + forward_reward - ctrl_cost*.
+    - *healthy_reward*:
+    Every timestep that the Ant is healthy (see definition in section "Episode End"),
+    it gets a reward of fixed value `healthy_reward` (default is $1$).
+    - *forward_reward*:
+    A reward for moving forward,
+    this reward would be positive if the Ant moves forward (in the positive $x$ direction / in the right direction).
+    $w_{forward} \times \frac{dx}{dt}$, where
+    $dx$ is the displacement of the `main_body` ($x_{after-action} - x_{before-action}$),
+    $dt$ is the time between actions, which depends on the `frame_skip` parameter (default is $5$),
+    and `frametime`, which is $0.01$ - so the default is $dt = 5 \times 0.01 = 0.05$,
+    $w_{forward}$ is the `forward_reward_weight` (default is $1$).
+    - *ctrl_cost*:
+    A negative reward to penalize the Ant for taking actions that are too large.
+    $w_{control} \times \|action\|_2^2$,
+    where $w_{control}$ is `ctrl_cost_weight` (default is $0.5$).
+    - *contact_cost*:
+    A negative reward to penalize the Ant if the external contact forces are too large.
+    $w_{contact} \times \|F_{contact}\|_2^2$, where
+    $w_{contact}$ is `contact_cost_weight` (default is $5\times10^{-4}$),
+    $F_{contact}$ are the external contact forces clipped by `contact_force_range` (see `cfrc_ext` section on Observation Space).
+
+    `info` contains the individual reward terms.
 
-    But if `use_contact_forces=True` or version < `v4`
-    The total reward returned is ***reward*** *=* *healthy_reward + forward_reward - ctrl_cost - contact_cost*.
+    But if `use_contact_forces=False` on `v4`
+    The total reward returned is ***reward*** *=* *healthy_reward + forward_reward - ctrl_cost*.
 
-    In either case `info` will also contain the individual reward terms.
 
     ## Starting State
-    All observations start in state
-    (0.0, 0.0,  0.75, 1.0, 0.0  ... 0.0) with a uniform noise in the range
-    of [-`reset_noise_scale`, `reset_noise_scale`] added to the positional values and standard normal noise
-    with mean 0 and standard deviation `reset_noise_scale` added to the velocity values for
-    stochasticity. Note that the initial z coordinate is intentionally selected
-    to be slightly high, thereby indicating a standing up ant. The initial orientation
-    is designed to make it face forward as well.
+    The initial position state is $[0.0, 0.0, 0.75, 1.0, 0.0, ... 0.0] + \mathcal{U}_{[-reset\_noise\_scale \times I_{15}, reset\_noise\_scale \times I_{15}]}$.
+    The initial velocity state is $\mathcal{N}(0_{14}, reset\_noise\_scale^2 \times I_{14})$.
 
-    ## Episode End
-    The ant is said to be unhealthy if any of the following happens:
+    where $\mathcal{N}$ is the multivariate normal distribution and $\mathcal{U}$ is the multivariate uniform continuous distribution.
 
-    1. Any of the state space values is no longer finite
-    2. The z-coordinate of the torso is **not** in the closed interval given by `healthy_z_range` (defaults to [0.2, 1.0])
+    Note that the z- and x-coordinates are non-zero so that the ant can immediately stand up and face forward (x-axis).
 
-    If `terminate_when_unhealthy=True` is passed during construction (which is the default),
-    the episode ends when any of the following happens:
 
-    1. Truncation: The episode duration reaches a 1000 timesteps
-    2. Termination: The ant is unhealthy
+    ## Episode End
+    ### Termination
+    If `terminate_when_unhealthy is True` (the default), the environment terminates when the Ant is unhealthy.
+    the Ant is unhealthy if any of the following happens:
 
-    If `terminate_when_unhealthy=False` is passed, the episode is ended only when 1000 timesteps are exceeded.
+    1. Any of the state space values is no longer finite.
+    2. The z-coordinate of the torso (the height) is **not** in the closed interval given by the `healthy_z_range` argument (default is $[0.2, 1.0]$).
 
-    ## Arguments
+    ### Truncation
+    The default duration of an episode is 1000 timesteps.
 
-    No additional arguments are currently supported in v2 and lower.
 
-    ```python
-    import gymnasium as gym
-    env = gym.make('Ant-v2')
-    ```
-
-    v3 and v4 take `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc.
+    ## Arguments
+    Ant provides a range of parameters to modify the observation space, reward function, initial state, and termination condition.
+    These parameters can be applied during `gymnasium.make` in the following way:
 
     ```python
     import gymnasium as gym
-    env = gym.make('Ant-v4', ctrl_cost_weight=0.1, ...)
+    env = gym.make('Ant-v5', ctrl_cost_weight=0.5, ...)
     ```
 
-    | Parameter               | Type       | Default      |Description                    |
-    |-------------------------|------------|--------------|-------------------------------|
-    | `xml_file`              | **str**    | `"ant.xml"`  | Path to a MuJoCo model |
-    | `ctrl_cost_weight`      | **float**  | `0.5`        | Weight for *ctrl_cost* term (see section on reward) |
-    | `use_contact_forces`    | **bool**  | `False`      | If true, it extends the observation space by adding contact forces (see `Observation Space` section) and includes contact_cost to the reward function (see `Rewards` section) |
-    | `contact_cost_weight`   | **float**  | `5e-4`       | Weight for *contact_cost* term (see section on reward) |
-    | `healthy_reward`        | **float**  | `1`          | Constant reward given if the ant is "healthy" after timestep |
-    | `terminate_when_unhealthy` | **bool**| `True`       | If true, issue a done signal if the z-coordinate of the torso is no longer in the `healthy_z_range` |
-    | `healthy_z_range`       | **tuple**  | `(0.2, 1)`   | The ant is considered healthy if the z-coordinate of the torso is in this range |
-    | `contact_force_range`   | **tuple**  | `(-1, 1)`    | Contact forces are clipped to this range in the computation of *contact_cost* |
-    | `reset_noise_scale`     | **float**  | `0.1`        | Scale of random perturbations of initial position and velocity (see section on Starting State) |
-    | `exclude_current_positions_from_observation`| **bool** | `True`| Whether or not to omit the x- and y-coordinates from observations. Excluding the position can serve as an inductive bias to induce position-agnostic behavior in policies |
+    | Parameter                                  | Type       | Default      |Description                    |
+    |--------------------------------------------|------------|--------------|-------------------------------|
+    |`xml_file`                                  | **str**    | `"ant.xml"`  | Path to a MuJoCo model                                                                                                                                                                                      |
+    |`forward_reward_weight`                     | **float**  | `1`          | Weight for _forward_reward_ term (see `Rewards` section)                                                                                                                                                    |
+    |`ctrl_cost_weight`                          | **float**  | `0.5`        | Weight for _ctrl_cost_ term (see `Rewards` section)                                                                                                                                                         |
+    |`contact_cost_weight`                       | **float**  | `5e-4`       | Weight for _contact_cost_ term (see `Rewards` section)                                                                                                                                                      |
+    |`healthy_reward`                            | **float**  | `1`          | Weight for _healthy_reward_ term (see `Rewards` section)                                                                                                                                                    |
+    |`main_body`                                 |**str\|int**| `1`("torso") | Name or ID of the body, whose displacement is used to calculate the *dx*/_forward_reward_ (useful for custom MuJoCo models) (see `Rewards` section)                                                         |
+    |`terminate_when_unhealthy`                  | **bool**   | `True`       | If `True`, issue a `terminated` signal is unhealthy (see `Episode End` section)                                                                                                                                |
+    |`healthy_z_range`                           | **tuple**  | `(0.2, 1)`   | The ant is considered healthy if the z-coordinate of the torso is in this range (see `Episode End` section)                                                                                                 |
+    |`contact_force_range`                       | **tuple**  | `(-1, 1)`    | Contact forces are clipped to this range in the computation of *contact_cost* (see `Rewards` section)                                                                                                       |
+    |`reset_noise_scale`                         | **float**  | `0.1`        | Scale of random perturbations of initial position and velocity (see `Starting State` section)                                                                                                               |
+    |`exclude_current_positions_from_observation`| **bool**   | `True`       | Whether or not to omit the x- and y-coordinates from observations. Excluding the position can serve as an inductive bias to induce position-agnostic behavior in policies (see `Observation State` section) |
+    |`include_cfrc_ext_in_observation`           | **bool**   | `True`       | Whether to include *cfrc_ext* elements in the observations (see `Observation State` section)                                                                                                                |
+    |`use_contact_forces` (`v4` only)            | **bool**   | `False`      | If `True`, it extends the observation space by adding contact forces (see `Observation Space` section) and includes contact_cost to the reward function (see `Rewards` section)                             |
 
     ## Version History
-    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3, also removed contact forces from the default observation space (new variable `use_contact_forces=True` can restore them)
-    * v3: Support for `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc. rgb rendering comes from tracking camera (so agent does not run away from screen)
-    * v2: All continuous control environments now use mujoco-py >= 1.50
+    * v5:
+        - Minimum `mujoco` version is now 2.3.3.
+        - Added support for fully custom/third party `mujoco` models using the `xml_file` argument (previously only a few changes could be made to the existing models).
+        - Added `default_camera_config` argument, a dictionary for setting the `mj_camera` properties, mainly useful for custom environments.
+        - Added `env.observation_structure`, a dictionary for specifying the observation space compose (e.g. `qpos`, `qvel`), useful for building tooling and wrappers for the MuJoCo environments.
+        - Return a non-empty `info` with `reset()`, previously an empty dictionary was returned, the new keys are the same state information as `step()`.
+        - Added `frame_skip` argument, used to configure the `dt` (duration of `step()`), default varies by environment check environment documentation pages.
+        - Fixed bug: `healthy_reward` was given on every step (even if the Ant is unhealthy), now it is only given when the Ant is healthy. The `info["reward_survive"]` is updated with this change (related [GitHub issue](https://github.com/Farama-Foundation/Gymnasium/issues/526)).
+        - The reward function now always includes `contact_cost`, before it was only included if `use_contact_forces=True` (can be set to `0` with `contact_cost_weight=0`).
+        - Excluded the `cfrc_ext` of `worldbody` from the observation space, as it was always 0 and thus provided no useful information to the agent, resulting in slightly faster training (related [GitHub issue](https://github.com/Farama-Foundation/Gymnasium/issues/204)).
+        - Added the `main_body` argument, which specifies the body used to compute the forward reward (mainly useful for custom MuJoCo models).
+        - Added the `forward_reward_weight` argument, which defaults to `1` (effectively the same behavior as in `v4`).
+        - Added the `include_cfrc_ext_in_observation` argument, previously in `v4` the inclusion of `cfrc_ext` observations was controlled by `use_contact_forces` which defaulted to `False`, while `include_cfrc_ext_in_observation` defaults to `True`.
+        - Removed the `use_contact_forces` argument (note: its functionality has been replaced by `include_cfrc_ext_in_observation` and `contact_cost_weight`) (related [GitHub issue](https://github.com/Farama-Foundation/Gymnasium/issues/214)).
+        - Fixed `info["reward_ctrl"]` sometimes containing `contact_cost` instead of `ctrl_cost`.
+        - Fixed `info["x_position"]` & `info["y_position"]` & `info["distance_from_origin"]` giving `xpos` instead of `qpos` observations (`xpos` observations are behind 1 `mj_step()` more [here](https://github.com/deepmind/mujoco/issues/889#issuecomment-1568896388)) (related [GitHub issue #1](https://github.com/Farama-Foundation/Gymnasium/issues/521) & [GitHub issue #2](https://github.com/Farama-Foundation/Gymnasium/issues/539)).
+        - Removed `info["forward_reward"]` as it is equivalent to `info["reward_forward"]`.
+    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3, also removed contact forces from the default observation space (new variable `use_contact_forces=True` can restore them).
+    * v3: Support for `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc. rgb rendering comes from tracking camera (so agent does not run away from screen).
+    * v2: All continuous control environments now use mujoco-py >= 1.50.
     * v1: max_time_steps raised to 1000 for robot based tasks. Added reward_threshold to environments.
-    * v0: Initial versions release (1.0.0)
+    * v0: Initial versions release
     """
 
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
-        "render_fps": 20,
     }
 
     def __init__(
         self,
-        xml_file="ant.xml",
-        ctrl_cost_weight=0.5,
-        use_contact_forces=False,
-        contact_cost_weight=5e-4,
-        healthy_reward=1.0,
-        terminate_when_unhealthy=True,
-        healthy_z_range=(0.2, 1.0),
-        contact_force_range=(-1.0, 1.0),
-        reset_noise_scale=0.1,
-        exclude_current_positions_from_observation=True,
+        xml_file: str = "ant.xml",
+        frame_skip: int = 5,
+        default_camera_config: Dict[str, Union[float, int]] = DEFAULT_CAMERA_CONFIG,
+        forward_reward_weight: float = 1,
+        ctrl_cost_weight: float = 0.5,
+        contact_cost_weight: float = 5e-4,
+        healthy_reward: float = 1.0,
+        main_body: Union[int, str] = 1,
+        terminate_when_unhealthy: bool = True,
+        healthy_z_range: Tuple[float, float] = (0.2, 1.0),
+        contact_force_range: Tuple[float, float] = (-1.0, 1.0),
+        reset_noise_scale: float = 0.1,
+        exclude_current_positions_from_observation: bool = True,
+        include_cfrc_ext_in_observation: bool = True,
         **kwargs,
     ):
         utils.EzPickle.__init__(
             self,
             xml_file,
+            frame_skip,
+            default_camera_config,
+            forward_reward_weight,
             ctrl_cost_weight,
-            use_contact_forces,
             contact_cost_weight,
             healthy_reward,
+            main_body,
             terminate_when_unhealthy,
             healthy_z_range,
             contact_force_range,
             reset_noise_scale,
             exclude_current_positions_from_observation,
+            include_cfrc_ext_in_observation,
             **kwargs,
         )
 
+        self._forward_reward_weight = forward_reward_weight
         self._ctrl_cost_weight = ctrl_cost_weight
         self._contact_cost_weight = contact_cost_weight
 
         self._healthy_reward = healthy_reward
         self._terminate_when_unhealthy = terminate_when_unhealthy
         self._healthy_z_range = healthy_z_range
 
         self._contact_force_range = contact_force_range
 
-        self._reset_noise_scale = reset_noise_scale
+        self._main_body = main_body
 
-        self._use_contact_forces = use_contact_forces
+        self._reset_noise_scale = reset_noise_scale
 
         self._exclude_current_positions_from_observation = (
             exclude_current_positions_from_observation
         )
-
-        obs_shape = 27
-        if not exclude_current_positions_from_observation:
-            obs_shape += 2
-        if use_contact_forces:
-            obs_shape += 84
-
-        observation_space = Box(
-            low=-np.inf, high=np.inf, shape=(obs_shape,), dtype=np.float64
-        )
+        self._include_cfrc_ext_in_observation = include_cfrc_ext_in_observation
 
         MujocoEnv.__init__(
             self,
             xml_file,
-            5,
-            observation_space=observation_space,
-            default_camera_config=DEFAULT_CAMERA_CONFIG,
+            frame_skip,
+            observation_space=None,  # needs to be defined after
+            default_camera_config=default_camera_config,
             **kwargs,
         )
 
+        self.metadata = {
+            "render_modes": [
+                "human",
+                "rgb_array",
+                "depth_array",
+            ],
+            "render_fps": int(np.round(1.0 / self.dt)),
+        }
+
+        obs_size = self.data.qpos.size + self.data.qvel.size
+        obs_size -= 2 * exclude_current_positions_from_observation
+        obs_size += self.data.cfrc_ext[1:].size * include_cfrc_ext_in_observation
+
+        self.observation_space = Box(
+            low=-np.inf, high=np.inf, shape=(obs_size,), dtype=np.float64
+        )
+
+        self.observation_structure = {
+            "skipped_qpos": 2 * exclude_current_positions_from_observation,
+            "qpos": self.data.qpos.size
+            - 2 * exclude_current_positions_from_observation,
+            "qvel": self.data.qvel.size,
+            "cfrc_ext": self.data.cfrc_ext[1:].size * include_cfrc_ext_in_observation,
+        }
+
     @property
     def healthy_reward(self):
-        return (
-            float(self.is_healthy or self._terminate_when_unhealthy)
-            * self._healthy_reward
-        )
+        return self.is_healthy * self._healthy_reward
 
     def control_cost(self, action):
         control_cost = self._ctrl_cost_weight * np.sum(np.square(action))
         return control_cost
 
     @property
     def contact_forces(self):
@@ -300,67 +342,68 @@
     @property
     def is_healthy(self):
         state = self.state_vector()
         min_z, max_z = self._healthy_z_range
         is_healthy = np.isfinite(state).all() and min_z <= state[2] <= max_z
         return is_healthy
 
-    @property
-    def terminated(self):
-        terminated = not self.is_healthy if self._terminate_when_unhealthy else False
-        return terminated
-
     def step(self, action):
-        xy_position_before = self.get_body_com("torso")[:2].copy()
+        xy_position_before = self.data.body(self._main_body).xpos[:2].copy()
         self.do_simulation(action, self.frame_skip)
-        xy_position_after = self.get_body_com("torso")[:2].copy()
+        xy_position_after = self.data.body(self._main_body).xpos[:2].copy()
 
         xy_velocity = (xy_position_after - xy_position_before) / self.dt
         x_velocity, y_velocity = xy_velocity
 
-        forward_reward = x_velocity
-        healthy_reward = self.healthy_reward
-
-        rewards = forward_reward + healthy_reward
-
-        costs = ctrl_cost = self.control_cost(action)
-
-        terminated = self.terminated
         observation = self._get_obs()
+        reward, reward_info = self._get_rew(x_velocity, action)
+        terminated = (not self.is_healthy) and self._terminate_when_unhealthy
         info = {
-            "reward_forward": forward_reward,
-            "reward_ctrl": -ctrl_cost,
-            "reward_survive": healthy_reward,
-            "x_position": xy_position_after[0],
-            "y_position": xy_position_after[1],
-            "distance_from_origin": np.linalg.norm(xy_position_after, ord=2),
+            "x_position": self.data.qpos[0],
+            "y_position": self.data.qpos[1],
+            "distance_from_origin": np.linalg.norm(self.data.qpos[0:2], ord=2),
             "x_velocity": x_velocity,
             "y_velocity": y_velocity,
-            "forward_reward": forward_reward,
+            **reward_info,
         }
-        if self._use_contact_forces:
-            contact_cost = self.contact_cost
-            costs += contact_cost
-            info["reward_ctrl"] = -contact_cost
-
-        reward = rewards - costs
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return observation, reward, terminated, False, info
 
+    def _get_rew(self, x_velocity: float, action):
+        forward_reward = x_velocity * self._forward_reward_weight
+        healthy_reward = self.healthy_reward
+        rewards = forward_reward + healthy_reward
+
+        ctrl_cost = self.control_cost(action)
+        contact_cost = self.contact_cost
+        costs = ctrl_cost + contact_cost
+
+        reward = rewards - costs
+
+        reward_info = {
+            "reward_forward": forward_reward,
+            "reward_ctrl": -ctrl_cost,
+            "reward_contact": -contact_cost,
+            "reward_survive": healthy_reward,
+        }
+
+        return reward, reward_info
+
     def _get_obs(self):
-        position = self.data.qpos.flat.copy()
-        velocity = self.data.qvel.flat.copy()
+        position = self.data.qpos.flatten()
+        velocity = self.data.qvel.flatten()
 
         if self._exclude_current_positions_from_observation:
             position = position[2:]
 
-        if self._use_contact_forces:
-            contact_force = self.contact_forces.flat.copy()
+        if self._include_cfrc_ext_in_observation:
+            contact_force = self.contact_forces[1:].flatten()
             return np.concatenate((position, velocity, contact_force))
         else:
             return np.concatenate((position, velocity))
 
     def reset_model(self):
         noise_low = -self._reset_noise_scale
         noise_high = self._reset_noise_scale
@@ -373,7 +416,14 @@
             + self._reset_noise_scale * self.np_random.standard_normal(self.model.nv)
         )
         self.set_state(qpos, qvel)
 
         observation = self._get_obs()
 
         return observation
+
+    def _get_reset_info(self):
+        return {
+            "x_position": self.data.qpos[0],
+            "y_position": self.data.qpos[1],
+            "distance_from_origin": np.linalg.norm(self.data.qpos[0:2], ord=2),
+        }
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/assets/ant.xml` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/ant.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/assets/half_cheetah.xml` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/half_cheetah.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/assets/hopper.xml` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/hopper.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/assets/humanoid.xml` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/humanoid.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/assets/humanoidstandup.xml` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/humanoidstandup.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/assets/inverted_double_pendulum.xml` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/inverted_double_pendulum.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/assets/inverted_pendulum.xml` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/inverted_pendulum.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/assets/point.xml` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/point.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/assets/pusher.xml` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/pusher.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/assets/reacher.xml` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/reacher.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/assets/swimmer.xml` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/swimmer.xml`

 * *Files 2% similar despite different names*

#### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/assets/swimmer.xml` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/swimmer.xml`

```diff
@@ -1,25 +1,25 @@
 <?xml version="1.0" encoding="utf-8"?>
 <mujoco model="swimmer">
   <compiler angle="degree" coordinate="local" inertiafromgeom="true"/>
-  <option collision="predefined" density="4000" integrator="RK4" timestep="0.01" viscosity="0.1"/>
+  <option density="4000" integrator="RK4" timestep="0.01" viscosity="0.1"/>
   <default>
-    <geom conaffinity="1" condim="1" contype="1" material="geom" rgba="0.8 0.6 .4 1"/>
+    <geom conaffinity="0" condim="1" contype="0" material="geom" rgba="0.8 0.6 .4 1"/>
     <joint armature="0.1"/>
   </default>
   <asset>
     <texture builtin="gradient" height="100" rgb1="1 1 1" rgb2="0 0 0" type="skybox" width="100"/>
     <texture builtin="flat" height="1278" mark="cross" markrgb="1 1 1" name="texgeom" random="0.01" rgb1="0.8 0.6 0.4" rgb2="0.8 0.6 0.4" type="cube" width="127"/>
     <texture builtin="checker" height="100" name="texplane" rgb1="0 0 0" rgb2="0.8 0.8 0.8" type="2d" width="100"/>
     <material name="MatPlane" reflectance="0.5" shininess="1" specular="1" texrepeat="30 30" texture="texplane"/>
     <material name="geom" texture="texgeom" texuniform="true"/>
   </asset>
   <worldbody>
     <light cutoff="100" diffuse="1 1 1" dir="-0 0 -1.3" directional="true" exponent="1" pos="0 0 1.3" specular=".1 .1 .1"/>
-    <geom conaffinity="1" condim="3" material="MatPlane" name="floor" pos="0 0 -0.1" rgba="0.8 0.9 0.8 1" size="40 40 0.1" type="plane"/>
+    <geom condim="3" material="MatPlane" name="floor" pos="0 0 -0.1" rgba="0.8 0.9 0.8 1" size="40 40 0.1" type="plane"/>
     <!--  ================= SWIMMER ================= /-->
     <body name="torso" pos="0 0 0">
       <camera name="track" mode="trackcom" pos="0 -3 3" xyaxes="1 0 0 0 1 1"/>
       <geom density="1000" fromto="1.5 0 0 0.5 0 0" size="0.1" type="capsule"/>
       <joint axis="1 0 0" name="slider1" pos="0 0 0" type="slide"/>
       <joint axis="0 1 0" name="slider2" pos="0 0 0" type="slide"/>
       <joint axis="0 0 1" name="free_body_rot" pos="0 0 0" type="hinge"/>
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/assets/walker2d.xml` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/assets/walker2d.xml`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/half_cheetah.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/half_cheetah.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         reward_ctrl = -0.1 * np.square(action).sum()
         reward_run = (xposafter - xposbefore) / self.dt
         reward = reward_ctrl + reward_run
         terminated = False
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return (
             ob,
             reward,
             terminated,
             False,
             dict(reward_run=reward_run, reward_ctrl=reward_ctrl),
         )
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/half_cheetah_v3.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/half_cheetah_v3.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,15 @@
             "x_velocity": x_velocity,
             "reward_run": forward_reward,
             "reward_ctrl": -ctrl_cost,
         }
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return observation, reward, terminated, False, info
 
     def _get_obs(self):
         position = self.sim.data.qpos.flat.copy()
         velocity = self.sim.data.qvel.flat.copy()
 
         if self._exclude_current_positions_from_observation:
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/half_cheetah_v4.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/half_cheetah_v5.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,228 +1,261 @@
-__credits__ = ["Rushiv Arora"]
+__credits__ = ["Kallinteris-Andreas", "Rushiv Arora"]
+
+from typing import Dict, Union
 
 import numpy as np
 
 from gymnasium import utils
 from gymnasium.envs.mujoco import MujocoEnv
 from gymnasium.spaces import Box
 
 
 DEFAULT_CAMERA_CONFIG = {
     "distance": 4.0,
 }
 
 
 class HalfCheetahEnv(MujocoEnv, utils.EzPickle):
-    """
+    r"""
     ## Description
+    This environment is based on the work of P. Wawrzyński in ["A Cat-Like Robot Real-Time Learning to Run"](http://staff.elka.pw.edu.pl/~pwawrzyn/pub-s/0812_LSCLRR.pdf).
+    The HalfCheetah is a 2-dimensional robot consisting of 9 body parts and 8 joints connecting them (including two paws).
+    The goal is to apply torque to the joints to make the cheetah run forward (right) as fast as possible, with a positive reward based on the distance moved forward and a negative reward for moving backward.
+    The cheetah's torso and head are fixed, and torque can only be applied to the other 6 joints over the front and back thighs (which connect to the torso), the shins (which connect to the thighs), and the feet (which connect to the shins).
 
-    This environment is based on the work by P. Wawrzyński in
-    ["A Cat-Like Robot Real-Time Learning to Run"](http://staff.elka.pw.edu.pl/~pwawrzyn/pub-s/0812_LSCLRR.pdf).
-    The HalfCheetah is a 2-dimensional robot consisting of 9 body parts and 8
-    joints connecting them (including two paws). The goal is to apply a torque
-    on the joints to make the cheetah run forward (right) as fast as possible,
-    with a positive reward allocated based on the distance moved forward and a
-    negative reward allocated for moving backward. The torso and head of the
-    cheetah are fixed, and the torque can only be applied on the other 6 joints
-    over the front and back thighs (connecting to the torso), shins
-    (connecting to the thighs) and feet (connecting to the shins).
 
     ## Action Space
+    ```{figure} action_space_figures/half_cheetah.png
+    :name: half_cheetah
+    ```
+
     The action space is a `Box(-1, 1, (6,), float32)`. An action represents the torques applied at the hinge joints.
 
-    | Num | Action                                  | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit         |
+    | Num | Action                                  | Control Min | Control Max | Name (in corresponding XML file) | Joint | Type (Unit)  |
     | --- | --------------------------------------- | ----------- | ----------- | -------------------------------- | ----- | ------------ |
     | 0   | Torque applied on the back thigh rotor  | -1          | 1           | bthigh                           | hinge | torque (N m) |
     | 1   | Torque applied on the back shin rotor   | -1          | 1           | bshin                            | hinge | torque (N m) |
     | 2   | Torque applied on the back foot rotor   | -1          | 1           | bfoot                            | hinge | torque (N m) |
     | 3   | Torque applied on the front thigh rotor | -1          | 1           | fthigh                           | hinge | torque (N m) |
     | 4   | Torque applied on the front shin rotor  | -1          | 1           | fshin                            | hinge | torque (N m) |
     | 5   | Torque applied on the front foot rotor  | -1          | 1           | ffoot                            | hinge | torque (N m) |
 
 
     ## Observation Space
-    Observations consist of positional values of different body parts of the
-    cheetah, followed by the velocities of those individual parts (their derivatives) with all the positions ordered before all the velocities.
+    The observation space consists of the following parts (in order):
+
+    - *qpos (8 elements by default):* Position values of the robot's body parts.
+    - *qvel (9 elements):* The velocities of these individual body parts (their derivatives).
+
+    By default, the observation does not include the robot's x-coordinate (`rootx`).
+    This can be included by passing `exclude_current_positions_from_observation=False` during construction.
+    In this case, the observation space will be a `Box(-Inf, Inf, (18,), float64)`, where the first observation element is the x-coordinate of the robot.
+    Regardless of whether `exclude_current_positions_from_observation` is set to `True` or `False`, the x- and y-coordinates are returned in `info` with the keys `"x_position"` and `"y_position"`, respectively.
+
+    By default, however, the observation space is a `Box(-Inf, Inf, (17,), float64)` where the elements are as follows:
+
+
+    | Num | Observation                                 | Min  | Max | Name (in corresponding XML file) | Joint | Type (Unit)              |
+    | --- | ------------------------------------------- | ---- | --- | -------------------------------- | ----- | ------------------------ |
+    | 0   | z-coordinate of the front tip               | -Inf | Inf | rootz                            | slide | position (m)             |
+    | 1   | angle of the front tip                      | -Inf | Inf | rooty                            | hinge | angle (rad)              |
+    | 2   | angle of the back thigh                     | -Inf | Inf | bthigh                           | hinge | angle (rad)              |
+    | 3   | angle of the back shin                      | -Inf | Inf | bshin                            | hinge | angle (rad)              |
+    | 4   | angle of the back foot                      | -Inf | Inf | bfoot                            | hinge | angle (rad)              |
+    | 5   | angle of the front thigh                    | -Inf | Inf | fthigh                           | hinge | angle (rad)              |
+    | 6   | angle of the front shin                     | -Inf | Inf | fshin                            | hinge | angle (rad)              |
+    | 7   | angle of the front foot                     | -Inf | Inf | ffoot                            | hinge | angle (rad)              |
+    | 8   | velocity of the x-coordinate of front tip   | -Inf | Inf | rootx                            | slide | velocity (m/s)           |
+    | 9   | velocity of the z-coordinate of front tip   | -Inf | Inf | rootz                            | slide | velocity (m/s)           |
+    | 10  | angular velocity of the front tip           | -Inf | Inf | rooty                            | hinge | angular velocity (rad/s) |
+    | 11  | angular velocity of the back thigh          | -Inf | Inf | bthigh                           | hinge | angular velocity (rad/s) |
+    | 12  | angular velocity of the back shin           | -Inf | Inf | bshin                            | hinge | angular velocity (rad/s) |
+    | 13  | angular velocity of the back foot           | -Inf | Inf | bfoot                            | hinge | angular velocity (rad/s) |
+    | 14  | angular velocity of the front thigh         | -Inf | Inf | fthigh                           | hinge | angular velocity (rad/s) |
+    | 15  | angular velocity of the front shin          | -Inf | Inf | fshin                            | hinge | angular velocity (rad/s) |
+    | 16  | angular velocity of the front foot          | -Inf | Inf | ffoot                            | hinge | angular velocity (rad/s) |
+    | excluded | x-coordinate of the front tip          | -Inf | Inf | rootx                            | slide | position (m)             |
 
-    By default, observations do not include the cheetah's `rootx`. It may
-    be included by passing `exclude_current_positions_from_observation=False` during construction.
-    In that case, the observation space will be a `Box(-Inf, Inf, (18,), float64)` where the first element
-    represents the `rootx`.
-    Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the
-    will be returned in `info` with key `"x_position"`.
-
-    However, by default, the observation is a `Box(-Inf, Inf, (17,), float64)` where the elements correspond to the following:
-
-    | Num | Observation                          | Min  | Max | Name (in corresponding XML file) | Joint | Unit                     |
-    | --- | ------------------------------------ | ---- | --- | -------------------------------- | ----- | ------------------------ |
-    | 0   | z-coordinate of the front tip        | -Inf | Inf | rootz                            | slide | position (m)             |
-    | 1   | angle of the front tip               | -Inf | Inf | rooty                            | hinge | angle (rad)              |
-    | 2   | angle of the second rotor            | -Inf | Inf | bthigh                           | hinge | angle (rad)              |
-    | 3   | angle of the second rotor            | -Inf | Inf | bshin                            | hinge | angle (rad)              |
-    | 4   | velocity of the tip along the x-axis | -Inf | Inf | bfoot                            | hinge | angle (rad)              |
-    | 5   | velocity of the tip along the y-axis | -Inf | Inf | fthigh                           | hinge | angle (rad)              |
-    | 6   | angular velocity of front tip        | -Inf | Inf | fshin                            | hinge | angle (rad)              |
-    | 7   | angular velocity of second rotor     | -Inf | Inf | ffoot                            | hinge | angle (rad)              |
-    | 8   | x-coordinate of the front tip        | -Inf | Inf | rootx                            | slide | velocity (m/s)           |
-    | 9   | y-coordinate of the front tip        | -Inf | Inf | rootz                            | slide | velocity (m/s)           |
-    | 10  | angle of the front tip               | -Inf | Inf | rooty                            | hinge | angular velocity (rad/s) |
-    | 11  | angle of the second rotor            | -Inf | Inf | bthigh                           | hinge | angular velocity (rad/s) |
-    | 12  | angle of the second rotor            | -Inf | Inf | bshin                            | hinge | angular velocity (rad/s) |
-    | 13  | velocity of the tip along the x-axis | -Inf | Inf | bfoot                            | hinge | angular velocity (rad/s) |
-    | 14  | velocity of the tip along the y-axis | -Inf | Inf | fthigh                           | hinge | angular velocity (rad/s) |
-    | 15  | angular velocity of front tip        | -Inf | Inf | fshin                            | hinge | angular velocity (rad/s) |
-    | 16  | angular velocity of second rotor     | -Inf | Inf | ffoot                            | hinge | angular velocity (rad/s) |
-    | excluded |  x-coordinate of the front tip  | -Inf | Inf | rootx                            | slide | position (m)             |
 
     ## Rewards
-    The reward consists of two parts:
-    - *forward_reward*: A reward of moving forward which is measured
-    as *`forward_reward_weight` * (x-coordinate before action - x-coordinate after action)/dt*. *dt* is
-    the time between actions and is dependent on the frame_skip parameter
-    (fixed to 5), where the frametime is 0.01 - making the
-    default *dt = 5 * 0.01 = 0.05*. This reward would be positive if the cheetah
-    runs forward (right).
-    - *ctrl_cost*: A cost for penalising the cheetah if it takes
-    actions that are too large. It is measured as *`ctrl_cost_weight` *
-    sum(action<sup>2</sup>)* where *`ctrl_cost_weight`* is a parameter set for the
-    control and has a default value of 0.1
+    The total reward is: ***reward*** *=* *forward_reward - ctrl_cost*.
+
+    - *forward_reward*:
+    A reward for moving forward,
+    this reward would be positive if the Half Cheetah moves forward (in the positive $x$ direction / in the right direction).
+    $w_{forward} \times \frac{dx}{dt}$, where
+    $dx$ is the displacement of the "tip" ($x_{after-action} - x_{before-action}$),
+    $dt$ is the time between actions, which depends on the `frame_skip` parameter (default is $5$),
+    and `frametime` which is $0.01$ - so the default is $dt = 5 \times 0.01 = 0.05$,
+    $w_{forward}$ is the `forward_reward_weight` (default is $1$).
+    - *ctrl_cost*:
+    A negative reward to penalize the Half Cheetah for taking actions that are too large.
+    $w_{control} \times \|action\|_2^2$,
+    where $w_{control}$ is `ctrl_cost_weight` (default is $0.1$).
+
+    `info` contains the individual reward terms.
 
-    The total reward returned is ***reward*** *=* *forward_reward - ctrl_cost* and `info` will also contain the individual reward terms
 
     ## Starting State
-    All observations start in state (0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0,
-    0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0,) with a noise added to the
-    initial state for stochasticity. As seen before, the first 8 values in the
-    state are positional and the last 9 values are velocity. A uniform noise in
-    the range of [-`reset_noise_scale`, `reset_noise_scale`] is added to the positional values while a standard
-    normal noise with a mean of 0 and standard deviation of `reset_noise_scale` is added to the
-    initial velocity values of all zeros.
+    The initial position state is $\mathcal{U}_{[-reset\_noise\_scale \times I_{9}, reset\_noise\_scale \times I_{9}]}$.
+    The initial velocity state is $\mathcal{N}(0_{9}, reset\_noise\_scale^2 \times I_{9})$.
 
-    ## Episode End
-    The episode truncates when the episode length is greater than 1000.
+    where $\mathcal{N}$ is the multivariate normal distribution and $\mathcal{U}$ is the multivariate uniform continuous distribution.
 
-    ## Arguments
 
-    No additional arguments are currently supported in v2 and lower.
+    ## Episode End
+    ### Termination
+    The Half Cheetah never terminates.
+
+    ### Truncation
+    The default duration of an episode is 1000 timesteps.
 
-    ```python
-    import gymnasium as gym
-    env = gym.make('HalfCheetah-v2')
-    ```
 
-    v3 and v4 take `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc.
+    ## Arguments
+    HalfCheetah provides a range of parameters to modify the observation space, reward function, initial state, and termination condition.
+    These parameters can be applied during `gymnasium.make` in the following way:
 
     ```python
     import gymnasium as gym
-    env = gym.make('HalfCheetah-v4', ctrl_cost_weight=0.1, ....)
+    env = gym.make('HalfCheetah-v5', ctrl_cost_weight=0.1, ....)
     ```
 
-    | Parameter                                    | Type      | Default              | Description                                                                                                                                                       |
-    | -------------------------------------------- | --------- | -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-    | `xml_file`                                   | **str**   | `"half_cheetah.xml"` | Path to a MuJoCo model                                                                                                                                            |
-    | `forward_reward_weight`                      | **float** | `1.0`                | Weight for _forward_reward_ term (see section on reward)                                                                                                          |
-    | `ctrl_cost_weight`                           | **float** | `0.1`                | Weight for _ctrl_cost_ weight (see section on reward)                                                                                                             |
-    | `reset_noise_scale`                          | **float** | `0.1`                | Scale of random perturbations of initial position and velocity (see section on Starting State)                                                                    |
-    | `exclude_current_positions_from_observation` | **bool**  | `True`               | Whether or not to omit the x-coordinate from observations. Excluding the position can serve as an inductive bias to induce position-agnostic behavior in policies |
+    | Parameter                                    | Type      | Default              | Description                                                                                                                                                                                         |
+    | -------------------------------------------- | --------- | -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+    | `xml_file`                                   | **str**   | `"half_cheetah.xml"` | Path to a MuJoCo model                                                                                                                                                                              |
+    | `forward_reward_weight`                      | **float** | `1`                  | Weight for _forward_reward_ term (see `Rewards` section)                                                                                                                                            |
+    | `ctrl_cost_weight`                           | **float** | `0.1`                | Weight for _ctrl_cost_ weight (see `Rewards` section)                                                                                                                                               |
+    | `reset_noise_scale`                          | **float** | `0.1`                | Scale of random perturbations of initial position and velocity (see `Starting State` section)                                                                                                       |
+    | `exclude_current_positions_from_observation` | **bool**  | `True`               | Whether or not to omit the x-coordinate from observations. Excluding the position can serve as an inductive bias to induce position-agnostic behavior in policies (see `Observation State` section) |
 
     ## Version History
-
-    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3
-    * v3: Support for `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc. rgb rendering comes from tracking camera (so agent does not run away from screen)
-    * v2: All continuous control environments now use mujoco-py >= 1.50
+    * v5:
+        - Minimum `mujoco` version is now 2.3.3.
+        - Added support for fully custom/third party `mujoco` models using the `xml_file` argument (previously only a few changes could be made to the existing models).
+        - Added `default_camera_config` argument, a dictionary for setting the `mj_camera` properties, mainly useful for custom environments.
+        - Added `env.observation_structure`, a dictionary for specifying the observation space compose (e.g. `qpos`, `qvel`), useful for building tooling and wrappers for the MuJoCo environments.
+        - Return a non-empty `info` with `reset()`, previously an empty dictionary was returned, the new keys are the same state information as `step()`.
+        - Added `frame_skip` argument, used to configure the `dt` (duration of `step()`), default varies by environment check environment documentation pages.
+        - Restored the `xml_file` argument (was removed in `v4`).
+        - Renamed `info["reward_run"]` to `info["reward_forward"]` to be consistent with the other environments.
+    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3.
+    * v3: Support for `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc. rgb rendering comes from tracking camera (so agent does not run away from screen).
+    * v2: All continuous control environments now use mujoco-py >= 1.50.
     * v1: max_time_steps raised to 1000 for robot based tasks. Added reward_threshold to environments.
-    * v0: Initial versions release (1.0.0)
+    * v0: Initial versions release.
     """
 
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
-        "render_fps": 20,
     }
 
     def __init__(
         self,
-        forward_reward_weight=1.0,
-        ctrl_cost_weight=0.1,
-        reset_noise_scale=0.1,
-        exclude_current_positions_from_observation=True,
+        xml_file: str = "half_cheetah.xml",
+        frame_skip: int = 5,
+        default_camera_config: Dict[str, Union[float, int]] = DEFAULT_CAMERA_CONFIG,
+        forward_reward_weight: float = 1.0,
+        ctrl_cost_weight: float = 0.1,
+        reset_noise_scale: float = 0.1,
+        exclude_current_positions_from_observation: bool = True,
         **kwargs,
     ):
         utils.EzPickle.__init__(
             self,
+            xml_file,
+            frame_skip,
+            default_camera_config,
             forward_reward_weight,
             ctrl_cost_weight,
             reset_noise_scale,
             exclude_current_positions_from_observation,
             **kwargs,
         )
 
         self._forward_reward_weight = forward_reward_weight
-
         self._ctrl_cost_weight = ctrl_cost_weight
 
         self._reset_noise_scale = reset_noise_scale
 
         self._exclude_current_positions_from_observation = (
             exclude_current_positions_from_observation
         )
 
-        if exclude_current_positions_from_observation:
-            observation_space = Box(
-                low=-np.inf, high=np.inf, shape=(17,), dtype=np.float64
-            )
-        else:
-            observation_space = Box(
-                low=-np.inf, high=np.inf, shape=(18,), dtype=np.float64
-            )
-
         MujocoEnv.__init__(
             self,
-            "half_cheetah.xml",
-            5,
-            observation_space=observation_space,
-            default_camera_config=DEFAULT_CAMERA_CONFIG,
+            xml_file,
+            frame_skip,
+            observation_space=None,
+            default_camera_config=default_camera_config,
             **kwargs,
         )
 
+        self.metadata = {
+            "render_modes": [
+                "human",
+                "rgb_array",
+                "depth_array",
+            ],
+            "render_fps": int(np.round(1.0 / self.dt)),
+        }
+
+        obs_size = (
+            self.data.qpos.size
+            + self.data.qvel.size
+            - exclude_current_positions_from_observation
+        )
+        self.observation_space = Box(
+            low=-np.inf, high=np.inf, shape=(obs_size,), dtype=np.float64
+        )
+
+        self.observation_structure = {
+            "skipped_qpos": 1 * exclude_current_positions_from_observation,
+            "qpos": self.data.qpos.size
+            - 1 * exclude_current_positions_from_observation,
+            "qvel": self.data.qvel.size,
+        }
+
     def control_cost(self, action):
         control_cost = self._ctrl_cost_weight * np.sum(np.square(action))
         return control_cost
 
     def step(self, action):
         x_position_before = self.data.qpos[0]
         self.do_simulation(action, self.frame_skip)
         x_position_after = self.data.qpos[0]
         x_velocity = (x_position_after - x_position_before) / self.dt
 
-        ctrl_cost = self.control_cost(action)
+        observation = self._get_obs()
+        reward, reward_info = self._get_rew(x_velocity, action)
+        info = {"x_position": x_position_after, "x_velocity": x_velocity, **reward_info}
 
+        if self.render_mode == "human":
+            self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
+        return observation, reward, False, False, info
+
+    def _get_rew(self, x_velocity: float, action):
         forward_reward = self._forward_reward_weight * x_velocity
+        ctrl_cost = self.control_cost(action)
 
-        observation = self._get_obs()
         reward = forward_reward - ctrl_cost
-        terminated = False
-        info = {
-            "x_position": x_position_after,
-            "x_velocity": x_velocity,
-            "reward_run": forward_reward,
+
+        reward_info = {
+            "reward_forward": forward_reward,
             "reward_ctrl": -ctrl_cost,
         }
-
-        if self.render_mode == "human":
-            self.render()
-        return observation, reward, terminated, False, info
+        return reward, reward_info
 
     def _get_obs(self):
-        position = self.data.qpos.flat.copy()
-        velocity = self.data.qvel.flat.copy()
+        position = self.data.qpos.flatten()
+        velocity = self.data.qvel.flatten()
 
         if self._exclude_current_positions_from_observation:
             position = position[1:]
 
         observation = np.concatenate((position, velocity)).ravel()
         return observation
 
@@ -238,7 +271,12 @@
             + self._reset_noise_scale * self.np_random.standard_normal(self.model.nv)
         )
 
         self.set_state(qpos, qvel)
 
         observation = self._get_obs()
         return observation
+
+    def _get_reset_info(self):
+        return {
+            "x_position": self.data.qpos[0],
+        }
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/hopper.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/walker2d.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,61 @@
 import numpy as np
 
 from gymnasium import utils
 from gymnasium.envs.mujoco import MuJocoPyEnv
 from gymnasium.spaces import Box
 
 
-class HopperEnv(MuJocoPyEnv, utils.EzPickle):
+class Walker2dEnv(MuJocoPyEnv, utils.EzPickle):
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
         "render_fps": 125,
     }
 
     def __init__(self, **kwargs):
-        observation_space = Box(low=-np.inf, high=np.inf, shape=(11,), dtype=np.float64)
+        observation_space = Box(low=-np.inf, high=np.inf, shape=(17,), dtype=np.float64)
         MuJocoPyEnv.__init__(
-            self, "hopper.xml", 4, observation_space=observation_space, **kwargs
+            self, "walker2d.xml", 4, observation_space=observation_space, **kwargs
         )
         utils.EzPickle.__init__(self, **kwargs)
 
     def step(self, a):
         posbefore = self.sim.data.qpos[0]
         self.do_simulation(a, self.frame_skip)
         posafter, height, ang = self.sim.data.qpos[0:3]
 
         alive_bonus = 1.0
         reward = (posafter - posbefore) / self.dt
         reward += alive_bonus
         reward -= 1e-3 * np.square(a).sum()
-        s = self.state_vector()
-        terminated = not (
-            np.isfinite(s).all()
-            and (np.abs(s[2:]) < 100).all()
-            and (height > 0.7)
-            and (abs(ang) < 0.2)
-        )
+        terminated = not (height > 0.8 and height < 2.0 and ang > -1.0 and ang < 1.0)
         ob = self._get_obs()
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return ob, reward, terminated, False, {}
 
     def _get_obs(self):
-        return np.concatenate(
-            [self.sim.data.qpos.flat[1:], np.clip(self.sim.data.qvel.flat, -10, 10)]
-        )
+        qpos = self.sim.data.qpos
+        qvel = self.sim.data.qvel
+        return np.concatenate([qpos[1:], np.clip(qvel, -10, 10)]).ravel()
 
     def reset_model(self):
-        qpos = self.init_qpos + self.np_random.uniform(
-            low=-0.005, high=0.005, size=self.model.nq
-        )
-        qvel = self.init_qvel + self.np_random.uniform(
-            low=-0.005, high=0.005, size=self.model.nv
+        self.set_state(
+            self.init_qpos
+            + self.np_random.uniform(low=-0.005, high=0.005, size=self.model.nq),
+            self.init_qvel
+            + self.np_random.uniform(low=-0.005, high=0.005, size=self.model.nv),
         )
-        self.set_state(qpos, qvel)
         return self._get_obs()
 
     def viewer_setup(self):
         assert self.viewer is not None
         self.viewer.cam.trackbodyid = 2
-        self.viewer.cam.distance = self.model.stat.extent * 0.75
+        self.viewer.cam.distance = self.model.stat.extent * 0.5
         self.viewer.cam.lookat[2] = 1.15
         self.viewer.cam.elevation = -20
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/hopper_v3.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/hopper_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
         info = {
             "x_position": x_position_after,
             "x_velocity": x_velocity,
         }
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return observation, reward, terminated, False, info
 
     def reset_model(self):
         noise_low = -self._reset_noise_scale
         noise_high = self._reset_noise_scale
 
         qpos = self.init_qpos + self.np_random.uniform(
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/hopper_v4.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/hopper_v5.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+__credits__ = ["Kallinteris-Andreas"]
+
+from typing import Dict, Tuple, Union
+
 import numpy as np
 
 from gymnasium import utils
 from gymnasium.envs.mujoco import MujocoEnv
 from gymnasium.spaces import Box
 
 
@@ -10,52 +14,50 @@
     "distance": 3.0,
     "lookat": np.array((0.0, 0.0, 1.15)),
     "elevation": -20.0,
 }
 
 
 class HopperEnv(MujocoEnv, utils.EzPickle):
-    """
+    r"""
     ## Description
+    This environment is based on the work of Erez, Tassa, and Todorov in ["Infinite Horizon Model Predictive Control for Nonlinear Periodic Tasks"](http://www.roboticsproceedings.org/rss07/p10.pdf).
+    The environment aims to increase the number of independent state and control variables compared to classical control environments.
+    The hopper is a two-dimensional one-legged figure consisting of four main body parts - the torso at the top, the thigh in the middle, the leg at the bottom, and a single foot on which the entire body rests.
+    The goal is to make hops that move in the forward (right) direction by applying torque to the three hinges that connect the four body parts.
 
-    This environment is based on the work done by Erez, Tassa, and Todorov in
-    ["Infinite Horizon Model Predictive Control for Nonlinear Periodic Tasks"](http://www.roboticsproceedings.org/rss07/p10.pdf). The environment aims to
-    increase the number of independent state and control variables as compared to
-    the classic control environments. The hopper is a two-dimensional
-    one-legged figure that consist of four main body parts - the torso at the
-    top, the thigh in the middle, the leg in the bottom, and a single foot on
-    which the entire body rests. The goal is to make hops that move in the
-    forward (right) direction by applying torques on the three hinges
-    connecting the four body parts.
 
     ## Action Space
+    ```{figure} action_space_figures/hopper.png
+    :name: hopper
+    ```
+
     The action space is a `Box(-1, 1, (3,), float32)`. An action represents the torques applied at the hinge joints.
 
-    | Num | Action                             | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit         |
+    | Num | Action                             | Control Min | Control Max | Name (in corresponding XML file) | Joint | Type (Unit)  |
     |-----|------------------------------------|-------------|-------------|----------------------------------|-------|--------------|
     | 0   | Torque applied on the thigh rotor  | -1          | 1           | thigh_joint                      | hinge | torque (N m) |
     | 1   | Torque applied on the leg rotor    | -1          | 1           | leg_joint                        | hinge | torque (N m) |
     | 2   | Torque applied on the foot rotor   | -1          | 1           | foot_joint                       | hinge | torque (N m) |
 
+
     ## Observation Space
-    Observations consist of positional values of different body parts of the
-    hopper, followed by the velocities of those individual parts
-    (their derivatives) with all the positions ordered before all the velocities.
-
-    By default, observations do not include the x-coordinate of the hopper. It may
-    be included by passing `exclude_current_positions_from_observation=False` during construction.
-    In that case, the observation space will be `Box(-Inf, Inf, (12,), float64)` where the first observation
-    represents the x-coordinate of the hopper.
-    Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the x-coordinate
-    will be returned in `info` with key `"x_position"`.
+    The observation space consists of the following parts (in order):
+
+    - *qpos (5 elements by default):* Position values of the robot's body parts.
+    - *qvel (6 elements):* The velocities of these individual body parts (their derivatives).
 
-    However, by default, the observation is a `Box(-Inf, Inf, (11,), float64)` where the elements
-    correspond to the following:
+    By default, the observation does not include the robot's x-coordinate (`rootx`).
+    This can  be included by passing `exclude_current_positions_from_observation=False` during construction.
+    In this case, the observation space will be a `Box(-Inf, Inf, (12,), float64)`, where the first observation element is the x-coordinate of the robot.
+    Regardless of whether `exclude_current_positions_from_observation` is set to `True` or `False`, the x- and y-coordinates are returned in `info` with the keys `"x_position"` and `"y_position"`, respectively.
 
-    | Num | Observation                                        | Min  | Max | Name (in corresponding XML file) | Joint | Unit                     |
+    By default, however, the observation space is a `Box(-Inf, Inf, (11,), float64)` where the elements are as follows:
+
+    | Num | Observation                                        | Min  | Max | Name (in corresponding XML file) | Joint | Type (Unit)              |
     | --- | -------------------------------------------------- | ---- | --- | -------------------------------- | ----- | ------------------------ |
     | 0   | z-coordinate of the torso (height of hopper)       | -Inf | Inf | rootz                            | slide | position (m)             |
     | 1   | angle of the torso                                 | -Inf | Inf | rooty                            | hinge | angle (rad)              |
     | 2   | angle of the thigh joint                           | -Inf | Inf | thigh_joint                      | hinge | angle (rad)              |
     | 3   | angle of the leg joint                             | -Inf | Inf | leg_joint                        | hinge | angle (rad)              |
     | 4   | angle of the foot joint                            | -Inf | Inf | foot_joint                       | hinge | angle (rad)              |
     | 5   | velocity of the x-coordinate of the torso          | -Inf | Inf | rootx                          | slide | velocity (m/s)           |
@@ -64,111 +66,127 @@
     | 8   | angular velocity of the thigh hinge                | -Inf | Inf | thigh_joint                      | hinge | angular velocity (rad/s) |
     | 9   | angular velocity of the leg hinge                  | -Inf | Inf | leg_joint                        | hinge | angular velocity (rad/s) |
     | 10  | angular velocity of the foot hinge                 | -Inf | Inf | foot_joint                       | hinge | angular velocity (rad/s) |
     | excluded | x-coordinate of the torso                     | -Inf | Inf | rootx                            | slide | position (m)             |
 
 
     ## Rewards
-    The reward consists of three parts:
-    - *healthy_reward*: Every timestep that the hopper is healthy (see definition in section "Episode Termination"), it gets a reward of fixed value `healthy_reward`.
-    - *forward_reward*: A reward of hopping forward which is measured
-    as *`forward_reward_weight` * (x-coordinate before action - x-coordinate after action)/dt*. *dt* is
-    the time between actions and is dependent on the frame_skip parameter
-    (fixed to 4), where the frametime is 0.002 - making the
-    default *dt = 4 * 0.002 = 0.008*. This reward would be positive if the hopper
-    hops forward (positive x direction).
-    - *ctrl_cost*: A cost for penalising the hopper if it takes
-    actions that are too large. It is measured as *`ctrl_cost_weight` *
-    sum(action<sup>2</sup>)* where *`ctrl_cost_weight`* is a parameter set for the
-    control and has a default value of 0.001
+    The total reward is: ***reward*** *=* *healthy_reward + forward_reward - ctrl_cost*.
 
-    The total reward returned is ***reward*** *=* *healthy_reward + forward_reward - ctrl_cost* and `info` will also contain the individual reward terms
+    - *healthy_reward*:
+    Every timestep that the Hopper is healthy (see definition in section "Episode End"),
+    it gets a reward of fixed value `healthy_reward` (default is $1$).
+    - *forward_reward*:
+    A reward for moving forward,
+    this reward would be positive if the Hopper moves forward (in the positive $x$ direction / in the right direction).
+    $w_{forward} \times \frac{dx}{dt}$, where
+    $dx$ is the displacement of the "torso" ($x_{after-action} - x_{before-action}$),
+    $dt$ is the time between actions, which depends on the `frame_skip` parameter (default is $4$),
+    and `frametime` which is $0.002$ - so the default is $dt = 4 \times 0.002 = 0.008$,
+    $w_{forward}$ is the `forward_reward_weight` (default is $1$).
+    - *ctrl_cost*:
+    A negative reward to penalize the Hopper for taking actions that are too large.
+    $w_{control} \times \|action\|_2^2$,
+    where $w_{control}$ is `ctrl_cost_weight` (default is $10^{-3}$).
 
-    ## Starting State
-    All observations start in state
-    (0.0, 1.25, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0) with a uniform noise
-     in the range of [-`reset_noise_scale`, `reset_noise_scale`] added to the values for stochasticity.
+    `info` contains the individual reward terms.
 
-    ## Episode End
-    The hopper is said to be unhealthy if any of the following happens:
 
-    1. An element of `observation[1:]` (if  `exclude_current_positions_from_observation=True`, else `observation[2:]`) is no longer contained in the closed interval specified by the argument `healthy_state_range`
-    2. The height of the hopper (`observation[0]` if  `exclude_current_positions_from_observation=True`, else `observation[1]`) is no longer contained in the closed interval specified by the argument `healthy_z_range` (usually meaning that it has fallen)
-    3. The angle (`observation[1]` if  `exclude_current_positions_from_observation=True`, else `observation[2]`) is no longer contained in the closed interval specified by the argument `healthy_angle_range`
+    ## Starting State
+    The initial position state is $[0, 1.25, 0, 0, 0, 0] + \mathcal{U}_{[-reset\_noise\_scale \times I_{6}, reset\_noise\_scale \times I_{6}]}$.
+    The initial velocity state is $\mathcal{U}_{[-reset\_noise\_scale \times I_{6}, reset\_noise\_scale \times I_{6}]}$.
 
-    If `terminate_when_unhealthy=True` is passed during construction (which is the default),
-    the episode ends when any of the following happens:
+    where $\mathcal{U}$ is the multivariate uniform continuous distribution.
 
-    1. Truncation: The episode duration reaches a 1000 timesteps
-    2. Termination: The hopper is unhealthy
+    Note that the z-coordinate is non-zero so that the hopper can stand up immediately.
 
-    If `terminate_when_unhealthy=False` is passed, the episode is ended only when 1000 timesteps are exceeded.
 
-    ## Arguments
+    ## Episode End
+    ### Termination
+    If `terminate_when_unhealthy is True` (the default), the environment terminates when the Hopper is unhealthy.
+    The Hopper is unhealthy if any of the following happens:
+
+    1. An element of `observation[1:]` (if  `exclude_current_positions_from_observation=True`, otherwise `observation[2:]`) is no longer contained in the closed interval specified by the `healthy_state_range` argument (default is $[-100, 100]$).
+    2. The height of the hopper (`observation[0]` if  `exclude_current_positions_from_observation=True`, otherwise `observation[1]`) is no longer contained in the closed interval specified by the `healthy_z_range` argument (default is $[0.7, +\infty]$) (usually meaning that it has fallen).
+    3. The angle of the torso (`observation[1]` if  `exclude_current_positions_from_observation=True`, otherwise `observation[2]`) is no longer contained in the closed interval specified by the `healthy_angle_range` argument (default is $[-0.2, 0.2]$).
 
-    No additional arguments are currently supported in v2 and lower.
+    ### Truncation
+    The default duration of an episode is 1000 timesteps.
 
-    ```python
-    import gymnasium as gym
-    env = gym.make('Hopper-v2')
-    ```
 
-    v3 and v4 take `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc.
+    ## Arguments
+    Hopper provides a range of parameters to modify the observation space, reward function, initial state, and termination condition.
+    These parameters can be applied during `gymnasium.make` in the following way:
 
     ```python
     import gymnasium as gym
-    env = gym.make('Hopper-v4', ctrl_cost_weight=0.1, ....)
+    env = gym.make('Hopper-v5', ctrl_cost_weight=1e-3, ....)
     ```
 
-    | Parameter                                    | Type      | Default               | Description                                                                                                                                                                     |
-    | -------------------------------------------- | --------- | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-    | `xml_file`                                   | **str**   | `"hopper.xml"`        | Path to a MuJoCo model                                                                                                                                                          |
-    | `forward_reward_weight`                      | **float** | `1.0`                 | Weight for _forward_reward_ term (see section on reward)                                                                                                                        |
-    | `ctrl_cost_weight`                           | **float** | `0.001`               | Weight for _ctrl_cost_ reward (see section on reward)                                                                                                                           |
-    | `healthy_reward`                             | **float** | `1`                   | Constant reward given if the ant is "healthy" after timestep                                                                                                                    |
-    | `terminate_when_unhealthy`                   | **bool**  | `True`                | If true, issue a done signal if the hopper is no longer healthy                                                                                                                 |
-    | `healthy_state_range`                        | **tuple** | `(-100, 100)`         | The elements of `observation[1:]` (if `exclude_current_positions_from_observation=True`, else `observation[2:]`) must be in this range for the hopper to be considered healthy  |
-    | `healthy_z_range`                            | **tuple** | `(0.7, float("inf"))` | The z-coordinate must be in this range for the hopper to be considered healthy                                                                                                  |
-    | `healthy_angle_range`                        | **tuple** | `(-0.2, 0.2)`         | The angle given by `observation[1]` (if `exclude_current_positions_from_observation=True`, else `observation[2]`) must be in this range for the hopper to be considered healthy |
-    | `reset_noise_scale`                          | **float** | `5e-3`                | Scale of random perturbations of initial position and velocity (see section on Starting State)                                                                                  |
-    | `exclude_current_positions_from_observation` | **bool**  | `True`                | Whether or not to omit the x-coordinate from observations. Excluding the position can serve as an inductive bias to induce position-agnostic behavior in policies               |
+    | Parameter                                    | Type      | Default               | Description                                                                                                                                                                                                 |
+    | -------------------------------------------- | --------- | --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+    | `xml_file`                                   | **str**   | `"hopper.xml"`        | Path to a MuJoCo model                                                                                                                                                                                      |
+    | `forward_reward_weight`                      | **float** | `1`                   | Weight for _forward_reward_ term (see `Rewards` section)                                                                                                                                                    |
+    | `ctrl_cost_weight`                           | **float** | `1e-3`                | Weight for _ctrl_cost_ reward (see `Rewards` section)                                                                                                                                                       |
+    | `healthy_reward`                             | **float** | `1`                   | Weight for _healthy_reward_ reward (see `Rewards` section)                                                                                                                                                  |
+    | `terminate_when_unhealthy`                   | **bool**  | `True`                | If `True`, issue a `terminated` signal is unhealthy (see `Episode End` section)                                                                                                                                |
+    | `healthy_state_range`                        | **tuple** | `(-100, 100)`         | The elements of `observation[1:]` (if `exclude_current_positions_from_observation=True`, else `observation[2:]`) must be in this range for the hopper to be considered healthy (see `Episode End` section)  |
+    | `healthy_z_range`                            | **tuple** | `(0.7, float("inf"))` | The z-coordinate must be in this range for the hopper to be considered healthy (see `Episode End` section)                                                                                                  |
+    | `healthy_angle_range`                        | **tuple** | `(-0.2, 0.2)`         | The angle given by `observation[1]` (if `exclude_current_positions_from_observation=True`, else `observation[2]`) must be in this range for the hopper to be considered healthy (see `Episode End` section) |
+    | `reset_noise_scale`                          | **float** | `5e-3`                | Scale of random perturbations of initial position and velocity (see `Starting State` section)                                                                                                               |
+    | `exclude_current_positions_from_observation` | **bool**  | `True`                | Whether or not to omit the x-coordinate from observations. Excluding the position can serve as an inductive bias to induce position-agnostic behavior in policies(see `Observation Space` section)          |
 
     ## Version History
-
-    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3
+    * v5:
+        - Minimum `mujoco` version is now 2.3.3.
+        - Added support for fully custom/third party `mujoco` models using the `xml_file` argument (previously only a few changes could be made to the existing models).
+        - Added `default_camera_config` argument, a dictionary for setting the `mj_camera` properties, mainly useful for custom environments.
+        - Added `env.observation_structure`, a dictionary for specifying the observation space compose (e.g. `qpos`, `qvel`), useful for building tooling and wrappers for the MuJoCo environments.
+        - Return a non-empty `info` with `reset()`, previously an empty dictionary was returned, the new keys are the same state information as `step()`.
+        - Added `frame_skip` argument, used to configure the `dt` (duration of `step()`), default varies by environment check environment documentation pages.
+        - Fixed bug: `healthy_reward` was given on every step (even if the Hopper was unhealthy), now it is only given when the Hopper is healthy. The `info["reward_survive"]` is updated with this change (related [GitHub issue](https://github.com/Farama-Foundation/Gymnasium/issues/526)).
+        - Restored the `xml_file` argument (was removed in `v4`).
+        - Added individual reward terms in `info` (`info["reward_forward"]`, info`["reward_ctrl"]`, `info["reward_survive"]`).
+        - Added `info["z_distance_from_origin"]` which is equal to the vertical distance of the "torso" body from its initial position.
+    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3.
     * v3: Support for `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc. rgb rendering comes from tracking camera (so agent does not run away from screen)
-    * v2: All continuous control environments now use mujoco-py >= 1.50
+    * v2: All continuous control environments now use mujoco-py >= 1.50.
     * v1: max_time_steps raised to 1000 for robot based tasks. Added reward_threshold to environments.
-    * v0: Initial versions release (1.0.0)
+    * v0: Initial versions release.
     """
 
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
-        "render_fps": 125,
     }
 
     def __init__(
         self,
-        forward_reward_weight=1.0,
-        ctrl_cost_weight=1e-3,
-        healthy_reward=1.0,
-        terminate_when_unhealthy=True,
-        healthy_state_range=(-100.0, 100.0),
-        healthy_z_range=(0.7, float("inf")),
-        healthy_angle_range=(-0.2, 0.2),
-        reset_noise_scale=5e-3,
-        exclude_current_positions_from_observation=True,
+        xml_file: str = "hopper.xml",
+        frame_skip: int = 4,
+        default_camera_config: Dict[str, Union[float, int]] = DEFAULT_CAMERA_CONFIG,
+        forward_reward_weight: float = 1.0,
+        ctrl_cost_weight: float = 1e-3,
+        healthy_reward: float = 1.0,
+        terminate_when_unhealthy: bool = True,
+        healthy_state_range: Tuple[float, float] = (-100.0, 100.0),
+        healthy_z_range: Tuple[float, float] = (0.7, float("inf")),
+        healthy_angle_range: Tuple[float, float] = (-0.2, 0.2),
+        reset_noise_scale: float = 5e-3,
+        exclude_current_positions_from_observation: bool = True,
         **kwargs,
     ):
         utils.EzPickle.__init__(
             self,
+            xml_file,
+            frame_skip,
+            default_camera_config,
             forward_reward_weight,
             ctrl_cost_weight,
             healthy_reward,
             terminate_when_unhealthy,
             healthy_state_range,
             healthy_z_range,
             healthy_angle_range,
@@ -190,38 +208,51 @@
 
         self._reset_noise_scale = reset_noise_scale
 
         self._exclude_current_positions_from_observation = (
             exclude_current_positions_from_observation
         )
 
-        if exclude_current_positions_from_observation:
-            observation_space = Box(
-                low=-np.inf, high=np.inf, shape=(11,), dtype=np.float64
-            )
-        else:
-            observation_space = Box(
-                low=-np.inf, high=np.inf, shape=(12,), dtype=np.float64
-            )
-
         MujocoEnv.__init__(
             self,
-            "hopper.xml",
-            4,
-            observation_space=observation_space,
-            default_camera_config=DEFAULT_CAMERA_CONFIG,
+            xml_file,
+            frame_skip,
+            observation_space=None,
+            default_camera_config=default_camera_config,
             **kwargs,
         )
 
+        self.metadata = {
+            "render_modes": [
+                "human",
+                "rgb_array",
+                "depth_array",
+            ],
+            "render_fps": int(np.round(1.0 / self.dt)),
+        }
+
+        obs_size = (
+            self.data.qpos.size
+            + self.data.qvel.size
+            - exclude_current_positions_from_observation
+        )
+        self.observation_space = Box(
+            low=-np.inf, high=np.inf, shape=(obs_size,), dtype=np.float64
+        )
+
+        self.observation_structure = {
+            "skipped_qpos": 1 * exclude_current_positions_from_observation,
+            "qpos": self.data.qpos.size
+            - 1 * exclude_current_positions_from_observation,
+            "qvel": self.data.qvel.size,
+        }
+
     @property
     def healthy_reward(self):
-        return (
-            float(self.is_healthy or self._terminate_when_unhealthy)
-            * self._healthy_reward
-        )
+        return self.is_healthy * self._healthy_reward
 
     def control_cost(self, action):
         control_cost = self._ctrl_cost_weight * np.sum(np.square(action))
         return control_cost
 
     @property
     def is_healthy(self):
@@ -236,55 +267,63 @@
         healthy_z = min_z < z < max_z
         healthy_angle = min_angle < angle < max_angle
 
         is_healthy = all((healthy_state, healthy_z, healthy_angle))
 
         return is_healthy
 
-    @property
-    def terminated(self):
-        terminated = not self.is_healthy if self._terminate_when_unhealthy else False
-        return terminated
-
     def _get_obs(self):
-        position = self.data.qpos.flat.copy()
-        velocity = np.clip(self.data.qvel.flat.copy(), -10, 10)
+        position = self.data.qpos.flatten()
+        velocity = np.clip(self.data.qvel.flatten(), -10, 10)
 
         if self._exclude_current_positions_from_observation:
             position = position[1:]
 
         observation = np.concatenate((position, velocity)).ravel()
         return observation
 
     def step(self, action):
         x_position_before = self.data.qpos[0]
         self.do_simulation(action, self.frame_skip)
         x_position_after = self.data.qpos[0]
         x_velocity = (x_position_after - x_position_before) / self.dt
 
-        ctrl_cost = self.control_cost(action)
-
-        forward_reward = self._forward_reward_weight * x_velocity
-        healthy_reward = self.healthy_reward
-
-        rewards = forward_reward + healthy_reward
-        costs = ctrl_cost
-
         observation = self._get_obs()
-        reward = rewards - costs
-        terminated = self.terminated
+        reward, reward_info = self._get_rew(x_velocity, action)
+        terminated = (not self.is_healthy) and self._terminate_when_unhealthy
         info = {
             "x_position": x_position_after,
+            "z_distance_from_origin": self.data.qpos[1] - self.init_qpos[1],
             "x_velocity": x_velocity,
+            **reward_info,
         }
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return observation, reward, terminated, False, info
 
+    def _get_rew(self, x_velocity: float, action):
+        forward_reward = self._forward_reward_weight * x_velocity
+        healthy_reward = self.healthy_reward
+        rewards = forward_reward + healthy_reward
+
+        ctrl_cost = self.control_cost(action)
+        costs = ctrl_cost
+
+        reward = rewards - costs
+
+        reward_info = {
+            "reward_forward": forward_reward,
+            "reward_ctrl": -ctrl_cost,
+            "reward_survive": healthy_reward,
+        }
+
+        return reward, reward_info
+
     def reset_model(self):
         noise_low = -self._reset_noise_scale
         noise_high = self._reset_noise_scale
 
         qpos = self.init_qpos + self.np_random.uniform(
             low=noise_low, high=noise_high, size=self.model.nq
         )
@@ -292,7 +331,13 @@
             low=noise_low, high=noise_high, size=self.model.nv
         )
 
         self.set_state(qpos, qvel)
 
         observation = self._get_obs()
         return observation
+
+    def _get_reset_info(self):
+        return {
+            "x_position": self.data.qpos[0],
+            "z_distance_from_origin": self.data.qpos[1] - self.init_qpos[1],
+        }
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/humanoid.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/humanoid.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         quad_impact_cost = min(quad_impact_cost, 10)
         reward = lin_vel_cost - quad_ctrl_cost - quad_impact_cost + alive_bonus
         qpos = self.sim.data.qpos
         terminated = bool((qpos[2] < 1.0) or (qpos[2] > 2.0))
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return (
             self._get_obs(),
             reward,
             terminated,
             False,
             dict(
                 reward_linvel=lin_vel_cost,
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/humanoid_v3.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/humanoid_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,15 @@
             "x_velocity": x_velocity,
             "y_velocity": y_velocity,
             "forward_reward": forward_reward,
         }
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return observation, reward, terminated, False, info
 
     def reset_model(self):
         noise_low = -self._reset_noise_scale
         noise_high = self._reset_noise_scale
 
         qpos = self.init_qpos + self.np_random.uniform(
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/humanoid_v4.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/humanoid_v5.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+__credits__ = ["Kallinteris-Andreas"]
+
+from typing import Dict, Tuple, Union
+
 import numpy as np
 
 from gymnasium import utils
 from gymnasium.envs.mujoco import MujocoEnv
 from gymnasium.spaces import Box
 
 
@@ -16,61 +20,80 @@
 def mass_center(model, data):
     mass = np.expand_dims(model.body_mass, axis=1)
     xpos = data.xipos
     return (np.sum(mass * xpos, axis=0) / np.sum(mass))[0:2].copy()
 
 
 class HumanoidEnv(MujocoEnv, utils.EzPickle):
-    """
+    r"""
     ## Description
+    This environment is based on the environment introduced by Tassa, Erez and Todorov in ["Synthesis and stabilization of complex behaviors through online trajectory optimization"](https://ieeexplore.ieee.org/document/6386025).
+    The 3D bipedal robot is designed to simulate a human.
+    It has a torso (abdomen) with a pair of legs and arms, and a pair of tendons connecting the hips to the knees.
+    The legs each consist of three body parts (thigh, shin, foot), and the arms consist of two body parts (upper arm, forearm).
+    The goal of the environment is to walk forward as fast as possible without falling over.
 
-    This environment is based on the environment introduced by Tassa, Erez and Todorov
-    in ["Synthesis and stabilization of complex behaviors through online trajectory optimization"](https://ieeexplore.ieee.org/document/6386025).
-    The 3D bipedal robot is designed to simulate a human. It has a torso (abdomen) with a pair of
-    legs and arms. The legs each consist of three body parts, and the arms 2 body parts (representing the knees and
-    elbows respectively). The goal of the environment is to walk forward as fast as possible without falling over.
 
     ## Action Space
+    ```{figure} action_space_figures/humanoid.png
+    :name: humanoid
+    ```
+
     The action space is a `Box(-1, 1, (17,), float32)`. An action represents the torques applied at the hinge joints.
 
-    | Num | Action                    | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit |
-    |-----|----------------------|---------------|----------------|---------------------------------------|-------|------|
-    | 0   | Torque applied on the hinge in the y-coordinate of the abdomen                     | -0.4 | 0.4 | abdomen_y                   | hinge | torque (N m) |
-    | 1   | Torque applied on the hinge in the z-coordinate of the abdomen                     | -0.4 | 0.4 | abdomen_z                   | hinge | torque (N m) |
-    | 2   | Torque applied on the hinge in the x-coordinate of the abdomen                     | -0.4 | 0.4 | abdomen_x                   | hinge | torque (N m) |
-    | 3   | Torque applied on the rotor between torso/abdomen and the right hip (x-coordinate) | -0.4 | 0.4 | right_hip_x (right_thigh)   | hinge | torque (N m) |
-    | 4   | Torque applied on the rotor between torso/abdomen and the right hip (z-coordinate) | -0.4 | 0.4 | right_hip_z (right_thigh)   | hinge | torque (N m) |
-    | 5   | Torque applied on the rotor between torso/abdomen and the right hip (y-coordinate) | -0.4 | 0.4 | right_hip_y (right_thigh)   | hinge | torque (N m) |
-    | 6   | Torque applied on the rotor between the right hip/thigh and the right shin         | -0.4 | 0.4 | right_knee                  | hinge | torque (N m) |
-    | 7   | Torque applied on the rotor between torso/abdomen and the left hip (x-coordinate)  | -0.4 | 0.4 | left_hip_x (left_thigh)     | hinge | torque (N m) |
-    | 8   | Torque applied on the rotor between torso/abdomen and the left hip (z-coordinate)  | -0.4 | 0.4 | left_hip_z (left_thigh)     | hinge | torque (N m) |
-    | 9   | Torque applied on the rotor between torso/abdomen and the left hip (y-coordinate)  | -0.4 | 0.4 | left_hip_y (left_thigh)     | hinge | torque (N m) |
-    | 10  | Torque applied on the rotor between the left hip/thigh and the left shin           | -0.4 | 0.4 | left_knee                   | hinge | torque (N m) |
-    | 11  | Torque applied on the rotor between the torso and right upper arm (coordinate -1)  | -0.4 | 0.4 | right_shoulder1             | hinge | torque (N m) |
-    | 12  | Torque applied on the rotor between the torso and right upper arm (coordinate -2)  | -0.4 | 0.4 | right_shoulder2             | hinge | torque (N m) |
-    | 13  | Torque applied on the rotor between the right upper arm and right lower arm        | -0.4 | 0.4 | right_elbow                 | hinge | torque (N m) |
-    | 14  | Torque applied on the rotor between the torso and left upper arm (coordinate -1)   | -0.4 | 0.4 | left_shoulder1              | hinge | torque (N m) |
-    | 15  | Torque applied on the rotor between the torso and left upper arm (coordinate -2)   | -0.4 | 0.4 | left_shoulder2              | hinge | torque (N m) |
-    | 16  | Torque applied on the rotor between the left upper arm and left lower arm          | -0.4 | 0.4 | left_elbow                  | hinge | torque (N m) |
+    | Num | Action                                                                             | Control Min | Control Max | Name (in corresponding XML file) | Joint | Type (Unit)  |
+    | --- | ---------------------------------------------------------------------------------- | ----------- | ----------- | -------------------------------- | ----- | ------------ |
+    | 0   | Torque applied on the hinge in the y-coordinate of the abdomen                     | -0.4        | 0.4         | abdomen_y                        | hinge | torque (N m) |
+    | 1   | Torque applied on the hinge in the z-coordinate of the abdomen                     | -0.4        | 0.4         | abdomen_z                        | hinge | torque (N m) |
+    | 2   | Torque applied on the hinge in the x-coordinate of the abdomen                     | -0.4        | 0.4         | abdomen_x                        | hinge | torque (N m) |
+    | 3   | Torque applied on the rotor between torso/abdomen and the right hip (x-coordinate) | -0.4        | 0.4         | right_hip_x (right_thigh)        | hinge | torque (N m) |
+    | 4   | Torque applied on the rotor between torso/abdomen and the right hip (z-coordinate) | -0.4        | 0.4         | right_hip_z (right_thigh)        | hinge | torque (N m) |
+    | 5   | Torque applied on the rotor between torso/abdomen and the right hip (y-coordinate) | -0.4        | 0.4         | right_hip_y (right_thigh)        | hinge | torque (N m) |
+    | 6   | Torque applied on the rotor between the right hip/thigh and the right shin         | -0.4        | 0.4         | right_knee                       | hinge | torque (N m) |
+    | 7   | Torque applied on the rotor between torso/abdomen and the left hip (x-coordinate)  | -0.4        | 0.4         | left_hip_x (left_thigh)          | hinge | torque (N m) |
+    | 8   | Torque applied on the rotor between torso/abdomen and the left hip (z-coordinate)  | -0.4        | 0.4         | left_hip_z (left_thigh)          | hinge | torque (N m) |
+    | 9   | Torque applied on the rotor between torso/abdomen and the left hip (y-coordinate)  | -0.4        | 0.4         | left_hip_y (left_thigh)          | hinge | torque (N m) |
+    | 10  | Torque applied on the rotor between the left hip/thigh and the left shin           | -0.4        | 0.4         | left_knee                        | hinge | torque (N m) |
+    | 11  | Torque applied on the rotor between the torso and right upper arm (coordinate -1)  | -0.4        | 0.4         | right_shoulder1                  | hinge | torque (N m) |
+    | 12  | Torque applied on the rotor between the torso and right upper arm (coordinate -2)  | -0.4        | 0.4         | right_shoulder2                  | hinge | torque (N m) |
+    | 13  | Torque applied on the rotor between the right upper arm and right lower arm        | -0.4        | 0.4         | right_elbow                      | hinge | torque (N m) |
+    | 14  | Torque applied on the rotor between the torso and left upper arm (coordinate -1)   | -0.4        | 0.4         | left_shoulder1                   | hinge | torque (N m) |
+    | 15  | Torque applied on the rotor between the torso and left upper arm (coordinate -2)   | -0.4        | 0.4         | left_shoulder2                   | hinge | torque (N m) |
+    | 16  | Torque applied on the rotor between the left upper arm and left lower arm          | -0.4        | 0.4         | left_elbow                       | hinge | torque (N m) |
+
 
     ## Observation Space
-    Observations consist of positional values of different body parts of the Humanoid,
-    followed by the velocities of those individual parts (their derivatives) with all the
-    positions ordered before all the velocities.
-
-    By default, observations do not include the x- and y-coordinates of the torso. These may
-    be included by passing `exclude_current_positions_from_observation=False` during construction.
-    In that case, the observation space will be a `Box(-Inf, Inf, (378,), float64)` where the first two observations
-    represent the x- and y-coordinates of the torso.
-    Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the x- and y-coordinates
-    will be returned in `info` with keys `"x_position"` and `"y_position"`, respectively.
+    The observation space consists of the following parts (in order)
 
-    However, by default, the observation is a `Box(-Inf, Inf, (376,), float64)`. The elements correspond to the following:
+    - *qpos (22 elements by default):* The position values of the robot's body parts.
+    - *qvel (23 elements):* The velocities of these individual body parts (their derivatives).
+    - *cinert (130 elements):* Mass and inertia of the rigid body parts relative to the center of mass,
+    (this is an intermediate result of the transition).
+    It has shape 13*10 (*nbody * 10*).
+    (cinert - inertia matrix and body mass offset and body mass)
+    - *cvel (78 elements):* Center of mass based velocity.
+    It has shape 13 * 6 (*nbody * 6*).
+    (com velocity - velocity x, y, z and angular velocity x, y, z)
+    - *qfrc_actuator (17 elements):* Constraint force generated as the actuator force at each joint.
+    This has shape `(17,)`  *(nv * 1)*.
+    - *cfrc_ext (78 elements):* This is the center of mass based external force on the body parts.
+    It has shape 13 * 6 (*nbody * 6*) and thus adds another 78 elements to the observation space.
+    (external forces - force x, y, z and torque x, y, z)
+
+    where *nbody* is the number of bodies in the robot,
+    and *nv* is the number of degrees of freedom (*= dim(qvel)*).
+
+    By default, the observation does not include the x- and y-coordinates of the torso.
+    These can be included by passing `exclude_current_positions_from_observation=False` during construction.
+    In this case, the observation space will be a `Box(-Inf, Inf, (350,), float64)`, where the first two observations are the x- and y-coordinates of the torso.
+    Regardless of whether `exclude_current_positions_from_observation` is set to `True` or `False`, the x- and y-coordinates are returned in `info` with the keys `"x_position"` and `"y_position"`, respectively.
 
-    | Num | Observation                                                                                                     | Min  | Max | Name (in corresponding XML file) | Joint | Unit                       |
+    By default, however, the observation space is a `Box(-Inf, Inf, (348,), float64)`, where the position and velocity elements are as follows:
+
+    | Num | Observation                                                                                                     | Min  | Max | Name (in corresponding XML file) | Joint | Type (Unit)                |
     | --- | --------------------------------------------------------------------------------------------------------------- | ---- | --- | -------------------------------- | ----- | -------------------------- |
     | 0   | z-coordinate of the torso (centre)                                                                              | -Inf | Inf | root                             | free  | position (m)               |
     | 1   | x-orientation of the torso (centre)                                                                             | -Inf | Inf | root                             | free  | angle (rad)                |
     | 2   | y-orientation of the torso (centre)                                                                             | -Inf | Inf | root                             | free  | angle (rad)                |
     | 3   | z-orientation of the torso (centre)                                                                             | -Inf | Inf | root                             | free  | angle (rad)                |
     | 4   | w-orientation of the torso (centre)                                                                             | -Inf | Inf | root                             | free  | angle (rad)                |
     | 5   | z-angle of the abdomen (in lower_waist)                                                                         | -Inf | Inf | abdomen_z                        | hinge | angle (rad)                |
@@ -89,278 +112,350 @@
     | 18  | angle between right upper arm and right_lower_arm                                                               | -Inf | Inf | right_elbow                      | hinge | angle (rad)                |
     | 19  | coordinate-1 (multi-axis) angle between torso and left arm (in left_upper_arm)                                  | -Inf | Inf | left_shoulder1                   | hinge | angle (rad)                |
     | 20  | coordinate-2 (multi-axis) angle between torso and left arm (in left_upper_arm)                                  | -Inf | Inf | left_shoulder2                   | hinge | angle (rad)                |
     | 21  | angle between left upper arm and left_lower_arm                                                                 | -Inf | Inf | left_elbow                       | hinge | angle (rad)                |
     | 22  | x-coordinate velocity of the torso (centre)                                                                     | -Inf | Inf | root                             | free  | velocity (m/s)             |
     | 23  | y-coordinate velocity of the torso (centre)                                                                     | -Inf | Inf | root                             | free  | velocity (m/s)             |
     | 24  | z-coordinate velocity of the torso (centre)                                                                     | -Inf | Inf | root                             | free  | velocity (m/s)             |
-    | 25  | x-coordinate angular velocity of the torso (centre)                                                             | -Inf | Inf | root                             | free  | anglular velocity (rad/s)  |
-    | 26  | y-coordinate angular velocity of the torso (centre)                                                             | -Inf | Inf | root                             | free  | anglular velocity (rad/s)  |
-    | 27  | z-coordinate angular velocity of the torso (centre)                                                             | -Inf | Inf | root                             | free  | anglular velocity (rad/s)  |
-    | 28  | z-coordinate of angular velocity of the abdomen (in lower_waist)                                                | -Inf | Inf | abdomen_z                        | hinge | anglular velocity (rad/s)  |
-    | 29  | y-coordinate of angular velocity of the abdomen (in lower_waist)                                                | -Inf | Inf | abdomen_y                        | hinge | anglular velocity (rad/s)  |
-    | 30  | x-coordinate of angular velocity of the abdomen (in pelvis)                                                     | -Inf | Inf | abdomen_x                        | hinge | aanglular velocity (rad/s) |
-    | 31  | x-coordinate of the angular velocity of the angle between pelvis and right hip (in right_thigh)                 | -Inf | Inf | right_hip_x                      | hinge | anglular velocity (rad/s)  |
-    | 32  | z-coordinate of the angular velocity of the angle between pelvis and right hip (in right_thigh)                 | -Inf | Inf | right_hip_z                      | hinge | anglular velocity (rad/s)  |
-    | 33  | y-coordinate of the angular velocity of the angle between pelvis and right hip (in right_thigh)                 | -Inf | Inf | right_hip_y                      | hinge | anglular velocity (rad/s)  |
-    | 34  | angular velocity of the angle between right hip and the right shin (in right_knee)                              | -Inf | Inf | right_knee                       | hinge | anglular velocity (rad/s)  |
-    | 35  | x-coordinate of the angular velocity of the angle between pelvis and left hip (in left_thigh)                   | -Inf | Inf | left_hip_x                       | hinge | anglular velocity (rad/s)  |
-    | 36  | z-coordinate of the angular velocity of the angle between pelvis and left hip (in left_thigh)                   | -Inf | Inf | left_hip_z                       | hinge | anglular velocity (rad/s)  |
-    | 37  | y-coordinate of the angular velocity of the angle between pelvis and left hip (in left_thigh)                   | -Inf | Inf | left_hip_y                       | hinge | anglular velocity (rad/s)  |
-    | 38  | angular velocity of the angle between left hip and the left shin (in left_knee)                                 | -Inf | Inf | left_knee                        | hinge | anglular velocity (rad/s)  |
-    | 39  | coordinate-1 (multi-axis) of the angular velocity of the angle between torso and right arm (in right_upper_arm) | -Inf | Inf | right_shoulder1                  | hinge | anglular velocity (rad/s)  |
-    | 40  | coordinate-2 (multi-axis) of the angular velocity of the angle between torso and right arm (in right_upper_arm) | -Inf | Inf | right_shoulder2                  | hinge | anglular velocity (rad/s)  |
-    | 41  | angular velocity of the angle between right upper arm and right_lower_arm                                       | -Inf | Inf | right_elbow                      | hinge | anglular velocity (rad/s)  |
-    | 42  | coordinate-1 (multi-axis) of the angular velocity of the angle between torso and left arm (in left_upper_arm)   | -Inf | Inf | left_shoulder1                   | hinge | anglular velocity (rad/s)  |
-    | 43  | coordinate-2 (multi-axis) of the angular velocity of the angle between torso and left arm (in left_upper_arm)   | -Inf | Inf | left_shoulder2                   | hinge | anglular velocity (rad/s)  |
-    | 44  | angular velocity of the angle between left upper arm and left_lower_arm                                         | -Inf | Inf | left_elbow                       | hinge | anglular velocity (rad/s)  |
+    | 25  | x-coordinate angular velocity of the torso (centre)                                                             | -Inf | Inf | root                             | free  | angular velocity (rad/s)   |
+    | 26  | y-coordinate angular velocity of the torso (centre)                                                             | -Inf | Inf | root                             | free  | angular velocity (rad/s)   |
+    | 27  | z-coordinate angular velocity of the torso (centre)                                                             | -Inf | Inf | root                             | free  | angular velocity (rad/s)   |
+    | 28  | z-coordinate of angular velocity of the abdomen (in lower_waist)                                                | -Inf | Inf | abdomen_z                        | hinge | angular velocity (rad/s)   |
+    | 29  | y-coordinate of angular velocity of the abdomen (in lower_waist)                                                | -Inf | Inf | abdomen_y                        | hinge | angular velocity (rad/s)   |
+    | 30  | x-coordinate of angular velocity of the abdomen (in pelvis)                                                     | -Inf | Inf | abdomen_x                        | hinge | angular velocity (rad/s)   |
+    | 31  | x-coordinate of the angular velocity of the angle between pelvis and right hip (in right_thigh)                 | -Inf | Inf | right_hip_x                      | hinge | angular velocity (rad/s)   |
+    | 32  | z-coordinate of the angular velocity of the angle between pelvis and right hip (in right_thigh)                 | -Inf | Inf | right_hip_z                      | hinge | angular velocity (rad/s)   |
+    | 33  | y-coordinate of the angular velocity of the angle between pelvis and right hip (in right_thigh)                 | -Inf | Inf | right_hip_y                      | hinge | angular velocity (rad/s)   |
+    | 34  | angular velocity of the angle between right hip and the right shin (in right_knee)                              | -Inf | Inf | right_knee                       | hinge | angular velocity (rad/s)   |
+    | 35  | x-coordinate of the angular velocity of the angle between pelvis and left hip (in left_thigh)                   | -Inf | Inf | left_hip_x                       | hinge | angular velocity (rad/s)   |
+    | 36  | z-coordinate of the angular velocity of the angle between pelvis and left hip (in left_thigh)                   | -Inf | Inf | left_hip_z                       | hinge | angular velocity (rad/s)   |
+    | 37  | y-coordinate of the angular velocity of the angle between pelvis and left hip (in left_thigh)                   | -Inf | Inf | left_hip_y                       | hinge | angular velocity (rad/s)   |
+    | 38  | angular velocity of the angle between left hip and the left shin (in left_knee)                                 | -Inf | Inf | left_knee                        | hinge | angular velocity (rad/s)   |
+    | 39  | coordinate-1 (multi-axis) of the angular velocity of the angle between torso and right arm (in right_upper_arm) | -Inf | Inf | right_shoulder1                  | hinge | angular velocity (rad/s)   |
+    | 40  | coordinate-2 (multi-axis) of the angular velocity of the angle between torso and right arm (in right_upper_arm) | -Inf | Inf | right_shoulder2                  | hinge | angular velocity (rad/s)   |
+    | 41  | angular velocity of the angle between right upper arm and right_lower_arm                                       | -Inf | Inf | right_elbow                      | hinge | angular velocity (rad/s)   |
+    | 42  | coordinate-1 (multi-axis) of the angular velocity of the angle between torso and left arm (in left_upper_arm)   | -Inf | Inf | left_shoulder1                   | hinge | angular velocity (rad/s)   |
+    | 43  | coordinate-2 (multi-axis) of the angular velocity of the angle between torso and left arm (in left_upper_arm)   | -Inf | Inf | left_shoulder2                   | hinge | angular velocity (rad/s)   |
+    | 44  | angular velocity of the angle between left upper arm and left_lower_arm                                         | -Inf | Inf | left_elbow                       | hinge | angular velocity (rad/s)   |
     | excluded | x-coordinate of the torso (centre)                                                                         | -Inf | Inf | root                             | free  | position (m)               |
     | excluded | y-coordinate of the torso (centre)                                                                         | -Inf | Inf | root                             | free  | position (m)               |
 
-    Additionally, after all the positional and velocity based values in the table,
-    the observation contains (in order):
-    - *cinert:* Mass and inertia of a single rigid body relative to the center of mass
-    (this is an intermediate result of transition). It has shape 14*10 (*nbody * 10*)
-    and hence adds to another 140 elements in the state space.
-    - *cvel:* Center of mass based velocity. It has shape 14 * 6 (*nbody * 6*) and hence
-    adds another 84 elements in the state space
-    - *qfrc_actuator:* Constraint force generated as the actuator force. This has shape
-    `(23,)`  *(nv * 1)* and hence adds another 23 elements to the state space.
-    - *cfrc_ext:* This is the center of mass based external force on the body.  It has shape
-    14 * 6 (*nbody * 6*) and hence adds to another 84 elements in the state space.
-    where *nbody* stands for the number of bodies in the robot and *nv* stands for the
-    number of degrees of freedom (*= dim(qvel)*)
-
     The body parts are:
 
-    | id (for `v2`,`v3`,`v4`) | body part |
-    | --- |  ------------  |
-    | 0   | worldBody (note: all values are constant 0) |
-    | 1   | torso |
-    | 2   | lwaist |
-    | 3   | pelvis |
-    | 4   | right_thigh |
-    | 5   | right_sin |
-    | 6   | right_foot |
-    | 7   | left_thigh |
-    | 8   | left_sin |
-    | 9   | left_foot |
-    | 10  | right_upper_arm |
-    | 11  | right_lower_arm |
-    | 12  | left_upper_arm |
-    | 13  | left_lower_arm |
+    | body part       | id (for `v2`, `v3`, `v4)` | id (for `v5`) |
+    |  -------------  |  ---   |  ---  |
+    | worldbody (note: all values are constant 0) | 0  |excluded|
+    | torso           |1  | 0      |
+    | lwaist          |2  | 1      |
+    | pelvis          |3  | 2      |
+    | right_thigh     |4  | 3      |
+    | right_sin       |5  | 4      |
+    | right_foot      |6  | 5      |
+    | left_thigh      |7  | 6      |
+    | left_sin        |8  | 7      |
+    | left_foot       |9  | 8      |
+    | right_upper_arm |10 | 9      |
+    | right_lower_arm |11 | 10     |
+    | left_upper_arm  |12 | 11     |
+    | left_lower_arm  |13 | 12     |
 
     The joints are:
 
-    | id (for `v2`,`v3`,`v4`) | joint |
-    | --- |  ------------  |
-    | 0   | root |
-    | 1   | root |
-    | 2   | root |
-    | 3   | root |
-    | 4   | root |
-    | 5   | root |
-    | 6   | abdomen_z |
-    | 7   | abdomen_y |
-    | 8   | abdomen_x |
-    | 9   | right_hip_x |
-    | 10  | right_hip_z |
-    | 11  | right_hip_y |
-    | 12  | right_knee |
-    | 13  | left_hip_x |
-    | 14  | left_hiz_z |
-    | 15  | left_hip_y |
-    | 16  | left_knee |
-    | 17  | right_shoulder1 |
-    | 18  | right_shoulder2 |
-    | 19  | right_elbow|
-    | 20  | left_shoulder1 |
-    | 21  | left_shoulder2 |
-    | 22  | left_elfbow |
-
-    The (x,y,z) coordinates are translational DOFs while the orientations are rotational
-    DOFs expressed as quaternions. One can read more about free joints on the
-    [Mujoco Documentation](https://mujoco.readthedocs.io/en/latest/XMLreference.html).
-
-    **Note:** Humanoid-v4 environment no longer has the following contact forces issue.
-    If using previous Humanoid versions from v4, there have been reported issues that using a Mujoco-Py version > 2.0
-    results in the contact forces always being 0. As such we recommend to use a Mujoco-Py
-    version < 2.0 when using the Humanoid environment if you would like to report results
-    with contact forces (if contact forces are not used in your experiments, you can use
-    version > 2.0).
+    | joint           | id (for `v2`, `v3`, `v4)` | id (for `v5`) |
+    |  -------------  |  ---   |  ---  |
+    | root (note: all values are constant 0) | 0  |excluded|
+    | root (note: all values are constant 0) | 1  |excluded|
+    | root (note: all values are constant 0) | 2  |excluded|
+    | root (note: all values are constant 0) | 3  |excluded|
+    | root (note: all values are constant 0) | 4  |excluded|
+    | root (note: all values are constant 0) | 5  |excluded|
+    | abdomen_z       | 6  | 0      |
+    | abdomen_y       | 7  | 1      |
+    | abdomen_x       | 8  | 2      |
+    | right_hip_x     | 9  | 3      |
+    | right_hip_z     | 10 | 4      |
+    | right_hip_y     | 11 | 5      |
+    | right_knee      | 12 | 6      |
+    | left_hip_x      | 13 | 7      |
+    | left_hiz_z      | 14 | 8      |
+    | left_hip_y      | 15 | 9      |
+    | left_knee       | 16 | 10     |
+    | right_shoulder1 | 17 | 11     |
+    | right_shoulder2 | 18 | 12     |
+    | right_elbow     | 19 | 13     |
+    | left_shoulder1  | 20 | 14     |
+    | left_shoulder2  | 21 | 15     |
+    | left_elfbow     | 22 | 16     |
+
+    The (x,y,z) coordinates are translational DOFs, while the orientations are rotational DOFs expressed as quaternions.
+    One can read more about free joints in the [MuJoCo documentation](https://mujoco.readthedocs.io/en/latest/XMLreference.html).
+
+    **Note:**
+    When using Humanoid-v3 or earlier versions, problems have been reported when using a `mujoco-py` version > 2.0, resulting in  contact forces always being 0.
+    Therefore, it is recommended to use a `mujoco-py` version < 2.0 when using the Humanoid environment if you want to report results with contact forces (if contact forces are not used in your experiments, you can use version > 2.0).
+
 
     ## Rewards
-    The reward consists of three parts:
-    - *healthy_reward*: Every timestep that the humanoid is alive (see section Episode Termination for definition), it gets a reward of fixed value `healthy_reward`
-    - *forward_reward*: A reward of walking forward which is measured as *`forward_reward_weight` *
-    (average center of mass before action - average center of mass after action)/dt*.
-    *dt* is the time between actions and is dependent on the frame_skip parameter
-    (default is 5), where the frametime is 0.003 - making the default *dt = 5 * 0.003 = 0.015*.
-    This reward would be positive if the humanoid walks forward (in positive x-direction). The calculation
-    for the center of mass is defined in the `.py` file for the Humanoid.
-    - *ctrl_cost*: A negative reward for penalising the humanoid if it has too
-    large of a control force. If there are *nu* actuators/controls, then the control has
-    shape  `nu x 1`. It is measured as *`ctrl_cost_weight` * sum(control<sup>2</sup>)*.
-    - *contact_cost*: A negative reward for penalising the humanoid if the external
-    contact force is too large. It is calculated by clipping
-    *`contact_cost_weight` * sum(external contact force<sup>2</sup>)* to the interval specified by `contact_cost_range`.
+    The total reward is: ***reward*** *=* *healthy_reward + forward_reward - ctrl_cost - contact_cost*.
+
+    - *healthy_reward*:
+    Every timestep that the Humanoid is alive (see definition in section "Episode End"),
+    it gets a reward of fixed value `healthy_reward` (default is $5$).
+    - *forward_reward*:
+    A reward for moving forward,
+    this reward would be positive if the Humanoid moves forward (in the positive $x$ direction / in the right direction).
+    $w_{forward} \times \frac{dx}{dt}$, where
+    $dx$ is the displacement of the center of mass ($x_{after-action} - x_{before-action}$),
+    $dt$ is the time between actions, which depends on the `frame_skip` parameter (default is $5$),
+    and `frametime` which is $0.001$ - so the default is $dt = 5 \times 0.003 = 0.015$,
+    $w_{forward}$ is the `forward_reward_weight` (default is $1.25$).
+    - *ctrl_cost*:
+    A negative reward to penalize the Humanoid for taking actions that are too large.
+    $w_{control} \times \|action\|_2^2$,
+    where $w_{control}$ is `ctrl_cost_weight` (default is $0.1$).
+    - *contact_cost*:
+    A negative reward to penalize the Humanoid if the external contact forces are too large.
+    $w_{contact} \times clamp(contact\_cost\_range, \|F_{contact}\|_2^2)$, where
+    $w_{contact}$ is `contact_cost_weight` (default is $5\times10^{-7}$),
+    $F_{contact}$ are the external contact forces (see `cfrc_ext` section on observation).
+
+    `info` contains the individual reward terms.
+
+    **Note:** There is a bug in the `Humanoid-v4` environment that causes *contact_cost* to always be 0.
 
-    The total reward returned is ***reward*** *=* *healthy_reward + forward_reward - ctrl_cost - contact_cost* and `info` will also contain the individual reward terms
 
     ## Starting State
-    All observations start in state
-    (0.0, 0.0,  1.4, 1.0, 0.0  ... 0.0) with a uniform noise in the range
-    of [-`reset_noise_scale`, `reset_noise_scale`] added to the positional and velocity values (values in the table)
-    for stochasticity. Note that the initial z coordinate is intentionally
-    selected to be high, thereby indicating a standing up humanoid. The initial
-    orientation is designed to make it face forward as well.
+    The initial position state is $[0.0, 0.0, 1.4, 1.0, 0.0, ... 0.0] + \mathcal{U}_{[-reset\_noise\_scale \times I_{24}, reset\_noise\_scale \times I_{24}]}$.
+    The initial velocity state is $\mathcal{U}_{[-reset\_noise\_scale \times I_{23}, reset\_noise\_scale \times I_{23}]}$.
 
-    ## Episode End
-    The humanoid is said to be unhealthy if the z-position of the torso is no longer contained in the
-    closed interval specified by the argument `healthy_z_range`.
+    where $\mathcal{U}$ is the multivariate uniform continuous distribution.
 
-    If `terminate_when_unhealthy=True` is passed during construction (which is the default),
-    the episode ends when any of the following happens:
+    Note that the z- and x-coordinates are non-zero so that the humanoid can immediately stand up and face forward (x-axis).
 
-    1. Truncation: The episode duration reaches a 1000 timesteps
-    3. Termination: The humanoid is unhealthy
 
-    If `terminate_when_unhealthy=False` is passed, the episode is ended only when 1000 timesteps are exceeded.
+    ## Episode End
+    ### Termination
+    If `terminate_when_unhealthy is True` (the default), the environment terminates when the Humanoid is unhealthy.
+    The Humanoid is said to be unhealthy if any of the following happens:
 
-    ## Arguments
+    1. The z-coordinate of the torso (the height) is **not** in the closed interval given by the `healthy_z_range` argument (default is $[1.0, 2.0]$).
 
-    No additional arguments are currently supported in v2 and lower.
+    ### Truncation
+    The default duration of an episode is 1000 timesteps.
 
-    ```python
-    import gymnasium as gym
-    env = gym.make('Humanoid-v4')
-    ```
 
-    v3 and v4 take `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc.
+    ## Arguments
+    Humanoid provides a range of parameters to modify the observation space, reward function, initial state, and termination condition.
+    These parameters can be applied during `gymnasium.make` in the following way:
 
     ```python
     import gymnasium as gym
-    env = gym.make('Humanoid-v4', ctrl_cost_weight=0.1, ....)
+    env = gym.make('Humanoid-v5', ctrl_cost_weight=0.1, ....)
     ```
 
-    | Parameter                                    | Type      | Default          | Description                                                                                                                                                               |
-    | -------------------------------------------- | --------- | ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-    | `xml_file`                                   | **str**   | `"humanoid.xml"` | Path to a MuJoCo model                                                                                                                                                    |
-    | `forward_reward_weight`                      | **float** | `1.25`           | Weight for _forward_reward_ term (see section on reward)                                                                                                                  |
-    | `ctrl_cost_weight`                           | **float** | `0.1`            | Weight for _ctrl_cost_ term (see section on reward)                                                                                                                       |
-    | `contact_cost_weight`                        | **float** | `5e-7`           | Weight for _contact_cost_ term (see section on reward)                                                                                                                    |
-    | `healthy_reward`                             | **float** | `5.0`            | Constant reward given if the humanoid is "healthy" after timestep                                                                                                         |
-    | `terminate_when_unhealthy`                   | **bool**  | `True`           | If true, issue a done signal if the z-coordinate of the torso is no longer in the `healthy_z_range`                                                                       |
-    | `healthy_z_range`                            | **tuple** | `(1.0, 2.0)`     | The humanoid is considered healthy if the z-coordinate of the torso is in this range                                                                                      |
-    | `reset_noise_scale`                          | **float** | `1e-2`           | Scale of random perturbations of initial position and velocity (see section on Starting State)                                                                            |
-    | `exclude_current_positions_from_observation` | **bool**  | `True`           | Whether or not to omit the x- and y-coordinates from observations. Excluding the position can serve as an inductive bias to induce position-agnostic behavior in policies |
+    | Parameter                                    | Type      | Default          | Description                                                                                                                                                                                                 |
+    | -------------------------------------------- | --------- | ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+    | `xml_file`                                   | **str**   | `"humanoid.xml"` | Path to a MuJoCo model                                                                                                                                                                                      |
+    | `forward_reward_weight`                      | **float** | `1.25`           | Weight for _forward_reward_ term (see `Rewards` section)                                                                                                                                                    |
+    | `ctrl_cost_weight`                           | **float** | `0.1`            | Weight for _ctrl_cost_ term (see `Rewards` section)                                                                                                                                                         |
+    | `contact_cost_weight`                        | **float** | `5e-7`           | Weight for _contact_cost_ term (see `Rewards` section)                                                                                                                                                      |
+    | `contact_cost_range`                         | **float** | `(-np.inf, 10.0)`| Clamps the _contact_cost_ term (see `Rewards` section)                                                                                                                                                      |
+    | `healthy_reward`                             | **float** | `5.0`            | Weight for _healthy_reward_ term (see `Rewards` section)                                                                                                                                                    |
+    | `terminate_when_unhealthy`                   | **bool**  | `True`           | If `True`, issue a `terminated` signal is unhealthy (see `Episode End` section)                                                                                                                                |
+    | `healthy_z_range`                            | **tuple** | `(1.0, 2.0)`     | The humanoid is considered healthy if the z-coordinate of the torso is in this range (see `Episode End` section)                                                                                            |
+    | `reset_noise_scale`                          | **float** | `1e-2`           | Scale of random perturbations of initial position and velocity (see `Starting State` section)                                                                                                               |
+    | `exclude_current_positions_from_observation` | **bool**  | `True`           | Whether or not to omit the x- and y-coordinates from observations. Excluding the position can serve as an inductive bias to induce position-agnostic behavior in policies (see `Observation State` section) |
+    | `include_cinert_in_observation`              | **bool**  | `True`           | Whether to include *cinert* elements in the observations (see `Observation State` section)                                                                                                                  |
+    | `include_cvel_in_observation`                | **bool**  | `True`           | Whether to include *cvel* elements in the observations (see `Observation State` section)                                                                                                                    |
+    | `include_qfrc_actuator_in_observation`       | **bool**  | `True`           | Whether to include *qfrc_actuator* elements in the observations (see `Observation State` section)                                                                                                           |
+    | `include_cfrc_ext_in_observation`            | **bool**  | `True`           | Whether to include *cfrc_ext* elements in the observations (see `Observation State` section)                                                                                                                |
 
     ## Version History
-
+    * v5:
+        - Minimum `mujoco` version is now 2.3.3.
+        - Added support for fully custom/third party `mujoco` models using the `xml_file` argument (previously only a few changes could be made to the existing models).
+        - Added `default_camera_config` argument, a dictionary for setting the `mj_camera` properties, mainly useful for custom environments.
+        - Added `env.observation_structure`, a dictionary for specifying the observation space compose (e.g. `qpos`, `qvel`), useful for building tooling and wrappers for the MuJoCo environments.
+        - Return a non-empty `info` with `reset()`, previously an empty dictionary was returned, the new keys are the same state information as `step()`.
+        - Added `frame_skip` argument, used to configure the `dt` (duration of `step()`), default varies by environment check environment documentation pages.
+        - Fixed bug: `healthy_reward` was given on every step (even if the Humanoid was unhealthy), now it is only given when the Humanoid is healthy. The `info["reward_survive"]` is updated with this change (related [GitHub issue](https://github.com/Farama-Foundation/Gymnasium/issues/526)).
+        - Restored `contact_cost` and the corresponding `contact_cost_weight` and `contact_cost_range` arguments, with the same defaults as in `Humanoid-v3` (was removed in `v4`) (related [GitHub issue](https://github.com/Farama-Foundation/Gymnasium/issues/504)).
+        - Excluded the `cinert` & `cvel` & `cfrc_ext` of `worldbody` and `root`/`freejoint` `qfrc_actuator` from the observation space, as it was always 0 and thus provided no useful information to the agent, resulting in slightly faster training (related [GitHub issue](https://github.com/Farama-Foundation/Gymnasium/issues/204)).
+        - Restored the `xml_file` argument (was removed in `v4`).
+        - Added `include_cinert_in_observation`, `include_cvel_in_observation`, `include_qfrc_actuator_in_observation`, `include_cfrc_ext_in_observation` arguments to allow for the exclusion of observation elements from the observation space.
+        - Fixed `info["x_position"]` & `info["y_position"]` & `info["distance_from_origin"]` returning `xpos` instead of `qpos` based observations (`xpos` observations are behind 1 `mj_step()` more [here](https://github.com/deepmind/mujoco/issues/889#issuecomment-1568896388)) (related [GitHub issue #1](https://github.com/Farama-Foundation/Gymnasium/issues/521) & [GitHub issue #2](https://github.com/Farama-Foundation/Gymnasium/issues/539)).
+        - Added `info["tendon_length"]` and `info["tendon_velocity"]` containing observations of the Humanoid's 2 tendons connecting the hips to the knees.
+        - Renamed `info["reward_alive"]` to `info["reward_survive"]` to be consistent with the other environments.
+        - Renamed `info["reward_linvel"]` to `info["reward_forward"]` to be consistent with the other environments.
+        - Renamed `info["reward_quadctrl"]` to `info["reward_ctrl"]` to be consistent with the other environments.
+        - Removed `info["forward_reward"]` as it is equivalent to `info["reward_forward"]`.
     * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3
     * v3: Support for `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc. rgb rendering comes from tracking camera (so agent does not run away from screen)
     * v2: All continuous control environments now use mujoco-py >= 1.50
     * v1: max_time_steps raised to 1000 for robot based tasks. Added reward_threshold to environments.
-    * v0: Initial versions release (1.0.0)
+    * v0: Initial versions release
     """
 
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
-        "render_fps": 67,
     }
 
     def __init__(
         self,
-        forward_reward_weight=1.25,
-        ctrl_cost_weight=0.1,
-        healthy_reward=5.0,
-        terminate_when_unhealthy=True,
-        healthy_z_range=(1.0, 2.0),
-        reset_noise_scale=1e-2,
-        exclude_current_positions_from_observation=True,
+        xml_file: str = "humanoid.xml",
+        frame_skip: int = 5,
+        default_camera_config: Dict[str, Union[float, int]] = DEFAULT_CAMERA_CONFIG,
+        forward_reward_weight: float = 1.25,
+        ctrl_cost_weight: float = 0.1,
+        contact_cost_weight: float = 5e-7,
+        contact_cost_range: Tuple[float, float] = (-np.inf, 10.0),
+        healthy_reward: float = 5.0,
+        terminate_when_unhealthy: bool = True,
+        healthy_z_range: Tuple[float, float] = (1.0, 2.0),
+        reset_noise_scale: float = 1e-2,
+        exclude_current_positions_from_observation: bool = True,
+        include_cinert_in_observation: bool = True,
+        include_cvel_in_observation: bool = True,
+        include_qfrc_actuator_in_observation: bool = True,
+        include_cfrc_ext_in_observation: bool = True,
         **kwargs,
     ):
         utils.EzPickle.__init__(
             self,
+            xml_file,
+            frame_skip,
+            default_camera_config,
             forward_reward_weight,
             ctrl_cost_weight,
+            contact_cost_weight,
+            contact_cost_range,
             healthy_reward,
             terminate_when_unhealthy,
             healthy_z_range,
             reset_noise_scale,
             exclude_current_positions_from_observation,
+            include_cinert_in_observation,
+            include_cvel_in_observation,
+            include_qfrc_actuator_in_observation,
+            include_cfrc_ext_in_observation,
             **kwargs,
         )
 
         self._forward_reward_weight = forward_reward_weight
         self._ctrl_cost_weight = ctrl_cost_weight
+        self._contact_cost_weight = contact_cost_weight
+        self._contact_cost_range = contact_cost_range
         self._healthy_reward = healthy_reward
         self._terminate_when_unhealthy = terminate_when_unhealthy
         self._healthy_z_range = healthy_z_range
 
         self._reset_noise_scale = reset_noise_scale
 
         self._exclude_current_positions_from_observation = (
             exclude_current_positions_from_observation
         )
 
-        if exclude_current_positions_from_observation:
-            observation_space = Box(
-                low=-np.inf, high=np.inf, shape=(376,), dtype=np.float64
-            )
-        else:
-            observation_space = Box(
-                low=-np.inf, high=np.inf, shape=(378,), dtype=np.float64
-            )
+        self._include_cinert_in_observation = include_cinert_in_observation
+        self._include_cvel_in_observation = include_cvel_in_observation
+        self._include_qfrc_actuator_in_observation = (
+            include_qfrc_actuator_in_observation
+        )
+        self._include_cfrc_ext_in_observation = include_cfrc_ext_in_observation
 
         MujocoEnv.__init__(
             self,
-            "humanoid.xml",
-            5,
-            observation_space=observation_space,
-            default_camera_config=DEFAULT_CAMERA_CONFIG,
+            xml_file,
+            frame_skip,
+            observation_space=None,
+            default_camera_config=default_camera_config,
             **kwargs,
         )
 
+        self.metadata = {
+            "render_modes": [
+                "human",
+                "rgb_array",
+                "depth_array",
+            ],
+            "render_fps": int(np.round(1.0 / self.dt)),
+        }
+
+        obs_size = self.data.qpos.size + self.data.qvel.size
+        obs_size -= 2 * exclude_current_positions_from_observation
+        obs_size += self.data.cinert[1:].size * include_cinert_in_observation
+        obs_size += self.data.cvel[1:].size * include_cvel_in_observation
+        obs_size += (self.data.qvel.size - 6) * include_qfrc_actuator_in_observation
+        obs_size += self.data.cfrc_ext[1:].size * include_cfrc_ext_in_observation
+
+        self.observation_space = Box(
+            low=-np.inf, high=np.inf, shape=(obs_size,), dtype=np.float64
+        )
+
+        self.observation_structure = {
+            "skipped_qpos": 2 * exclude_current_positions_from_observation,
+            "qpos": self.data.qpos.size
+            - 2 * exclude_current_positions_from_observation,
+            "qvel": self.data.qvel.size,
+            "cinert": self.data.cinert[1:].size * include_cinert_in_observation,
+            "cvel": self.data.cvel[1:].size * include_cvel_in_observation,
+            "qfrc_actuator": (self.data.qvel.size - 6)
+            * include_qfrc_actuator_in_observation,
+            "cfrc_ext": self.data.cfrc_ext[1:].size * include_cfrc_ext_in_observation,
+            "ten_lenght": 0,
+            "ten_velocity": 0,
+        }
+
     @property
     def healthy_reward(self):
-        return (
-            float(self.is_healthy or self._terminate_when_unhealthy)
-            * self._healthy_reward
-        )
+        return self.is_healthy * self._healthy_reward
 
     def control_cost(self, action):
         control_cost = self._ctrl_cost_weight * np.sum(np.square(self.data.ctrl))
         return control_cost
 
     @property
+    def contact_cost(self):
+        contact_forces = self.data.cfrc_ext
+        contact_cost = self._contact_cost_weight * np.sum(np.square(contact_forces))
+        min_cost, max_cost = self._contact_cost_range
+        contact_cost = np.clip(contact_cost, min_cost, max_cost)
+        return contact_cost
+
+    @property
     def is_healthy(self):
         min_z, max_z = self._healthy_z_range
         is_healthy = min_z < self.data.qpos[2] < max_z
 
         return is_healthy
 
-    @property
-    def terminated(self):
-        terminated = (not self.is_healthy) if self._terminate_when_unhealthy else False
-        return terminated
-
     def _get_obs(self):
-        position = self.data.qpos.flat.copy()
-        velocity = self.data.qvel.flat.copy()
+        position = self.data.qpos.flatten()
+        velocity = self.data.qvel.flatten()
 
-        com_inertia = self.data.cinert.flat.copy()
-        com_velocity = self.data.cvel.flat.copy()
+        if self._include_cinert_in_observation is True:
+            com_inertia = self.data.cinert[1:].flatten()
+        else:
+            com_inertia = np.array([])
+        if self._include_cvel_in_observation is True:
+            com_velocity = self.data.cvel[1:].flatten()
+        else:
+            com_velocity = np.array([])
 
-        actuator_forces = self.data.qfrc_actuator.flat.copy()
-        external_contact_forces = self.data.cfrc_ext.flat.copy()
+        if self._include_qfrc_actuator_in_observation is True:
+            actuator_forces = self.data.qfrc_actuator[6:].flatten()
+        else:
+            actuator_forces = np.array([])
+        if self._include_cfrc_ext_in_observation is True:
+            external_contact_forces = self.data.cfrc_ext[1:].flatten()
+        else:
+            external_contact_forces = np.array([])
 
         if self._exclude_current_positions_from_observation:
             position = position[2:]
 
         return np.concatenate(
             (
                 position,
@@ -376,47 +471,69 @@
         xy_position_before = mass_center(self.model, self.data)
         self.do_simulation(action, self.frame_skip)
         xy_position_after = mass_center(self.model, self.data)
 
         xy_velocity = (xy_position_after - xy_position_before) / self.dt
         x_velocity, y_velocity = xy_velocity
 
-        ctrl_cost = self.control_cost(action)
-
-        forward_reward = self._forward_reward_weight * x_velocity
-        healthy_reward = self.healthy_reward
-
-        rewards = forward_reward + healthy_reward
-
         observation = self._get_obs()
-        reward = rewards - ctrl_cost
-        terminated = self.terminated
+        reward, reward_info = self._get_rew(x_velocity, action)
+        terminated = (not self.is_healthy) and self._terminate_when_unhealthy
         info = {
-            "reward_linvel": forward_reward,
-            "reward_quadctrl": -ctrl_cost,
-            "reward_alive": healthy_reward,
-            "x_position": xy_position_after[0],
-            "y_position": xy_position_after[1],
-            "distance_from_origin": np.linalg.norm(xy_position_after, ord=2),
+            "x_position": self.data.qpos[0],
+            "y_position": self.data.qpos[1],
+            "tendon_lenght": self.data.ten_length,
+            "tendon_velocity": self.data.ten_velocity,
+            "distance_from_origin": np.linalg.norm(self.data.qpos[0:2], ord=2),
             "x_velocity": x_velocity,
             "y_velocity": y_velocity,
-            "forward_reward": forward_reward,
+            **reward_info,
         }
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return observation, reward, terminated, False, info
 
+    def _get_rew(self, x_velocity: float, action):
+        forward_reward = self._forward_reward_weight * x_velocity
+        healthy_reward = self.healthy_reward
+        rewards = forward_reward + healthy_reward
+
+        ctrl_cost = self.control_cost(action)
+        contact_cost = self.contact_cost
+        costs = ctrl_cost + contact_cost
+
+        reward = rewards - costs
+
+        reward_info = {
+            "reward_survive": healthy_reward,
+            "reward_forward": forward_reward,
+            "reward_ctrl": -ctrl_cost,
+            "reward_contact": -contact_cost,
+        }
+
+        return reward, reward_info
+
     def reset_model(self):
         noise_low = -self._reset_noise_scale
         noise_high = self._reset_noise_scale
 
         qpos = self.init_qpos + self.np_random.uniform(
             low=noise_low, high=noise_high, size=self.model.nq
         )
         qvel = self.init_qvel + self.np_random.uniform(
             low=noise_low, high=noise_high, size=self.model.nv
         )
         self.set_state(qpos, qvel)
 
         observation = self._get_obs()
         return observation
+
+    def _get_reset_info(self):
+        return {
+            "x_position": self.data.qpos[0],
+            "y_position": self.data.qpos[1],
+            "tendon_lenght": self.data.ten_length,
+            "tendon_velocity": self.data.ten_velocity,
+            "distance_from_origin": np.linalg.norm(self.data.qpos[0:2], ord=2),
+        }
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/humanoidstandup.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/humanoidstandup_v4.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,73 @@
 import numpy as np
 
 from gymnasium import utils
-from gymnasium.envs.mujoco import MuJocoPyEnv
+from gymnasium.envs.mujoco import MujocoEnv
 from gymnasium.spaces import Box
 
 
-class HumanoidStandupEnv(MuJocoPyEnv, utils.EzPickle):
+DEFAULT_CAMERA_CONFIG = {
+    "trackbodyid": 1,
+    "distance": 4.0,
+    "lookat": np.array((0.0, 0.0, 0.8925)),
+    "elevation": -20.0,
+}
+
+
+class HumanoidStandupEnv(MujocoEnv, utils.EzPickle):
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
         "render_fps": 67,
     }
 
     def __init__(self, **kwargs):
         observation_space = Box(
             low=-np.inf, high=np.inf, shape=(376,), dtype=np.float64
         )
-        MuJocoPyEnv.__init__(
+        MujocoEnv.__init__(
             self,
             "humanoidstandup.xml",
             5,
             observation_space=observation_space,
+            default_camera_config=DEFAULT_CAMERA_CONFIG,
             **kwargs,
         )
         utils.EzPickle.__init__(self, **kwargs)
 
     def _get_obs(self):
-        data = self.sim.data
+        data = self.data
         return np.concatenate(
             [
                 data.qpos.flat[2:],
                 data.qvel.flat,
                 data.cinert.flat,
                 data.cvel.flat,
                 data.qfrc_actuator.flat,
                 data.cfrc_ext.flat,
             ]
         )
 
     def step(self, a):
         self.do_simulation(a, self.frame_skip)
-        pos_after = self.sim.data.qpos[2]
-        data = self.sim.data
+        pos_after = self.data.qpos[2]
+        data = self.data
         uph_cost = (pos_after - 0) / self.model.opt.timestep
 
         quad_ctrl_cost = 0.1 * np.square(data.ctrl).sum()
         quad_impact_cost = 0.5e-6 * np.square(data.cfrc_ext).sum()
         quad_impact_cost = min(quad_impact_cost, 10)
         reward = uph_cost - quad_ctrl_cost - quad_impact_cost + 1
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return (
             self._get_obs(),
             reward,
             False,
             False,
             dict(
                 reward_linup=uph_cost,
@@ -74,14 +84,7 @@
             + self.np_random.uniform(
                 low=-c,
                 high=c,
                 size=self.model.nv,
             ),
         )
         return self._get_obs()
-
-    def viewer_setup(self):
-        assert self.viewer is not None
-        self.viewer.cam.trackbodyid = 1
-        self.viewer.cam.distance = self.model.stat.extent * 1.0
-        self.viewer.cam.lookat[2] = 0.8925
-        self.viewer.cam.elevation = -20
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/inverted_double_pendulum.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/inverted_double_pendulum.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         vel_penalty = 1e-3 * v1**2 + 5e-3 * v2**2
         alive_bonus = 10
         r = alive_bonus - dist_penalty - vel_penalty
         terminated = bool(y <= 1)
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return ob, r, terminated, False, {}
 
     def _get_obs(self):
         return np.concatenate(
             [
                 self.sim.data.qpos[:1],  # cart x pos
                 np.sin(self.sim.data.qpos[1:]),  # link angles
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/inverted_double_pendulum_v4.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/inverted_double_pendulum_v5.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+__credits__ = ["Kallinteris-Andreas"]
+
+from typing import Dict, Union
+
 import numpy as np
 
 from gymnasium import utils
 from gymnasium.envs.mujoco import MujocoEnv
 from gymnasium.spaces import Box
 
 
@@ -9,171 +13,223 @@
     "trackbodyid": 0,
     "distance": 4.1225,
     "lookat": np.array((0.0, 0.0, 0.12250000000000005)),
 }
 
 
 class InvertedDoublePendulumEnv(MujocoEnv, utils.EzPickle):
-    """
+    r"""
     ## Description
+    This environment originates from control theory and builds on the cartpole environment based on the work of Barto, Sutton, and Anderson in ["Neuronlike adaptive elements that can solve difficult learning control problems"](https://ieeexplore.ieee.org/document/6313077),
+    powered by the Mujoco physics simulator - allowing for more complex experiments (such as varying the effects of gravity or constraints).
+    This environment involves a cart that can be moved linearly, with one pole attached to it and a second pole attached to the other end of the first pole (leaving the second pole as the only one with a free end).
+    The cart can be pushed left or right, and the goal is to balance the second pole on top of the first pole, which is in turn on top of the cart, by applying continuous forces to the cart.
 
-    This environment originates from control theory and builds on the cartpole
-    environment based on the work done by Barto, Sutton, and Anderson in
-    ["Neuronlike adaptive elements that can solve difficult learning control problems"](https://ieeexplore.ieee.org/document/6313077),
-    powered by the Mujoco physics simulator - allowing for more complex experiments
-    (such as varying the effects of gravity or constraints). This environment involves a cart that can
-    moved linearly, with a pole fixed on it and a second pole fixed on the other end of the first one
-    (leaving the second pole as the only one with one free end). The cart can be pushed left or right,
-    and the goal is to balance the second pole on top of the first pole, which is in turn on top of the
-    cart, by applying continuous forces on the cart.
 
     ## Action Space
     The agent take a 1-element vector for actions.
     The action space is a continuous `(action)` in `[-1, 1]`, where `action` represents the
     numerical force applied to the cart (with magnitude representing the amount of force and
     sign representing the direction)
 
-    | Num | Action                    | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit      |
+    | Num | Action                    | Control Min | Control Max | Name (in corresponding XML file) | Joint |Type (Unit)|
     |-----|---------------------------|-------------|-------------|----------------------------------|-------|-----------|
     | 0   | Force applied on the cart | -1          | 1           | slider                           | slide | Force (N) |
 
+
     ## Observation Space
+    The observation space consists of the following parts (in order):
 
-    The state space consists of positional values of different body parts of the pendulum system,
-    followed by the velocities of those individual parts (their derivatives) with all the
-    positions ordered before all the velocities.
+    - *qpos (1 element):* Position values of the robot's cart.
+    - *sin(qpos) (2 elements):* The sine of the angles of poles.
+    - *cos(qpos) (2 elements):* The cosine of the angles of poles.
+    - *qvel (3 elements):* The velocities of these individual body parts (their derivatives).
+    - *qfrc_constraint (1 element):* Constraint force of the cart.
+    There is one constraint force for contacts for each degree of freedom (3).
+    The approach and handling of constraints by MuJoCo is unique to the simulator and is based on their research.
+    More information can be found  in their [*documentation*](https://mujoco.readthedocs.io/en/latest/computation.html) or in their paper ["Analytically-invertible dynamics with contacts and constraints: Theory and implementation in MuJoCo"](https://homes.cs.washington.edu/~todorov/papers/TodorovICRA14.pdf).
 
-    The observation is a `ndarray` with shape `(11,)` where the elements correspond to the following:
+    The observation space is a `Box(-Inf, Inf, (9,), float64)` where the elements are as follows:
 
-    | Num | Observation                                                       | Min  | Max | Name (in corresponding XML file) | Joint | Unit                     |
+    | Num | Observation                                                       | Min  | Max | Name (in corresponding XML file) | Joint | Type (Unit)              |
     | --- | ----------------------------------------------------------------- | ---- | --- | -------------------------------- | ----- | ------------------------ |
     | 0   | position of the cart along the linear surface                     | -Inf | Inf | slider                           | slide | position (m)             |
     | 1   | sine of the angle between the cart and the first pole             | -Inf | Inf | sin(hinge)                       | hinge | unitless                 |
     | 2   | sine of the angle between the two poles                           | -Inf | Inf | sin(hinge2)                      | hinge | unitless                 |
     | 3   | cosine of the angle between the cart and the first pole           | -Inf | Inf | cos(hinge)                       | hinge | unitless                 |
     | 4   | cosine of the angle between the two poles                         | -Inf | Inf | cos(hinge2)                      | hinge | unitless                 |
     | 5   | velocity of the cart                                              | -Inf | Inf | slider                           | slide | velocity (m/s)           |
     | 6   | angular velocity of the angle between the cart and the first pole | -Inf | Inf | hinge                            | hinge | angular velocity (rad/s) |
     | 7   | angular velocity of the angle between the two poles               | -Inf | Inf | hinge2                           | hinge | angular velocity (rad/s) |
-    | 8   | constraint force - 1                                              | -Inf | Inf |                                  |       | Force (N)                |
-    | 9   | constraint force - 2                                              | -Inf | Inf |                                  |       | Force (N)                |
-    | 10  | constraint force - 3                                              | -Inf | Inf |                                  |       | Force (N)                |
+    | 8   | constraint force - x                                              | -Inf | Inf | slider                           | slide | Force (N)                |
+    | excluded | constraint force - y                                         | -Inf | Inf | slider                           | slide | Force (N)                |
+    | excluded | constraint force - z                                         | -Inf | Inf | slider                           | slide | Force (N)                |
 
 
-    There is physical contact between the robots and their environment - and Mujoco
-    attempts at getting realistic physics simulations for the possible physical contact
-    dynamics by aiming for physical accuracy and computational efficiency.
+    ## Rewards
+    The total reward is: ***reward*** *=* *alive_bonus - distance_penalty - velocity_penalty*.
 
-    There is one constraint force for contacts for each degree of freedom (3).
-    The approach and handling of constraints by Mujoco is unique to the simulator
-    and is based on their research. Once can find more information in their
-    [*documentation*](https://mujoco.readthedocs.io/en/latest/computation.html)
-    or in their paper
-    ["Analytically-invertible dynamics with contacts and constraints: Theory and implementation in MuJoCo"](https://homes.cs.washington.edu/~todorov/papers/TodorovICRA14.pdf).
+    - *alive_bonus*:
+    Every timestep that the Inverted Pendulum is healthy (see definition in section "Episode End"),
+    it gets a reward of fixed value `healthy_reward` (default is $10$).
+    - *distance_penalty*:
+    This reward is a measure of how far the *tip* of the second pendulum (the only free end) moves,
+    and it is calculated as $0.01 x_{pole2-tip}^2 + (y_{pole2-tip}-2)^2$,
+    where $x_{pole2-tip}, y_{pole2-tip}$ are the xy-coordinatesof the tip of the second pole.
+    - *velocity_penalty*:
+    A negative reward to penalize the agent for moving too fast.
+    $10^{-3} \omega_1 + 5 \times 10^{-3} \omega_2$,
+    where $\omega_1, \omega_2$ are the angular velocities of the hinges.
 
+    `info` contains the individual reward terms.
 
-    ## Rewards
 
-    The reward consists of two parts:
-    - *alive_bonus*: The goal is to make the second inverted pendulum stand upright
-    (within a certain angle limit) as long as possible - as such a reward of +10 is awarded
-     for each timestep that the second pole is upright.
-    - *distance_penalty*: This reward is a measure of how far the *tip* of the second pendulum
-    (the only free end) moves, and it is calculated as
-    *0.01 * x<sup>2</sup> + (y - 2)<sup>2</sup>*, where *x* is the x-coordinate of the tip
-    and *y* is the y-coordinate of the tip of the second pole.
-    - *velocity_penalty*: A negative reward for penalising the agent if it moves too
-    fast *0.001 *  v<sub>1</sub><sup>2</sup> + 0.005 * v<sub>2</sub> <sup>2</sup>*
+    ## Starting State
+    The initial position state is $\mathcal{U}_{[-reset\_noise\_scale \times I_{3}, reset\_noise\_scale \times I_{3}]}$.
+    The initial velocity state is $\mathcal{N}(0_{3}, reset\_noise\_scale^2 \times I_{3})$.
 
-    The total reward returned is ***reward*** *=* *alive_bonus - distance_penalty - velocity_penalty*
+    where $\mathcal{N}$ is the multivariate normal distribution and $\mathcal{U}$ is the multivariate uniform continuous distribution.
 
-    ## Starting State
-    All observations start in state
-    (0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0) with a uniform noise in the range
-    of [-0.1, 0.1] added to the positional values (cart position and pole angles) and standard
-    normal force with a standard deviation of 0.1 added to the velocity values for stochasticity.
 
     ## Episode End
-    The episode ends when any of the following happens:
+    ### Termination
+    The environment terminates when the Inverted Double Pendulum is unhealthy.
+    The Inverted Double Pendulum is unhealthy if any of the following happens:
 
-    1.Truncation:  The episode duration reaches 1000 timesteps.
-    2.Termination: Any of the state space values is no longer finite.
-    3.Termination: The y_coordinate of the tip of the second pole *is less than or equal* to 1. The maximum standing height of the system is 1.196 m when all the parts are perpendicularly vertical on top of each other).
+    1.Termination: The y_coordinate of the tip of the second pole $\leq 1$.
 
-    ## Arguments
+    Note: The maximum standing height of the system is 1.2 m when all the parts are perpendicularly vertical on top of each other.
 
-    No additional arguments are currently supported.
+    ### Truncation
+    The default duration of an episode is 1000 timesteps.
 
-    ```python
-    import gymnasium as gym
-    env = gym.make('InvertedDoublePendulum-v4')
-    ```
-    There is no v3 for InvertedPendulum, unlike the robot environments where a v3 and
-    beyond take `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc.
+
+    ## Arguments
+    InvertedDoublePendulum provides a range of parameters to modify the observation space, reward function, initial state, and termination condition.
+    These parameters can be applied during `gymnasium.make` in the following way:
 
     ```python
     import gymnasium as gym
-    env = gym.make('InvertedDoublePendulum-v2')
+    env = gym.make('InvertedDoublePendulum-v5', healthy_reward=10, ...)
     ```
 
-    ## Version History
+    | Parameter               | Type       | Default                        | Description                                                                                   |
+    |-------------------------|------------|--------------------------------|-----------------------------------------------------------------------------------------------|
+    | `xml_file`              | **str**    |`"inverted_double_pendulum.xml"`| Path to a MuJoCo model                                                                        |
+    | `healthy_reward`        | **float**  | `10`                           | Constant reward given if the pendulum is `healthy` (upright) (see `Rewards` section)          |
+    | `reset_noise_scale`     | **float**  | `0.1`                          | Scale of random perturbations of initial position and velocity (see `Starting State` section) |
 
-    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3
-    * v3: Support for `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc. rgb rendering comes from tracking camera (so agent does not run away from screen)
-    * v2: All continuous control environments now use mujoco-py >= 1.50
-    * v1: max_time_steps raised to 1000 for robot based tasks (including inverted pendulum)
-    * v0: Initial versions release (1.0.0)
+    ## Version History
+    * v5:
+        - Minimum `mujoco` version is now 2.3.3.
+        - Added `default_camera_config` argument, a dictionary for setting the `mj_camera` properties, mainly useful for custom environments.
+        - Added `frame_skip` argument, used to configure the `dt` (duration of `step()`), default varies by environment check environment documentation pages.
+        - Fixed bug: `healthy_reward` was given on every step (even if the Pendulum is unhealthy), now it is only given if the DoublePendulum is healthy (not terminated)(related [GitHub issue](https://github.com/Farama-Foundation/Gymnasium/issues/500)).
+        - Excluded the `qfrc_constraint` ("constraint force") of the hinges from the observation space (as it was always 0, thus providing no useful information to the agent, resulting in slightly faster training) (related [GitHub issue](https://github.com/Farama-Foundation/Gymnasium/issues/228)).
+        - Added `xml_file` argument.
+        - Added `reset_noise_scale` argument to set the range of initial states.
+        - Added `healthy_reward` argument to configure the reward function (defaults are effectively the same as in `v4`).
+        - Added individual reward terms in `info` ( `info["reward_survive"]`, `info["distance_penalty"]`, `info["velocity_penalty"]`).
+    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3.
+    * v3: This environment does not have a v3 release.
+    * v2: All continuous control environments now use mujoco-py >= 1.50.
+    * v1: max_time_steps raised to 1000 for robot based tasks (including inverted pendulum).
+    * v0: Initial versions release.
     """
 
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
-        "render_fps": 20,
     }
 
-    def __init__(self, **kwargs):
-        observation_space = Box(low=-np.inf, high=np.inf, shape=(11,), dtype=np.float64)
+    def __init__(
+        self,
+        xml_file: str = "inverted_double_pendulum.xml",
+        frame_skip: int = 5,
+        default_camera_config: Dict[str, Union[float, int]] = {},
+        healthy_reward: float = 10.0,
+        reset_noise_scale: float = 0.1,
+        **kwargs,
+    ):
+        utils.EzPickle.__init__(self, xml_file, frame_skip, reset_noise_scale, **kwargs)
+
+        self._healthy_reward = healthy_reward
+        self._reset_noise_scale = reset_noise_scale
+
+        observation_space = Box(low=-np.inf, high=np.inf, shape=(9,), dtype=np.float64)
+
         MujocoEnv.__init__(
             self,
-            "inverted_double_pendulum.xml",
-            5,
+            xml_file,
+            frame_skip,
             observation_space=observation_space,
-            default_camera_config=DEFAULT_CAMERA_CONFIG,
+            default_camera_config=default_camera_config,
             **kwargs,
         )
-        utils.EzPickle.__init__(self, **kwargs)
+
+        self.metadata = {
+            "render_modes": [
+                "human",
+                "rgb_array",
+                "depth_array",
+            ],
+            "render_fps": int(np.round(1.0 / self.dt)),
+        }
 
     def step(self, action):
         self.do_simulation(action, self.frame_skip)
-        ob = self._get_obs()
+
         x, _, y = self.data.site_xpos[0]
-        dist_penalty = 0.01 * x**2 + (y - 2) ** 2
-        v1, v2 = self.data.qvel[1:3]
-        vel_penalty = 1e-3 * v1**2 + 5e-3 * v2**2
-        alive_bonus = 10
-        r = alive_bonus - dist_penalty - vel_penalty
+        observation = self._get_obs()
         terminated = bool(y <= 1)
+        reward, reward_info = self._get_rew(x, y, terminated)
+
+        info = reward_info
+
         if self.render_mode == "human":
             self.render()
-        return ob, r, terminated, False, {}
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
+        return observation, reward, terminated, False, info
+
+    def _get_rew(self, x, y, terminated):
+        v1, v2 = self.data.qvel[1:3]
+        dist_penalty = 0.01 * x**2 + (y - 2) ** 2
+        vel_penalty = 1e-3 * v1**2 + 5e-3 * v2**2
+        alive_bonus = self._healthy_reward * int(not terminated)
+
+        reward = alive_bonus - dist_penalty - vel_penalty
+
+        reward_info = {
+            "reward_survive": alive_bonus,
+            "distance_penalty": -dist_penalty,
+            "velocity_penalty": -vel_penalty,
+        }
+
+        return reward, reward_info
 
     def _get_obs(self):
         return np.concatenate(
             [
                 self.data.qpos[:1],  # cart x pos
                 np.sin(self.data.qpos[1:]),  # link angles
                 np.cos(self.data.qpos[1:]),
                 np.clip(self.data.qvel, -10, 10),
-                np.clip(self.data.qfrc_constraint, -10, 10),
+                np.clip(self.data.qfrc_constraint, -10, 10)[:1],
             ]
         ).ravel()
 
     def reset_model(self):
+        noise_low = -self._reset_noise_scale
+        noise_high = self._reset_noise_scale
+
         self.set_state(
             self.init_qpos
-            + self.np_random.uniform(low=-0.1, high=0.1, size=self.model.nq),
-            self.init_qvel + self.np_random.standard_normal(self.model.nv) * 0.1,
+            + self.np_random.uniform(
+                low=noise_low, high=noise_high, size=self.model.nq
+            ),
+            self.init_qvel
+            + self.np_random.standard_normal(self.model.nv) * self._reset_noise_scale,
         )
         return self._get_obs()
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/inverted_pendulum.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/inverted_pendulum.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         self.do_simulation(a, self.frame_skip)
 
         ob = self._get_obs()
         terminated = bool(not np.isfinite(ob).all() or (np.abs(ob[1]) > 0.2))
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return ob, reward, terminated, False, {}
 
     def reset_model(self):
         qpos = self.init_qpos + self.np_random.uniform(
             size=self.model.nq, low=-0.01, high=0.01
         )
         qvel = self.init_qvel + self.np_random.uniform(
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/mujoco_env.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/mujoco_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,22 +23,36 @@
 else:
     MUJOCO_IMPORT_ERROR = None
 
 
 DEFAULT_SIZE = 480
 
 
-class BaseMujocoEnv(gym.Env[np.float64, np.float32]):
+def expand_model_path(model_path: str) -> str:
+    """Expands the `model_path` to a full path if it starts with '~' or '.' or '/'."""
+    if model_path.startswith(".") or model_path.startswith("/"):
+        fullpath = model_path
+    elif model_path.startswith("~"):
+        fullpath = path.expanduser(model_path)
+    else:
+        fullpath = path.join(path.dirname(__file__), "assets", model_path)
+    if not path.exists(fullpath):
+        raise OSError(f"File {fullpath} does not exist")
+
+    return fullpath
+
+
+class BaseMujocoEnv(gym.Env[NDArray[np.float64], NDArray[np.float32]]):
     """Superclass for all MuJoCo environments."""
 
     def __init__(
         self,
         model_path,
         frame_skip,
-        observation_space: Space,
+        observation_space: Optional[Space],
         render_mode: Optional[str] = None,
         width: int = DEFAULT_SIZE,
         height: int = DEFAULT_SIZE,
         camera_id: Optional[int] = None,
         camera_name: Optional[str] = None,
     ):
         """Base abstract class for mujoco based environments.
@@ -53,22 +67,15 @@
             camera_id: The camera ID used.
             camera_name: The name of the camera used (can not be used in conjunction with `camera_id`).
 
         Raises:
             OSError: when the `model_path` does not exist.
             error.DependencyNotInstalled: When `mujoco` is not installed.
         """
-        if model_path.startswith(".") or model_path.startswith("/"):
-            self.fullpath = model_path
-        elif model_path.startswith("~"):
-            self.fullpath = path.expanduser(model_path)
-        else:
-            self.fullpath = path.join(path.dirname(__file__), "assets", model_path)
-        if not path.exists(self.fullpath):
-            raise OSError(f"File {self.fullpath} does not exist")
+        self.fullpath = expand_model_path(model_path)
 
         self.width = width
         self.height = height
         # may use width and height
         self.model, self.data = self._initialize_simulation()
 
         self.init_qpos = self.data.qpos.ravel().copy()
@@ -81,30 +88,34 @@
             "rgb_array",
             "depth_array",
         ], self.metadata["render_modes"]
         if "render_fps" in self.metadata:
             assert (
                 int(np.round(1.0 / self.dt)) == self.metadata["render_fps"]
             ), f'Expected value: {int(np.round(1.0 / self.dt))}, Actual value: {self.metadata["render_fps"]}'
-
-        self.observation_space = observation_space
+        if observation_space is not None:
+            self.observation_space = observation_space
         self._set_action_space()
 
         self.render_mode = render_mode
         self.camera_name = camera_name
         self.camera_id = camera_id
 
     def _set_action_space(self):
         bounds = self.model.actuator_ctrlrange.copy().astype(np.float32)
         low, high = bounds.T
         self.action_space = spaces.Box(low=low, high=high, dtype=np.float32)
         return self.action_space
 
     # methods to override:
     # ----------------------------
+    def step(
+        self, action: NDArray[np.float32]
+    ) -> Tuple[NDArray[np.float64], np.float64, bool, bool, Dict[str, np.float64]]:
+        raise NotImplementedError
 
     def reset_model(self) -> NDArray[np.float64]:
         """
         Reset the robot degrees of freedom (qpos and qvel).
         Implement this in each subclass.
         """
         raise NotImplementedError
@@ -207,15 +218,15 @@
                 "(HINT: you need to install mujoco-py, and also perform the setup instructions "
                 "here: https://github.com/openai/mujoco-py.)"
             )
 
         logger.deprecation(
             "This version of the mujoco environments depends "
             "on the mujoco-py bindings, which are no longer maintained "
-            "and may stop working. Please upgrade to the v4 versions of "
+            "and may stop working. Please upgrade to the v5 or v4 versions of "
             "the environments (which depend on the mujoco python bindings instead), unless "
             "you are trying to precisely replicate previous works)."
         )
 
         self.viewer = None
         self._viewers = {}
 
@@ -339,21 +350,22 @@
 class MujocoEnv(BaseMujocoEnv):
     """Superclass for MuJoCo environments."""
 
     def __init__(
         self,
         model_path,
         frame_skip,
-        observation_space: Space,
+        observation_space: Optional[Space],
         render_mode: Optional[str] = None,
         width: int = DEFAULT_SIZE,
         height: int = DEFAULT_SIZE,
         camera_id: Optional[int] = None,
         camera_name: Optional[str] = None,
-        default_camera_config: Optional[dict] = None,
+        default_camera_config: Optional[Dict[str, Union[float, int]]] = None,
+        max_geom: int = 1000,
     ):
         if MUJOCO_IMPORT_ERROR is not None:
             raise error.DependencyNotInstalled(
                 f"{MUJOCO_IMPORT_ERROR}. "
                 "(HINT: you need to install mujoco, run `pip install gymnasium[mujoco]`.)"
             )
 
@@ -367,20 +379,27 @@
             camera_id,
             camera_name,
         )
 
         from gymnasium.envs.mujoco.mujoco_rendering import MujocoRenderer
 
         self.mujoco_renderer = MujocoRenderer(
-            self.model, self.data, default_camera_config
+            self.model,
+            self.data,
+            default_camera_config,
+            self.width,
+            self.height,
+            max_geom,
+            camera_id,
+            camera_name,
         )
 
     def _initialize_simulation(
         self,
-    ):
+    ) -> Tuple["mujoco._structs.MjModel", "mujoco._structs.MjData"]:
         model = mujoco.MjModel.from_xml_path(self.fullpath)
         # MjrContext will copy model.vis.global_.off* to con.off*
         model.vis.global_.offwidth = self.width
         model.vis.global_.offheight = self.height
         data = mujoco.MjData(model)
         return model, data
 
@@ -402,17 +421,15 @@
 
         # As of MuJoCo 2.0, force-related quantities like cacc are not computed
         # unless there's a force sensor in the model.
         # See https://github.com/openai/gym/issues/1541
         mujoco.mj_rnePostConstraint(self.model, self.data)
 
     def render(self):
-        return self.mujoco_renderer.render(
-            self.render_mode, self.camera_id, self.camera_name
-        )
+        return self.mujoco_renderer.render(self.render_mode)
 
     def close(self):
         if self.mujoco_renderer is not None:
             self.mujoco_renderer.close()
 
     def get_body_com(self, body_name):
         return self.data.body(body_name).xpos
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/mujoco_rendering.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/mujoco_rendering.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,27 +34,32 @@
         ("osmesa", _import_osmesa),
     ]
 )
 
 
 class BaseRender:
     def __init__(
-        self, model: "mujoco.MjModel", data: "mujoco.MjData", width: int, height: int
+        self,
+        model: "mujoco.MjModel",
+        data: "mujoco.MjData",
+        width: int,
+        height: int,
+        max_geom: int = 1000,
     ):
         """Render context superclass for offscreen and window rendering."""
         self.model = model
         self.data = data
 
         self._markers = []
         self._overlays = {}
 
         self.viewport = mujoco.MjrRect(0, 0, width, height)
 
         # This goes to specific visualizer
-        self.scn = mujoco.MjvScene(self.model, 1000)
+        self.scn = mujoco.MjvScene(self.model, max_geom)
         self.cam = mujoco.MjvCamera()
         self.vopt = mujoco.MjvOption()
         self.pert = mujoco.MjvPerturb()
 
         self.make_context_current()
 
         # Keep in Mujoco Context
@@ -130,22 +135,26 @@
         """
         raise NotImplementedError
 
 
 class OffScreenViewer(BaseRender):
     """Offscreen rendering class with opengl context."""
 
-    def __init__(self, model: "mujoco.MjMujoco", data: "mujoco.MjData"):
-        width = model.vis.global_.offwidth
-        height = model.vis.global_.offheight
-
+    def __init__(
+        self,
+        model: "mujoco.MjMujoco",
+        data: "mujoco.MjData",
+        width: int,
+        height: int,
+        max_geom: int = 1000,
+    ):
         # We must make GLContext before MjrContext
         self._get_opengl_backend(width, height)
 
-        super().__init__(model, data, width, height)
+        super().__init__(model, data, width, height, max_geom)
 
         self._init_camera()
 
     def _init_camera(self):
         self.cam.type = mujoco.mjtCamera.mjCAMERA_FREE
         self.cam.fixedcamid = -1
         for i in range(3):
@@ -188,15 +197,15 @@
         self.opengl_context.free()
 
     def __del__(self):
         self.free()
 
     def render(
         self,
-        render_mode: str,
+        render_mode: Optional[str],
         camera_id: Optional[int] = None,
         segmentation: bool = False,
     ):
         if camera_id is not None:
             if camera_id == -1:
                 self.cam.type = mujoco.mjtCamera.mjCAMERA_FREE
             else:
@@ -277,15 +286,22 @@
         self.free()
         glfw.terminate()
 
 
 class WindowViewer(BaseRender):
     """Class for window rendering in all MuJoCo environments."""
 
-    def __init__(self, model: "mujoco.MjModel", data: "mujoco.MjData"):
+    def __init__(
+        self,
+        model: "mujoco.MjModel",
+        data: "mujoco.MjData",
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        max_geom: int = 1000,
+    ):
         glfw.init()
 
         self._button_left_pressed = False
         self._button_right_pressed = False
         self._last_mouse_x = 0
         self._last_mouse_y = 0
         self._paused = False
@@ -296,29 +312,34 @@
         self._image_path = "/tmp/frame_%07d.png"
         self._time_per_render = 1 / 60.0
         self._run_speed = 1.0
         self._loop_count = 0
         self._advance_by_one_step = False
         self._hide_menu = False
 
-        width, height = glfw.get_video_mode(glfw.get_primary_monitor()).size
+        monitor_width, monitor_height = glfw.get_video_mode(
+            glfw.get_primary_monitor()
+        ).size
+        width = monitor_width // 2 if width is None else width
+        height = monitor_height // 2 if height is None else height
+
         glfw.window_hint(glfw.VISIBLE, 1)
-        self.window = glfw.create_window(width // 2, height // 2, "mujoco", None, None)
+        self.window = glfw.create_window(width, height, "mujoco", None, None)
 
         self.width, self.height = glfw.get_framebuffer_size(self.window)
         window_width, _ = glfw.get_window_size(self.window)
         self._scale = self.width * 1.0 / window_width
 
         # set callbacks
         glfw.set_cursor_pos_callback(self.window, self._cursor_pos_callback)
         glfw.set_mouse_button_callback(self.window, self._mouse_button_callback)
         glfw.set_scroll_callback(self.window, self._scroll_callback)
         glfw.set_key_callback(self.window, self._key_callback)
 
-        super().__init__(model, data, width, height)
+        super().__init__(model, data, width, height, max_geom)
         glfw.swap_interval(1)
 
     def _set_mujoco_buffer(self):
         mujoco.mjr_setBuffer(mujoco.mjtFramebuffer.mjFB_WINDOW, self.con)
 
     def make_context_current(self):
         glfw.make_context_current(self.window)
@@ -515,15 +536,15 @@
             action = mujoco.mjtMouse.mjMOUSE_ZOOM
 
         dx = int(self._scale * xpos) - self._last_mouse_x
         dy = int(self._scale * ypos) - self._last_mouse_y
         width, height = glfw.get_framebuffer_size(window)
 
         mujoco.mjv_moveCamera(
-            self.model, action, dx / height, dy / height, self.scn, self.cam
+            self.model, action, dx / width, dy / height, self.scn, self.cam
         )
 
         self._last_mouse_x = int(self._scale * xpos)
         self._last_mouse_y = int(self._scale * ypos)
 
     def _mouse_button_callback(self, window: "glfw.LP__GLFWwindow", button, act, mods):
         self._button_left_pressed = (
@@ -585,17 +606,22 @@
             fname = self._image_path % (self._image_idx - 1)
             self.add_overlay(topleft, "Cap[t]ure frame", "Saved as %s" % fname)
         else:
             self.add_overlay(topleft, "Cap[t]ure frame", "")
         self.add_overlay(topleft, "Toggle geomgroup visibility", "0-4")
 
         self.add_overlay(bottomleft, "FPS", "%d%s" % (1 / self._time_per_render, ""))
-        self.add_overlay(
-            bottomleft, "Solver iterations", str(self.data.solver_iter + 1)
-        )
+        if mujoco.__version__ >= "3.0.0":
+            self.add_overlay(
+                bottomleft, "Solver iterations", str(self.data.solver_niter[0] + 1)
+            )
+        elif mujoco.__version__ < "3.0.0":
+            self.add_overlay(
+                bottomleft, "Solver iterations", str(self.data.solver_iter + 1)
+            )
         self.add_overlay(
             bottomleft, "Step", str(round(self.data.time / self.model.opt.timestep))
         )
         self.add_overlay(bottomleft, "timestep", "%.5f" % self.model.opt.timestep)
 
 
 class MujocoRenderer:
@@ -608,86 +634,94 @@
     """
 
     def __init__(
         self,
         model: "mujoco.MjModel",
         data: "mujoco.MjData",
         default_cam_config: Optional[dict] = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        max_geom: int = 1000,
+        camera_id: Optional[int] = None,
+        camera_name: Optional[str] = None,
     ):
         """A wrapper for clipping continuous actions within the valid bound.
 
         Args:
             model: MjModel data structure of the MuJoCo simulation
             data: MjData data structure of the MuJoCo simulation
             default_cam_config: dictionary with attribute values of the viewer's default camera, https://mujoco.readthedocs.io/en/latest/XMLreference.html?highlight=camera#visual-global
+            width: width of the OpenGL rendering context
+            height: height of the OpenGL rendering context
+            max_geom: maximum number of geometries to render
+            camera_id: The integer camera id from which to render the frame in the MuJoCo simulation
+            camera_name: The string name of the camera from which to render the frame in the MuJoCo simulation. This argument should not be passed if using cameara_id instead and vice versa
         """
         self.model = model
         self.data = data
         self._viewers = {}
         self.viewer = None
         self.default_cam_config = default_cam_config
+        self.width = width
+        self.height = height
+        self.max_geom = max_geom
+
+        # set self.camera_id using `camera_id` or `camera_name`
+        if camera_id is not None and camera_name is not None:
+            raise ValueError(
+                "Both `camera_id` and `camera_name` cannot be"
+                " specified at the same time."
+            )
+
+        no_camera_specified = camera_name is None and camera_id is None
+        if no_camera_specified:
+            camera_name = "track"
+
+        if camera_id is None:
+            self.camera_id = mujoco.mj_name2id(
+                self.model,
+                mujoco.mjtObj.mjOBJ_CAMERA,
+                camera_name,
+            )
 
     def render(
         self,
-        render_mode: str,
-        camera_id: Optional[int] = None,
-        camera_name: Optional[str] = None,
+        render_mode: Optional[str],
     ):
         """Renders a frame of the simulation in a specific format and camera view.
 
         Args:
             render_mode: The format to render the frame, it can be: "human", "rgb_array", or "depth_array"
-            camera_id: The integer camera id from which to render the frame in the MuJoCo simulation
-            camera_name: The string name of the camera from which to render the frame in the MuJoCo simulation. This argument should not be passed if using cameara_id instead and vice versa
 
         Returns:
             If render_mode is "rgb_array" or "depth_arra" it returns a numpy array in the specified format. "human" render mode does not return anything.
         """
 
         viewer = self._get_viewer(render_mode=render_mode)
 
-        if render_mode in {
-            "rgb_array",
-            "depth_array",
-        }:
-            if camera_id is not None and camera_name is not None:
-                raise ValueError(
-                    "Both `camera_id` and `camera_name` cannot be"
-                    " specified at the same time."
-                )
-
-            no_camera_specified = camera_name is None and camera_id is None
-            if no_camera_specified:
-                camera_name = "track"
-
-            if camera_id is None:
-                camera_id = mujoco.mj_name2id(
-                    self.model,
-                    mujoco.mjtObj.mjOBJ_CAMERA,
-                    camera_name,
-                )
-
-            img = viewer.render(render_mode=render_mode, camera_id=camera_id)
-            return img
-
+        if render_mode in ["rgb_array", "depth_array"]:
+            return viewer.render(render_mode=render_mode, camera_id=self.camera_id)
         elif render_mode == "human":
             return viewer.render()
 
-    def _get_viewer(self, render_mode: str):
+    def _get_viewer(self, render_mode: Optional[str]):
         """Initializes and returns a viewer class depending on the render_mode
         - `WindowViewer` class for "human" render mode
         - `OffScreenViewer` class for "rgb_array" or "depth_array" render mode
         """
         self.viewer = self._viewers.get(render_mode)
         if self.viewer is None:
             if render_mode == "human":
-                self.viewer = WindowViewer(self.model, self.data)
-
+                self.viewer = WindowViewer(
+                    self.model, self.data, self.width, self.height, self.max_geom
+                )
             elif render_mode in {"rgb_array", "depth_array"}:
-                self.viewer = OffScreenViewer(self.model, self.data)
+                self.viewer = OffScreenViewer(
+                    self.model, self.data, self.width, self.height, self.max_geom
+                )
             else:
                 raise AttributeError(
                     f"Unexpected mode: {render_mode}, expected modes: human, rgb_array, or depth_array"
                 )
             # Add default camera parameters
             self._set_cam_config()
             self._viewers[render_mode] = self.viewer
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/pusher.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/pusher_v4.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 import numpy as np
 
 from gymnasium import utils
-from gymnasium.envs.mujoco import MuJocoPyEnv
+from gymnasium.envs.mujoco import MujocoEnv
 from gymnasium.spaces import Box
 
 
-class PusherEnv(MuJocoPyEnv, utils.EzPickle):
+DEFAULT_CAMERA_CONFIG = {
+    "trackbodyid": -1,
+    "distance": 4.0,
+}
+
+
+class PusherEnv(MujocoEnv, utils.EzPickle):
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
         "render_fps": 20,
     }
 
     def __init__(self, **kwargs):
         utils.EzPickle.__init__(self, **kwargs)
         observation_space = Box(low=-np.inf, high=np.inf, shape=(23,), dtype=np.float64)
-        MuJocoPyEnv.__init__(
-            self, "pusher.xml", 5, observation_space=observation_space, **kwargs
+        MujocoEnv.__init__(
+            self,
+            "pusher.xml",
+            5,
+            observation_space=observation_space,
+            default_camera_config=DEFAULT_CAMERA_CONFIG,
+            **kwargs,
         )
 
     def step(self, a):
         vec_1 = self.get_body_com("object") - self.get_body_com("tips_arm")
         vec_2 = self.get_body_com("object") - self.get_body_com("goal")
 
         reward_near = -np.linalg.norm(vec_1)
@@ -32,27 +43,23 @@
         reward = reward_dist + 0.1 * reward_ctrl + 0.5 * reward_near
 
         self.do_simulation(a, self.frame_skip)
         if self.render_mode == "human":
             self.render()
 
         ob = self._get_obs()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return (
             ob,
             reward,
             False,
             False,
             dict(reward_dist=reward_dist, reward_ctrl=reward_ctrl),
         )
 
-    def viewer_setup(self):
-        assert self.viewer is not None
-        self.viewer.cam.trackbodyid = -1
-        self.viewer.cam.distance = 4.0
-
     def reset_model(self):
         qpos = self.init_qpos
 
         self.goal_pos = np.asarray([0, 0])
         while True:
             self.cylinder_pos = np.concatenate(
                 [
@@ -71,14 +78,14 @@
         qvel[-4:] = 0
         self.set_state(qpos, qvel)
         return self._get_obs()
 
     def _get_obs(self):
         return np.concatenate(
             [
-                self.sim.data.qpos.flat[:7],
-                self.sim.data.qvel.flat[:7],
+                self.data.qpos.flat[:7],
+                self.data.qvel.flat[:7],
                 self.get_body_com("tips_arm"),
                 self.get_body_com("object"),
                 self.get_body_com("goal"),
             ]
         )
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/pusher_v4.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/pusher_v5.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,62 @@
+__credits__ = ["Kallinteris-Andreas"]
+
+from typing import Dict, Union
+
 import numpy as np
 
 from gymnasium import utils
 from gymnasium.envs.mujoco import MujocoEnv
 from gymnasium.spaces import Box
 
 
 DEFAULT_CAMERA_CONFIG = {
     "trackbodyid": -1,
     "distance": 4.0,
 }
 
 
 class PusherEnv(MujocoEnv, utils.EzPickle):
-    """
+    r"""
     ## Description
-    "Pusher" is a multi-jointed robot arm which is very similar to that of a human.
-     The goal is to move a target cylinder (called *object*) to a goal position using the robot's end effector (called *fingertip*).
-      The robot consists of shoulder, elbow, forearm, and wrist joints.
+    "Pusher" is a multi-jointed robot arm that is very similar to a human arm.
+    The goal is to move a target cylinder (called *object*) to a goal position using the robot's end effector (called *fingertip*).
+    The robot consists of shoulder, elbow, forearm and wrist joints.
+
 
     ## Action Space
+    ```{figure} action_space_figures/pusher.png
+    :name: pusher
+    ```
+
     The action space is a `Box(-2, 2, (7,), float32)`. An action `(a, b)` represents the torques applied at the hinge joints.
 
-    | Num | Action                                                             | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit         |
+    | Num | Action                                                             | Control Min | Control Max | Name (in corresponding XML file) | Joint | Type (Unit)  |
     |-----|--------------------------------------------------------------------|-------------|-------------|----------------------------------|-------|--------------|
-    | 0    | Rotation of the panning the shoulder                              | -2          | 2           | r_shoulder_pan_joint             | hinge | torque (N m) |
-    | 1    | Rotation of the shoulder lifting joint                            | -2          | 2           | r_shoulder_lift_joint            | hinge | torque (N m) |
-    | 2    | Rotation of the shoulder rolling joint                            | -2          | 2           | r_upper_arm_roll_joint           | hinge | torque (N m) |
-    | 3    | Rotation of hinge joint that flexed the elbow                     | -2          | 2           | r_elbow_flex_joint               | hinge | torque (N m) |
-    | 4    | Rotation of hinge that rolls the forearm                          | -2          | 2           | r_forearm_roll_joint             | hinge | torque (N m) |
-    | 5    | Rotation of flexing the wrist                                     | -2          | 2           | r_wrist_flex_joint               | hinge | torque (N m) |
-    | 6    | Rotation of rolling the wrist                                     | -2          | 2           | r_wrist_roll_joint               | hinge | torque (N m) |
+    | 0   | Rotation of the panning the shoulder                               | -2          | 2           | r_shoulder_pan_joint             | hinge | torque (N m) |
+    | 1   | Rotation of the shoulder lifting joint                             | -2          | 2           | r_shoulder_lift_joint            | hinge | torque (N m) |
+    | 2   | Rotation of the shoulder rolling joint                             | -2          | 2           | r_upper_arm_roll_joint           | hinge | torque (N m) |
+    | 3   | Rotation of hinge joint that flexed the elbow                      | -2          | 2           | r_elbow_flex_joint               | hinge | torque (N m) |
+    | 4   | Rotation of hinge that rolls the forearm                           | -2          | 2           | r_forearm_roll_joint             | hinge | torque (N m) |
+    | 5   | Rotation of flexing the wrist                                      | -2          | 2           | r_wrist_flex_joint               | hinge | torque (N m) |
+    | 6   | Rotation of rolling the wrist                                      | -2          | 2           | r_wrist_roll_joint               | hinge | torque (N m) |
+
 
     ## Observation Space
+    The observation space consists of the following parts (in order):
 
-    Observations consist of
+    - *qpos (7 elements):* Position values of the robot's body parts.
+    - *qvel (7 elements):* The velocities of these individual body parts (their derivatives).
+    - *xpos (3 elements):* The coordinates of the fingertip of the pusher.
+    - *xpos (3 elements):* The coordinates of the object to be moved.
+    - *xpos (3 elements):* The coordinates of the goal position.
 
-    - Angle of rotational joints on the pusher
-    - Angular velocities of rotational joints on the pusher
-    - The coordinates of the fingertip of the pusher
-    - The coordinates of the object to be moved
-    - The coordinates of the goal position
-
-    The observation is a `Box(-Inf, Inf, (23,), float64)` where the elements correspond to the table below.
-    An analogy can be drawn to a human arm in order to help understand the state space, with the words flex and roll meaning the
-    same as human joints.
+    The observation space is a `Box(-Inf, Inf, (17,), float64)` where the elements are as follows:
 
-    | Num | Observation                                              | Min  | Max | Name (in corresponding XML file) | Joint    | Unit                     |
+    | Num | Observation                                              | Min  | Max | Name (in corresponding XML file) | Joint    | Type (Unit)              |
     | --- | -------------------------------------------------------- | ---- | --- | -------------------------------- | -------- | ------------------------ |
     | 0   | Rotation of the panning the shoulder                     | -Inf | Inf | r_shoulder_pan_joint             | hinge    | angle (rad)              |
     | 1   | Rotation of the shoulder lifting joint                   | -Inf | Inf | r_shoulder_lift_joint            | hinge    | angle (rad)              |
     | 2   | Rotation of the shoulder rolling joint                   | -Inf | Inf | r_upper_arm_roll_joint           | hinge    | angle (rad)              |
     | 3   | Rotation of hinge joint that flexed the elbow            | -Inf | Inf | r_elbow_flex_joint               | hinge    | angle (rad)              |
     | 4   | Rotation of hinge that rolls the forearm                 | -Inf | Inf | r_forearm_roll_joint             | hinge    | angle (rad)              |
     | 5   | Rotation of flexing the wrist                            | -Inf | Inf | r_wrist_flex_joint               | hinge    | angle (rad)              |
@@ -67,124 +74,174 @@
     | 17  | x-coordinate of the object to be moved                   | -Inf | Inf | object (obj_slidex)              | slide    | position (m)             |
     | 18  | y-coordinate of the object to be moved                   | -Inf | Inf | object (obj_slidey)              | slide    | position (m)             |
     | 19  | z-coordinate of the object to be moved                   | -Inf | Inf | object                           | cylinder | position (m)             |
     | 20  | x-coordinate of the goal position of the object          | -Inf | Inf | goal (goal_slidex)               | slide    | position (m)             |
     | 21  | y-coordinate of the goal position of the object          | -Inf | Inf | goal (goal_slidey)               | slide    | position (m)             |
     | 22  | z-coordinate of the goal position of the object          | -Inf | Inf | goal                             | sphere   | position (m)             |
 
+    To understand the state space, an analogy can be drawn to a human arm, where the words "flex" and "roll" have the same meaning as in human joints.
 
     ## Rewards
-    The reward consists of two parts:
-    - *reward_near *: This reward is a measure of how far the *fingertip*
-    of the pusher (the unattached end) is from the object, with a more negative
-    value assigned for when the pusher's *fingertip* is further away from the
-    target. It is calculated as the negative vector norm of (position of
-    the fingertip - position of target), or *-norm("fingertip" - "target")*.
-    - *reward_dist *: This reward is a measure of how far the object is from
-    the target goal position, with a more negative value assigned for object is
-    further away from the target. It is calculated as the negative vector norm of
-    (position of the object - position of goal), or *-norm("object" - "target")*.
-    - *reward_control*: A negative reward for penalising the pusher if
-    it takes actions that are too large. It is measured as the negative squared
-    Euclidean norm of the action, i.e. as *- sum(action<sup>2</sup>)*.
-
-    The total reward returned is ***reward*** *=* *reward_dist + 0.1 * reward_ctrl + 0.5 * reward_near*
-
-    Unlike other environments, Pusher does not allow you to specify weights for the individual reward terms.
-    However, `info` does contain the keys *reward_dist* and *reward_ctrl*. Thus, if you'd like to weight the terms,
-    you should create a wrapper that computes the weighted reward from `info`.
+    The total reward is: ***reward*** *=* *reward_dist + reward_ctrl + reward_near*.
+
+    - *reward_near*:
+    This reward is a measure of how far the *fingertip* of the pusher (the unattached end) is from the object,
+    with a more negative value assigned for when the pusher's *fingertip* is further away from the target.
+    It is $-w_{near} \|(P_{fingertip} - P_{target})\|_2$.
+    where $w_{near}$ is the `reward_near_weight` (default is $0.5$).
+    - *reward_dist*:
+    This reward is a measure of how far the object is from the target goal position,
+    with a more negative value assigned if the object is further away from the target.
+    It is $-w_{dist} \|(P_{object} - P_{target})\|_2$.
+    where $w_{dist}$ is the `reward_dist_weight` (default is $1$).
+    - *reward_control*:
+    A negative reward to penalize the pusher for taking actions that are too large.
+    It is measured as the negative squared Euclidean norm of the action, i.e. as $-w_{control} \|action\|_2^2$.
+    where $w_{control}$ is the `reward_control_weight` (default is $0.1$).
+
+    `info` contains the individual reward terms.
 
 
     ## Starting State
-    All pusher (not including object and goal) states start in
-    (0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0). A uniform noise in the range
-    [-0.005, 0.005] is added to the velocity attributes only. The velocities of
-    the object and goal are permanently set to 0. The object's x-position is selected uniformly
-    between [-0.3, 0] while the y-position is selected uniformly between [-0.2, 0.2], and this
-    process is repeated until the vector norm between the object's (x,y) position and origin is not greater
-    than 0.17. The goal always have the same position of (0.45, -0.05, -0.323).
+    The initial position state of the Pusher arm is $0_{6}$.
+    The initial position state of the object is $\mathcal{U}_{[[-0.3, -0.2], [0, 0.2]]}$.
+    The position state of the goal is (permanently) $[0.45, -0.05, -0.323]$.
+    The initial velocity state of the Pusher arm is $\mathcal{U}_{[-0.005 \times I_{6}, 0.005 \times I_{6}]}$.
+    The initial velocity state of the object is $0_2$.
+    The velocity state of the goal is (permanently) $0_3$.
 
-    The default framerate is 5 with each frame lasting for 0.01, giving rise to a *dt = 5 * 0.01 = 0.05*
+    where $\mathcal{U}$ is the multivariate uniform continuous distribution.
 
-    ## Episode End
+    Note that the initial position state of the object is sampled until its distance to the goal is $ > 0.17 m$.
 
-    The episode ends when any of the following happens:
+    The default frame rate is 5, with each frame lasting 0.01, so *dt = 5 * 0.01 = 0.05*.
 
-    1. Truncation: The episode duration reaches a 100 timesteps.
-    2. Termination: Any of the state space values is no longer finite.
 
-    ## Arguments
+    ## Episode End
+    ### Termination
+    The Pusher never terminates.
 
-    No additional arguments are currently supported (in v2 and lower),
-    but modifications can be made to the XML file in the assets folder
-    (or by changing the path to a modified XML file in another folder)..
+    ### Truncation
+    The default duration of an episode is 100 timesteps.
 
-    ```python
-    import gymnasium as gym
-    env = gym.make('Pusher-v4')
-    ```
 
-    There is no v3 for Pusher, unlike the robot environments where a v3 and
-    beyond take `gymnasmium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc.
+    ## Arguments
+    Pusher provides a range of parameters to modify the observation space, reward function, initial state, and termination condition.
+    These parameters can be applied during `gymnasium.make` in the following way:
 
     ```python
     import gymnasium as gym
-    env = gym.make('Pusher-v2')
+    env = gym.make('Pusher-v5', xml_file=...)
     ```
 
-    ## Version History
+    | Parameter               | Type       | Default      |Description                                               |
+    |-------------------------|------------|--------------|----------------------------------------------------------|
+    | `xml_file`              | **str**    |`"pusher.xml"`| Path to a MuJoCo model                                   |
+    | `reward_near_weight`    | **float**  | `0.5`        | Weight for _reward_near_ term (see `Rewards` section)    |
+    | `reward_dist_weight`    | **float**  | `1`          | Weight for _reward_dist_ term (see `Rewards` section)    |
+    | `reward_control_weight` | **float**  | `0.1`        | Weight for _reward_control_ term (see `Rewards` section) |
 
-    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3
-    * v2: All continuous control environments now use mujoco-py >= 1.50
-    * v1: max_time_steps raised to 1000 for robot based tasks (not including reacher, which has a max_time_steps of 50). Added reward_threshold to environments.
-    * v0: Initial versions release (1.0.0)
+    ## Version History
+    * v5:
+        - Minimum `mujoco` version is now 2.3.3.
+        - Added `default_camera_config` argument, a dictionary for setting the `mj_camera` properties, mainly useful for custom environments.
+        - Added `frame_skip` argument, used to configure the `dt` (duration of `step()`), default varies by environment check environment documentation pages.
+        - Added `xml_file` argument.
+        - Fixed bug: `reward_distance` & `reward_near` was based on the state before the physics step, now it is based on the state after the physics step (related [GitHub issue](https://github.com/Farama-Foundation/Gymnasium/issues/821)).
+        - Added `reward_near_weight`, `reward_dist_weight`, `reward_control_weight` arguments to configure the reward function (defaults are effectively the same as in `v4`).
+        - Fixed `info["reward_ctrl"]` not being multiplied by the reward weight.
+        - Added `info["reward_near"]` which is equal to the reward term `reward_near`.
+    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3.
+    * v3: This environment does not have a v3 release.
+    * v2: All continuous control environments now use mujoco-py >= 1.50.
+    * v1: max_time_steps raised to 1000 for robot based tasks (not including pusher, which has a max_time_steps of 100). Added reward_threshold to environments.
+    * v0: Initial versions release.
     """
 
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
-        "render_fps": 20,
     }
 
-    def __init__(self, **kwargs):
-        utils.EzPickle.__init__(self, **kwargs)
+    def __init__(
+        self,
+        xml_file: str = "pusher.xml",
+        frame_skip: int = 5,
+        default_camera_config: Dict[str, Union[float, int]] = DEFAULT_CAMERA_CONFIG,
+        reward_near_weight: float = 0.5,
+        reward_dist_weight: float = 1,
+        reward_control_weight: float = 0.1,
+        **kwargs,
+    ):
+        utils.EzPickle.__init__(
+            self,
+            xml_file,
+            frame_skip,
+            default_camera_config,
+            reward_near_weight,
+            reward_dist_weight,
+            reward_control_weight,
+            **kwargs,
+        )
+        self._reward_near_weight = reward_near_weight
+        self._reward_dist_weight = reward_dist_weight
+        self._reward_control_weight = reward_control_weight
+
         observation_space = Box(low=-np.inf, high=np.inf, shape=(23,), dtype=np.float64)
+
         MujocoEnv.__init__(
             self,
-            "pusher.xml",
-            5,
+            xml_file,
+            frame_skip,
             observation_space=observation_space,
-            default_camera_config=DEFAULT_CAMERA_CONFIG,
+            default_camera_config=default_camera_config,
             **kwargs,
         )
 
-    def step(self, a):
-        vec_1 = self.get_body_com("object") - self.get_body_com("tips_arm")
-        vec_2 = self.get_body_com("object") - self.get_body_com("goal")
-
-        reward_near = -np.linalg.norm(vec_1)
-        reward_dist = -np.linalg.norm(vec_2)
-        reward_ctrl = -np.square(a).sum()
-        reward = reward_dist + 0.1 * reward_ctrl + 0.5 * reward_near
+        self.metadata = {
+            "render_modes": [
+                "human",
+                "rgb_array",
+                "depth_array",
+            ],
+            "render_fps": int(np.round(1.0 / self.dt)),
+        }
+
+    def step(self, action):
+        self.do_simulation(action, self.frame_skip)
+
+        observation = self._get_obs()
+        reward, reward_info = self._get_rew(action)
+        info = reward_info
 
-        self.do_simulation(a, self.frame_skip)
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
+        return observation, reward, False, False, info
 
-        ob = self._get_obs()
-        return (
-            ob,
-            reward,
-            False,
-            False,
-            dict(reward_dist=reward_dist, reward_ctrl=reward_ctrl),
-        )
+    def _get_rew(self, action):
+        vec_1 = self.get_body_com("object") - self.get_body_com("tips_arm")
+        vec_2 = self.get_body_com("object") - self.get_body_com("goal")
+
+        reward_near = -np.linalg.norm(vec_1) * self._reward_near_weight
+        reward_dist = -np.linalg.norm(vec_2) * self._reward_dist_weight
+        reward_ctrl = -np.square(action).sum() * self._reward_control_weight
+
+        reward = reward_dist + reward_ctrl + reward_near
+
+        reward_info = {
+            "reward_dist": reward_dist,
+            "reward_ctrl": reward_ctrl,
+            "reward_near": reward_near,
+        }
+
+        return reward, reward_info
 
     def reset_model(self):
         qpos = self.init_qpos
 
         self.goal_pos = np.asarray([0, 0])
         while True:
             self.cylinder_pos = np.concatenate(
@@ -204,14 +261,14 @@
         qvel[-4:] = 0
         self.set_state(qpos, qvel)
         return self._get_obs()
 
     def _get_obs(self):
         return np.concatenate(
             [
-                self.data.qpos.flat[:7],
-                self.data.qvel.flat[:7],
+                self.data.qpos.flatten()[:7],
+                self.data.qvel.flatten()[:7],
                 self.get_body_com("tips_arm"),
                 self.get_body_com("object"),
                 self.get_body_com("goal"),
             ]
         )
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/reacher.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/reacher_v4.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,59 @@
 import numpy as np
 
 from gymnasium import utils
-from gymnasium.envs.mujoco import MuJocoPyEnv
+from gymnasium.envs.mujoco import MujocoEnv
 from gymnasium.spaces import Box
 
 
-class ReacherEnv(MuJocoPyEnv, utils.EzPickle):
+DEFAULT_CAMERA_CONFIG = {"trackbodyid": 0}
+
+
+class ReacherEnv(MujocoEnv, utils.EzPickle):
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
         "render_fps": 50,
     }
 
     def __init__(self, **kwargs):
         utils.EzPickle.__init__(self, **kwargs)
         observation_space = Box(low=-np.inf, high=np.inf, shape=(11,), dtype=np.float64)
-        MuJocoPyEnv.__init__(
-            self, "reacher.xml", 2, observation_space=observation_space, **kwargs
+        MujocoEnv.__init__(
+            self,
+            "reacher.xml",
+            2,
+            observation_space=observation_space,
+            default_camera_config=DEFAULT_CAMERA_CONFIG,
+            **kwargs,
         )
 
     def step(self, a):
         vec = self.get_body_com("fingertip") - self.get_body_com("target")
         reward_dist = -np.linalg.norm(vec)
         reward_ctrl = -np.square(a).sum()
         reward = reward_dist + reward_ctrl
 
         self.do_simulation(a, self.frame_skip)
         if self.render_mode == "human":
             self.render()
 
         ob = self._get_obs()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return (
             ob,
             reward,
             False,
             False,
             dict(reward_dist=reward_dist, reward_ctrl=reward_ctrl),
         )
 
-    def viewer_setup(self):
-        assert self.viewer is not None
-        self.viewer.cam.trackbodyid = 0
-
     def reset_model(self):
         qpos = (
             self.np_random.uniform(low=-0.1, high=0.1, size=self.model.nq)
             + self.init_qpos
         )
         while True:
             self.goal = self.np_random.uniform(low=-0.2, high=0.2, size=2)
@@ -59,17 +64,17 @@
             low=-0.005, high=0.005, size=self.model.nv
         )
         qvel[-2:] = 0
         self.set_state(qpos, qvel)
         return self._get_obs()
 
     def _get_obs(self):
-        theta = self.sim.data.qpos.flat[:2]
+        theta = self.data.qpos.flat[:2]
         return np.concatenate(
             [
                 np.cos(theta),
                 np.sin(theta),
-                self.sim.data.qpos.flat[2:],
-                self.sim.data.qvel.flat[:2],
+                self.data.qpos.flat[2:],
+                self.data.qvel.flat[:2],
                 self.get_body_com("fingertip") - self.get_body_com("target"),
             ]
         )
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/reacher_v4.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/inverted_pendulum_v5.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,190 +1,190 @@
+__credits__ = ["Kallinteris-Andreas"]
+
+from typing import Dict, Union
+
 import numpy as np
 
 from gymnasium import utils
 from gymnasium.envs.mujoco import MujocoEnv
 from gymnasium.spaces import Box
 
 
-DEFAULT_CAMERA_CONFIG = {"trackbodyid": 0}
+DEFAULT_CAMERA_CONFIG = {
+    "trackbodyid": 0,
+    "distance": 2.04,
+}
 
 
-class ReacherEnv(MujocoEnv, utils.EzPickle):
+class InvertedPendulumEnv(MujocoEnv, utils.EzPickle):
     """
     ## Description
-    "Reacher" is a two-jointed robot arm. The goal is to move the robot's end effector (called *fingertip*) close to a
-    target that is spawned at a random position.
+    This environment is the Cartpole environment, based on the work of Barto, Sutton, and Anderson in ["Neuronlike adaptive elements that can solve difficult learning control problems"](https://ieeexplore.ieee.org/document/6313077),
+    just like in the classic environments, but now powered by the Mujoco physics simulator - allowing for more complex experiments (such as varying the effects of gravity).
+    This environment consists of a cart that can be moved linearly, with a pole attached to one end and having another end free.
+    The cart can be pushed left or right, and the goal is to balance the pole on top of the cart by applying forces to the cart.
+
 
     ## Action Space
-    The action space is a `Box(-1, 1, (2,), float32)`. An action `(a, b)` represents the torques applied at the hinge joints.
+    The agent take a 1-element vector for actions.
 
-    | Num | Action                                                                          | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit |
-    |-----|---------------------------------------------------------------------------------|-------------|-------------|--------------------------|-------|------|
-    | 0   | Torque applied at the first hinge (connecting the link to the point of fixture) | -1 | 1 | joint0  | hinge | torque (N m) |
-    | 1   |  Torque applied at the second hinge (connecting the two links)                  | -1 | 1 | joint1  | hinge | torque (N m) |
+    The action space is a continuous `(action)` in `[-3, 3]`, where `action` represents
+    the numerical force applied to the cart (with magnitude representing the amount of
+    force and sign representing the direction)
+
+    | Num | Action                    | Control Min | Control Max | Name (in corresponding XML file) | Joint |Type (Unit)|
+    |-----|---------------------------|-------------|-------------|----------------------------------|-------|-----------|
+    | 0   | Force applied on the cart | -3          | 3           | slider                           | slide | Force (N) |
 
-    ## Observation Space
-    Observations consist of
 
-    - The cosine of the angles of the two arms
-    - The sine of the angles of the two arms
-    - The coordinates of the target
-    - The angular velocities of the arms
-    - The vector between the target and the reacher's fingertip (3 dimensional with the last element being 0)
-
-    The observation is a `Box(-Inf, Inf, (11,), float64)` where the elements correspond to the following:
-
-    | Num | Observation                                                                                    | Min  | Max | Name (in corresponding XML file) | Joint | Unit                     |
-    | --- | ---------------------------------------------------------------------------------------------- | ---- | --- | -------------------------------- | ----- | ------------------------ |
-    | 0   | cosine of the angle of the first arm                                                           | -Inf | Inf | cos(joint0)                      | hinge | unitless                 |
-    | 1   | cosine of the angle of the second arm                                                          | -Inf | Inf | cos(joint1)                      | hinge | unitless                 |
-    | 2   | sine of the angle of the first arm                                                             | -Inf | Inf | sin(joint0)                      | hinge | unitless                 |
-    | 3   | sine of the angle of the second arm                                                            | -Inf | Inf | sin(joint1)                      | hinge | unitless                 |
-    | 4   | x-coordinate of the target                                                                     | -Inf | Inf | target_x                         | slide | position (m)             |
-    | 5   | y-coordinate of the target                                                                     | -Inf | Inf | target_y                         | slide | position (m)             |
-    | 6   | angular velocity of the first arm                                                              | -Inf | Inf | joint0                           | hinge | angular velocity (rad/s) |
-    | 7   | angular velocity of the second arm                                                             | -Inf | Inf | joint1                           | hinge | angular velocity (rad/s) |
-    | 8   | x-value of position_fingertip - position_target                                                | -Inf | Inf | NA                               | slide | position (m)             |
-    | 9   | y-value of position_fingertip - position_target                                                | -Inf | Inf | NA                               | slide | position (m)             |
-    | 10  | z-value of position_fingertip - position_target (constantly 0 since reacher is 2d and z is same for both) | -Inf | Inf | NA                               | slide | position (m)             |
-
-
-    Most Gym environments just return the positions and velocity of the
-    joints in the `.xml` file as the state of the environment. However, in
-    reacher the state is created by combining only certain elements of the
-    position and velocity, and performing some function transformations on them.
-    If one is to read the `.xml` for reacher then they will find 4 joints:
-
-    | Num | Observation                 | Min      | Max      | Name (in corresponding XML file) | Joint | Unit               |
-    |-----|-----------------------------|----------|----------|----------------------------------|-------|--------------------|
-    | 0   | angle of the first arm      | -Inf     | Inf      | joint0                           | hinge | angle (rad)        |
-    | 1   | angle of the second arm     | -Inf     | Inf      | joint1                           | hinge | angle (rad)        |
-    | 2   | x-coordinate of the target  | -Inf     | Inf      | target_x                         | slide | position (m)       |
-    | 3   | y-coordinate of the target  | -Inf     | Inf      | target_y                         | slide | position (m)       |
+    ## Observation Space
+    The observation space consists of the following parts (in order):
+    - *qpos (2 element):* Position values of the robot's cart and pole.
+    - *qvel (2 elements):* The velocities of cart and pole (their derivatives).
+
+    The observation space is a `Box(-Inf, Inf, (4,), float64)` where the elements are as follows:
+
+    | Num | Observation                                   | Min  | Max | Name (in corresponding XML file) | Joint | Type (Unit)              |
+    | --- | --------------------------------------------- | ---- | --- | -------------------------------- | ----- | ------------------------- |
+    | 0   | position of the cart along the linear surface | -Inf | Inf | slider                           | slide | position (m)              |
+    | 1   | vertical angle of the pole on the cart        | -Inf | Inf | hinge                            | hinge | angle (rad)               |
+    | 2   | linear velocity of the cart                   | -Inf | Inf | slider                           | slide | velocity (m/s)            |
+    | 3   | angular velocity of the pole on the cart      | -Inf | Inf | hinge                            | hinge | angular velocity (rad/s)  |
 
 
     ## Rewards
-    The reward consists of two parts:
-    - *reward_distance*: This reward is a measure of how far the *fingertip*
-    of the reacher (the unattached end) is from the target, with a more negative
-    value assigned for when the reacher's *fingertip* is further away from the
-    target. It is calculated as the negative vector norm of (position of
-    the fingertip - position of target), or *-norm("fingertip" - "target")*.
-    - *reward_control*: A negative reward for penalising the walker if
-    it takes actions that are too large. It is measured as the negative squared
-    Euclidean norm of the action, i.e. as *- sum(action<sup>2</sup>)*.
-
-    The total reward returned is ***reward*** *=* *reward_distance + reward_control*
-
-    Unlike other environments, Reacher does not allow you to specify weights for the individual reward terms.
-    However, `info` does contain the keys *reward_dist* and *reward_ctrl*. Thus, if you'd like to weight the terms,
-    you should create a wrapper that computes the weighted reward from `info`.
+    The goal is to keep the inverted pendulum stand upright (within a certain angle limit) for as long as possible - as such, a reward of +1 is given for each timestep that the pole is upright.
+
+    The pole is considered upright if:
+    $|angle| < 0.2$.
+
+    and `info` also contains the reward.
 
 
     ## Starting State
-    All observations start in state
-    (0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0)
-    with a noise added for stochasticity. A uniform noise in the range
-    [-0.1, 0.1] is added to the positional attributes, while the target position
-    is selected uniformly at random in a disk of radius 0.2 around the origin.
-    Independent, uniform noise in the
-    range of [-0.005, 0.005] is added to the velocities, and the last
-    element ("fingertip" - "target") is calculated at the end once everything
-    is set. The default setting has a framerate of 2 and a *dt = 2 * 0.01 = 0.02*
+    The initial position state is $\\mathcal{U}_{[-reset\\_noise\\_scale \times I_{2}, reset\\_noise\\_scale \times I_{2}]}$.
+    The initial velocity state is $\\mathcal{U}_{[-reset\\_noise\\_scale \times I_{2}, reset\\_noise\\_scale \times I_{2}]}$.
+
+    where $\\mathcal{U}$ is the multivariate uniform continuous distribution.
+
 
     ## Episode End
+    ### Termination
+    The environment terminates when the Inverted Pendulum is unhealthy.
+    The Inverted Pendulum is unhealthy if any of the following happens:
 
-    The episode ends when any of the following happens:
+    1. Any of the state space values is no longer finite.
+    2. The absolute value of the vertical angle between the pole and the cart is greater than 0.2 radians.
 
-    1. Truncation: The episode duration reaches a 50 timesteps (with a new random target popping up if the reacher's fingertip reaches it before 50 timesteps)
-    2. Termination: Any of the state space values is no longer finite.
+    ### Truncation
+    The default duration of an episode is 1000 timesteps.
 
-    ## Arguments
 
-    No additional arguments are currently supported (in v2 and lower),
-    but modifications can be made to the XML file in the assets folder
-    (or by changing the path to a modified XML file in another folder)..
+    ## Arguments
+    InvertedPendulum provides a range of parameters to modify the observation space, reward function, initial state, and termination condition.
+    These parameters can be applied during `gymnasium.make` in the following way:
 
     ```python
     import gymnasium as gym
-    env = gym.make('Reacher-v4')
+    env = gym.make('InvertedPendulum-v5', reset_noise_scale=0.1)
     ```
 
-    There is no v3 for Reacher, unlike the robot environments where a v3 and
-    beyond take `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc.
+    | Parameter               | Type       | Default                 | Description                                                                                   |
+    |-------------------------|------------|-------------------------|-----------------------------------------------------------------------------------------------|
+    | `xml_file`              | **str**    |`"inverted_pendulum.xml"`| Path to a MuJoCo model                                                                        |
+    | `reset_noise_scale`     | **float**  | `0.01`                  | Scale of random perturbations of initial position and velocity (see `Starting State` section) |
 
     ## Version History
-
-    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3
-    * v2: All continuous control environments now use mujoco-py >= 1.50
-    * v1: max_time_steps raised to 1000 for robot based tasks (not including reacher, which has a max_time_steps of 50). Added reward_threshold to environments.
-    * v0: Initial versions release (1.0.0)
+    * v5:
+        - Minimum `mujoco` version is now 2.3.3.
+        - Added support for fully custom/third party `mujoco` models using the `xml_file` argument (previously only a few changes could be made to the existing models).
+        - Added `default_camera_config` argument, a dictionary for setting the `mj_camera` properties, mainly useful for custom environments.
+        - Added `env.observation_structure`, a dictionary for specifying the observation space compose (e.g. `qpos`, `qvel`), useful for building tooling and wrappers for the MuJoCo environments.
+        - Added `frame_skip` argument, used to configure the `dt` (duration of `step()`), default varies by environment check environment documentation pages.
+        - Fixed bug: `healthy_reward` was given on every step (even if the Pendulum is unhealthy), now it is only given if the Pendulum is healthy (not terminated) (related [GitHub issue](https://github.com/Farama-Foundation/Gymnasium/issues/500)).
+        - Added `xml_file` argument.
+        - Added `reset_noise_scale` argument to set the range of initial states.
+        - Added `info["reward_survive"]` which contains the reward.
+    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3.
+    * v3: This environment does not have a v3 release.
+    * v2: All continuous control environments now use mujoco-py >= 1.5.
+    * v1: max_time_steps raised to 1000 for robot based tasks (including inverted pendulum).
+    * v0: Initial versions release.
     """
 
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
-        "render_fps": 50,
     }
 
-    def __init__(self, **kwargs):
-        utils.EzPickle.__init__(self, **kwargs)
-        observation_space = Box(low=-np.inf, high=np.inf, shape=(11,), dtype=np.float64)
+    def __init__(
+        self,
+        xml_file: str = "inverted_pendulum.xml",
+        frame_skip: int = 2,
+        default_camera_config: Dict[str, Union[float, int]] = DEFAULT_CAMERA_CONFIG,
+        reset_noise_scale: float = 0.01,
+        **kwargs,
+    ):
+        utils.EzPickle.__init__(self, xml_file, frame_skip, reset_noise_scale, **kwargs)
+        observation_space = Box(low=-np.inf, high=np.inf, shape=(4,), dtype=np.float64)
+
+        self._reset_noise_scale = reset_noise_scale
+
         MujocoEnv.__init__(
             self,
-            "reacher.xml",
-            2,
+            xml_file,
+            frame_skip,
             observation_space=observation_space,
-            default_camera_config=DEFAULT_CAMERA_CONFIG,
+            default_camera_config=default_camera_config,
             **kwargs,
         )
 
-    def step(self, a):
-        vec = self.get_body_com("fingertip") - self.get_body_com("target")
-        reward_dist = -np.linalg.norm(vec)
-        reward_ctrl = -np.square(a).sum()
-        reward = reward_dist + reward_ctrl
+        self.metadata = {
+            "render_modes": [
+                "human",
+                "rgb_array",
+                "depth_array",
+            ],
+            "render_fps": int(np.round(1.0 / self.dt)),
+        }
+
+        self.observation_structure = {
+            "qpos": self.data.qpos.size,
+            "qvel": self.data.qvel.size,
+        }
 
-        self.do_simulation(a, self.frame_skip)
-        if self.render_mode == "human":
-            self.render()
+    def step(self, action):
+        self.do_simulation(action, self.frame_skip)
+
+        observation = self._get_obs()
 
-        ob = self._get_obs()
-        return (
-            ob,
-            reward,
-            False,
-            False,
-            dict(reward_dist=reward_dist, reward_ctrl=reward_ctrl),
+        terminated = bool(
+            not np.isfinite(observation).all() or (np.abs(observation[1]) > 0.2)
         )
 
+        reward = int(not terminated)
+
+        info = {"reward_survive": reward}
+
+        if self.render_mode == "human":
+            self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
+        return observation, reward, terminated, False, info
+
     def reset_model(self):
-        qpos = (
-            self.np_random.uniform(low=-0.1, high=0.1, size=self.model.nq)
-            + self.init_qpos
+        noise_low = -self._reset_noise_scale
+        noise_high = self._reset_noise_scale
+
+        qpos = self.init_qpos + self.np_random.uniform(
+            size=self.model.nq, low=noise_low, high=noise_high
         )
-        while True:
-            self.goal = self.np_random.uniform(low=-0.2, high=0.2, size=2)
-            if np.linalg.norm(self.goal) < 0.2:
-                break
-        qpos[-2:] = self.goal
         qvel = self.init_qvel + self.np_random.uniform(
-            low=-0.005, high=0.005, size=self.model.nv
+            size=self.model.nv, low=noise_low, high=noise_high
         )
-        qvel[-2:] = 0
         self.set_state(qpos, qvel)
         return self._get_obs()
 
     def _get_obs(self):
-        theta = self.data.qpos.flat[:2]
-        return np.concatenate(
-            [
-                np.cos(theta),
-                np.sin(theta),
-                self.data.qpos.flat[2:],
-                self.data.qvel.flat[:2],
-                self.get_body_com("fingertip") - self.get_body_com("target"),
-            ]
-        )
+        return np.concatenate([self.data.qpos, self.data.qvel]).ravel()
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/swimmer.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/swimmer.py`

 * *Files 26% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         reward_ctrl = -ctrl_cost_coeff * np.square(a).sum()
         reward = reward_fwd + reward_ctrl
         ob = self._get_obs()
 
         if self.render_mode == "human":
             self.render()
 
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return (
             ob,
             reward,
             False,
             False,
             dict(reward_fwd=reward_fwd, reward_ctrl=reward_ctrl),
         )
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/swimmer_v3.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/swimmer_v3.py`

 * *Files 11% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             "x_velocity": x_velocity,
             "y_velocity": y_velocity,
             "forward_reward": forward_reward,
         }
 
         if self.render_mode == "human":
             self.render()
-
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return observation, reward, False, False, info
 
     def _get_obs(self):
         position = self.sim.data.qpos.flat.copy()
         velocity = self.sim.data.qvel.flat.copy()
 
         if self._exclude_current_positions_from_observation:
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/swimmer_v4.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/swimmer_v5.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,153 +1,176 @@
-__credits__ = ["Rushiv Arora"]
+__credits__ = ["Kallinteris-Andreas", "Rushiv Arora"]
+
+from typing import Dict, Union
 
 import numpy as np
 
 from gymnasium import utils
 from gymnasium.envs.mujoco import MujocoEnv
 from gymnasium.spaces import Box
 
 
 class SwimmerEnv(MujocoEnv, utils.EzPickle):
-    """
+    r"""
     ## Description
-
-    This environment corresponds to the Swimmer environment described in Rémi Coulom's PhD thesis
-    ["Reinforcement Learning Using Neural Networks, with Applications to Motor Control"](https://tel.archives-ouvertes.fr/tel-00003985/document).
-    The environment aims to increase the number of independent state and control
-    variables as compared to the classic control environments. The swimmers
-    consist of three or more segments ('***links***') and one less articulation
-    joints ('***rotors***') - one rotor joint connecting exactly two links to
-    form a linear chain. The swimmer is suspended in a two dimensional pool and
-    always starts in the same position (subject to some deviation drawn from an
-    uniform distribution), and the goal is to move as fast as possible towards
-    the right by applying torque on the rotors and using the fluids friction.
+    This environment corresponds to the Swimmer environment described in Rémi Coulom's PhD thesis ["Reinforcement Learning Using Neural Networks, with Applications to Motor Control"](https://tel.archives-ouvertes.fr/tel-00003985/document).
+    The environment aims to increase the number of independent state and control variables compared to classical control environments.
+    The swimmers consist of three or more segments ('***links***') and one less articulation joints ('***rotors***') - one rotor joint connects exactly two links to form a linear chain.
+    The swimmer is suspended in a two-dimensional pool and always starts in the same position (subject to some deviation drawn from a uniform distribution),
+    and the goal is to move as fast as possible towards the right by applying torque to the rotors and using fluid friction.
 
     ## Notes
 
     The problem parameters are:
     Problem parameters:
     * *n*: number of body parts
     * *m<sub>i</sub>*: mass of part *i* (*i* ∈ {1...n})
     * *l<sub>i</sub>*: length of part *i* (*i* ∈ {1...n})
     * *k*: viscous-friction coefficient
 
-    While the default environment has *n* = 3, *l<sub>i</sub>* = 0.1,
-    and *k* = 0.1. It is possible to pass a custom MuJoCo XML file during construction to increase the
-    number of links, or to tweak any of the parameters.
+    While the default environment has *n* = 3, *l<sub>i</sub>* = 0.1, and *k* = 0.1.
+    It is possible to pass a custom MuJoCo XML file during construction to increase the number of links, or to tweak any of the parameters.
+
 
     ## Action Space
+    ```{figure} action_space_figures/swimmer.png
+    :name: swimmer
+    ```
+
     The action space is a `Box(-1, 1, (2,), float32)`. An action represents the torques applied between *links*
 
-    | Num | Action                             | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit         |
+    | Num | Action                             | Control Min | Control Max | Name (in corresponding XML file) | Joint | Type (Unit)  |
     |-----|------------------------------------|-------------|-------------|----------------------------------|-------|--------------|
     | 0   | Torque applied on the first rotor  | -1          | 1           | motor1_rot                       | hinge | torque (N m) |
     | 1   | Torque applied on the second rotor | -1          | 1           | motor2_rot                       | hinge | torque (N m) |
 
+
     ## Observation Space
-    By default, observations consists of:
-    * θ<sub>i</sub>: angle of part *i* with respect to the *x* axis
-    * θ<sub>i</sub>': its derivative with respect to time (angular velocity)
-
-    In the default case, observations do not include the x- and y-coordinates of the front tip. These may
-    be included by passing `exclude_current_positions_from_observation=False` during construction.
-    Then, the observation space will be `Box(-Inf, Inf, (10,), float64)` where the first two observations
-    represent the x- and y-coordinates of the front tip.
-    Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the x- and y-coordinates
-    will be returned in `info` with keys `"x_position"` and `"y_position"`, respectively.
+    The observation space consists of the following parts (in order):
 
-    By default, the observation is a `Box(-Inf, Inf, (8,), float64)` where the elements correspond to the following:
+    - *qpos (3 elements by default):* Position values of the robot's body parts.
+    - *qvel (5 elements):* The velocities of these individual body parts (their derivatives).
 
-    | Num | Observation                          | Min  | Max | Name (in corresponding XML file) | Joint | Unit                     |
+    By default, the observation does not include the x- and y-coordinates of the front tip.
+    These can be included by passing `exclude_current_positions_from_observation=False` during construction.
+    In this case, the observation space will be a `Box(-Inf, Inf, (10,), float64)`, where the first two observations are the x- and y-coordinates of the front tip.
+    Regardless of whether `exclude_current_positions_from_observation` is set to `True` or `False`, the x- and y-coordinates are returned in `info` with the keys `"x_position"` and `"y_position"`, respectively.
+
+    By default, however, the observation space is a `Box(-Inf, Inf, (8,), float64)` where the elements are as follows:
+
+    | Num | Observation                          | Min  | Max | Name (in corresponding XML file) | Joint | Type (Unit)              |
     | --- | ------------------------------------ | ---- | --- | -------------------------------- | ----- | ------------------------ |
     | 0   | angle of the front tip               | -Inf | Inf | free_body_rot                    | hinge | angle (rad)              |
     | 1   | angle of the first rotor             | -Inf | Inf | motor1_rot                       | hinge | angle (rad)              |
     | 2   | angle of the second rotor            | -Inf | Inf | motor2_rot                       | hinge | angle (rad)              |
     | 3   | velocity of the tip along the x-axis | -Inf | Inf | slider1                          | slide | velocity (m/s)           |
     | 4   | velocity of the tip along the y-axis | -Inf | Inf | slider2                          | slide | velocity (m/s)           |
     | 5   | angular velocity of front tip        | -Inf | Inf | free_body_rot                    | hinge | angular velocity (rad/s) |
     | 6   | angular velocity of first rotor      | -Inf | Inf | motor1_rot                       | hinge | angular velocity (rad/s) |
     | 7   | angular velocity of second rotor     | -Inf | Inf | motor2_rot                       | hinge | angular velocity (rad/s) |
     | excluded | position of the tip along the x-axis | -Inf | Inf | slider1                          | slide | position (m)           |
     | excluded | position of the tip along the y-axis | -Inf | Inf | slider2                          | slide | position (m)           |
 
+
     ## Rewards
-    The reward consists of two parts:
-    - *forward_reward*: A reward of moving forward which is measured
-    as *`forward_reward_weight` * (x-coordinate before action - x-coordinate after action)/dt*. *dt* is
-    the time between actions and is dependent on the frame_skip parameter
-    (default is 4), where the frametime is 0.01 - making the
-    default *dt = 4 * 0.01 = 0.04*. This reward would be positive if the swimmer
-    swims right as desired.
-    - *ctrl_cost*: A cost for penalising the swimmer if it takes
-    actions that are too large. It is measured as *`ctrl_cost_weight` *
-    sum(action<sup>2</sup>)* where *`ctrl_cost_weight`* is a parameter set for the
-    control and has a default value of 1e-4
+    The total reward is: ***reward*** *=* *forward_reward - ctrl_cost*.
+
+    - *forward_reward*:
+    A reward for moving forward,
+    this reward would be positive if the Swimmer moves forward (in the positive $x$ direction / in the right direction).
+    $w_{forward} \times \frac{dx}{dt}$, where
+    $dx$ is the displacement of the (front) "tip" ($x_{after-action} - x_{before-action}$),
+    $dt$ is the time between actions, which depends on the `frame_skip` parameter (default is 4),
+    and `frametime` which is $0.01$ - so the default is $dt = 4 \times 0.01 = 0.04$,
+    $w_{forward}$ is the `forward_reward_weight` (default is $1$).
+    - *ctrl_cost*:
+    A negative reward to penalize the Swimmer for taking actions that are too large.
+    $w_{control} \times \|action\|_2^2$,
+    where $w_{control}$ is `ctrl_cost_weight` (default is $10^{-4}$).
+
+    `info` contains the individual reward terms.
 
-    The total reward returned is ***reward*** *=* *forward_reward - ctrl_cost* and `info` will also contain the individual reward terms
 
     ## Starting State
-    All observations start in state (0,0,0,0,0,0,0,0) with a Uniform noise in the range of [-`reset_noise_scale`, `reset_noise_scale`] is added to the initial state for stochasticity.
+    The initial position state is $\mathcal{U}_{[-reset\_noise\_scale \times I_{5}, reset\_noise\_scale \times I_{5}]}$.
+    The initial velocity state is $\mathcal{U}_{[-reset\_noise\_scale \times I_{5}, reset\_noise\_scale \times I_{5}]}$.
 
-    ## Episode End
-    The episode truncates when the episode length is greater than 1000.
+    where $\mathcal{U}$ is the multivariate uniform continuous distribution.
 
-    ## Arguments
 
-    No additional arguments are currently supported in v2 and lower.
+    ## Episode End
+    ### Termination
+    The Swimmer never terminates.
+
+    ### Truncation
+    The default duration of an episode is 1000 timesteps.
 
-    ```python
-    import gymnasium as gym
-    gym.make('Swimmer-v4')
-    ```
 
-    v3 and v4 take `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc.
+    ## Arguments
+    Swimmer provides a range of parameters to modify the observation space, reward function, initial state, and termination condition.
+    These parameters can be applied during `gymnasium.make` in the following way:
 
     ```python
     import gymnasium as gym
-    env = gym.make('Swimmer-v4', ctrl_cost_weight=0.1, ....)
+    env = gym.make('Swimmer-v5', xml_file=...)
     ```
 
-    | Parameter                                    | Type      | Default         | Description                                                                                                                                                               |
-    | -------------------------------------------- | --------- | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-    | `xml_file`                                   | **str**   | `"swimmer.xml"` | Path to a MuJoCo model                                                                                                                                                    |
-    | `forward_reward_weight`                      | **float** | `1.0`           | Weight for _forward_reward_ term (see section on reward)                                                                                                                  |
-    | `ctrl_cost_weight`                           | **float** | `1e-4`          | Weight for _ctrl_cost_ term (see section on reward)                                                                                                                       |
-    | `reset_noise_scale`                          | **float** | `0.1`           | Scale of random perturbations of initial position and velocity (see section on Starting State)                                                                            |
-    | `exclude_current_positions_from_observation` | **bool**  | `True`          | Whether or not to omit the x- and y-coordinates from observations. Excluding the position can serve as an inductive bias to induce position-agnostic behavior in policies |
+    | Parameter                                  | Type      | Default       |Description                                                                                                                                                                                                  |
+    |--------------------------------------------| --------- |-------------- |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+    |`xml_file`                                  | **str**   |`"swimmer.xml"`| Path to a MuJoCo model                                                                                                                                                                                      |
+    |`forward_reward_weight`                     | **float** | `1`           | Weight for _forward_reward_ term (see `Rewards` section)                                                                                                                                                    |
+    |`ctrl_cost_weight`                          | **float** | `1e-4`        | Weight for _ctrl_cost_ term (see `Rewards` section)                                                                                                                                                         |
+    |`reset_noise_scale`                         | **float** | `0.1`         | Scale of random perturbations of initial position and velocity (see `Starting State` section)                                                                                                               |
+    |`exclude_current_positions_from_observation`| **bool**  | `True`        | Whether or not to omit the x- and y-coordinates from observations. Excluding the position can serve as an inductive bias to induce position-agnostic behavior in policies (see `Observation Space` section) |
 
 
     ## Version History
-
-    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3
-    * v3: Support for `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc. rgb rendering comes from tracking camera (so agent does not run away from screen)
-    * v2: All continuous control environments now use mujoco-py >= 1.50
+    * v5:
+        - Minimum `mujoco` version is now 2.3.3.
+        - Added support for fully custom/third party `mujoco` models using the `xml_file` argument (previously only a few changes could be made to the existing models).
+        - Added `default_camera_config` argument, a dictionary for setting the `mj_camera` properties, mainly useful for custom environments.
+        - Added `env.observation_structure`, a dictionary for specifying the observation space compose (e.g. `qpos`, `qvel`), useful for building tooling and wrappers for the MuJoCo environments.
+        - Return a non-empty `info` with `reset()`, previously an empty dictionary was returned, the new keys are the same state information as `step()`.
+        - Added `frame_skip` argument, used to configure the `dt` (duration of `step()`), default varies by environment check environment documentation pages.
+        - Restored the `xml_file` argument (was removed in `v4`).
+        - Added `forward_reward_weight`, `ctrl_cost_weight`, to configure the reward function (defaults are effectively the same as in `v4`).
+        - Added `reset_noise_scale` argument to set the range of initial states.
+        - Added `exclude_current_positions_from_observation` argument.
+        - Replaced `info["reward_fwd"]` and `info["forward_reward"]` with `info["reward_forward"]` to be consistent with the other environments.
+    * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3.
+    * v3: Support for `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc. rgb rendering comes from tracking camera (so agent does not run away from screen).
+    * v2: All continuous control environments now use mujoco-py >= 1.50.
     * v1: max_time_steps raised to 1000 for robot based tasks. Added reward_threshold to environments.
-    * v0: Initial versions release (1.0.0)
+    * v0: Initial versions release.
     """
 
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
-        "render_fps": 25,
     }
 
     def __init__(
         self,
-        forward_reward_weight=1.0,
-        ctrl_cost_weight=1e-4,
-        reset_noise_scale=0.1,
-        exclude_current_positions_from_observation=True,
+        xml_file: str = "swimmer.xml",
+        frame_skip: int = 4,
+        default_camera_config: Dict[str, Union[float, int]] = {},
+        forward_reward_weight: float = 1.0,
+        ctrl_cost_weight: float = 1e-4,
+        reset_noise_scale: float = 0.1,
+        exclude_current_positions_from_observation: bool = True,
         **kwargs,
     ):
         utils.EzPickle.__init__(
             self,
+            xml_file,
+            frame_skip,
+            default_camera_config,
             forward_reward_weight,
             ctrl_cost_weight,
             reset_noise_scale,
             exclude_current_positions_from_observation,
             **kwargs,
         )
 
@@ -155,63 +178,93 @@
         self._ctrl_cost_weight = ctrl_cost_weight
 
         self._reset_noise_scale = reset_noise_scale
 
         self._exclude_current_positions_from_observation = (
             exclude_current_positions_from_observation
         )
-        if exclude_current_positions_from_observation:
-            observation_space = Box(
-                low=-np.inf, high=np.inf, shape=(8,), dtype=np.float64
-            )
-        else:
-            observation_space = Box(
-                low=-np.inf, high=np.inf, shape=(10,), dtype=np.float64
-            )
+
         MujocoEnv.__init__(
-            self, "swimmer.xml", 4, observation_space=observation_space, **kwargs
+            self,
+            xml_file,
+            frame_skip,
+            observation_space=None,
+            default_camera_config=default_camera_config,
+            **kwargs,
         )
 
+        self.metadata = {
+            "render_modes": [
+                "human",
+                "rgb_array",
+                "depth_array",
+            ],
+            "render_fps": int(np.round(1.0 / self.dt)),
+        }
+
+        obs_size = (
+            self.data.qpos.size
+            + self.data.qvel.size
+            - 2 * exclude_current_positions_from_observation
+        )
+        self.observation_space = Box(
+            low=-np.inf, high=np.inf, shape=(obs_size,), dtype=np.float64
+        )
+
+        self.observation_structure = {
+            "skipped_qpos": 2 * exclude_current_positions_from_observation,
+            "qpos": self.data.qpos.size
+            - 2 * exclude_current_positions_from_observation,
+            "qvel": self.data.qvel.size,
+        }
+
     def control_cost(self, action):
         control_cost = self._ctrl_cost_weight * np.sum(np.square(action))
         return control_cost
 
     def step(self, action):
         xy_position_before = self.data.qpos[0:2].copy()
         self.do_simulation(action, self.frame_skip)
         xy_position_after = self.data.qpos[0:2].copy()
 
         xy_velocity = (xy_position_after - xy_position_before) / self.dt
         x_velocity, y_velocity = xy_velocity
 
-        forward_reward = self._forward_reward_weight * x_velocity
-
-        ctrl_cost = self.control_cost(action)
-
         observation = self._get_obs()
-        reward = forward_reward - ctrl_cost
+        reward, reward_info = self._get_rew(x_velocity, action)
         info = {
-            "reward_fwd": forward_reward,
-            "reward_ctrl": -ctrl_cost,
             "x_position": xy_position_after[0],
             "y_position": xy_position_after[1],
             "distance_from_origin": np.linalg.norm(xy_position_after, ord=2),
             "x_velocity": x_velocity,
             "y_velocity": y_velocity,
-            "forward_reward": forward_reward,
+            **reward_info,
         }
 
         if self.render_mode == "human":
             self.render()
-
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return observation, reward, False, False, info
 
+    def _get_rew(self, x_velocity: float, action):
+        forward_reward = self._forward_reward_weight * x_velocity
+        ctrl_cost = self.control_cost(action)
+
+        reward = forward_reward - ctrl_cost
+
+        reward_info = {
+            "reward_forward": forward_reward,
+            "reward_ctrl": -ctrl_cost,
+        }
+
+        return reward, reward_info
+
     def _get_obs(self):
-        position = self.data.qpos.flat.copy()
-        velocity = self.data.qvel.flat.copy()
+        position = self.data.qpos.flatten()
+        velocity = self.data.qvel.flatten()
 
         if self._exclude_current_positions_from_observation:
             position = position[2:]
 
         observation = np.concatenate([position, velocity]).ravel()
         return observation
 
@@ -226,7 +279,14 @@
             low=noise_low, high=noise_high, size=self.model.nv
         )
 
         self.set_state(qpos, qvel)
 
         observation = self._get_obs()
         return observation
+
+    def _get_reset_info(self):
+        return {
+            "x_position": self.data.qpos[0],
+            "y_position": self.data.qpos[1],
+            "distance_from_origin": np.linalg.norm(self.data.qpos[0:2], ord=2),
+        }
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/walker2d.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/humanoidstandup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,88 @@
 import numpy as np
 
 from gymnasium import utils
 from gymnasium.envs.mujoco import MuJocoPyEnv
 from gymnasium.spaces import Box
 
 
-class Walker2dEnv(MuJocoPyEnv, utils.EzPickle):
+class HumanoidStandupEnv(MuJocoPyEnv, utils.EzPickle):
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
-        "render_fps": 125,
+        "render_fps": 67,
     }
 
     def __init__(self, **kwargs):
-        observation_space = Box(low=-np.inf, high=np.inf, shape=(17,), dtype=np.float64)
+        observation_space = Box(
+            low=-np.inf, high=np.inf, shape=(376,), dtype=np.float64
+        )
         MuJocoPyEnv.__init__(
-            self, "walker2d.xml", 4, observation_space=observation_space, **kwargs
+            self,
+            "humanoidstandup.xml",
+            5,
+            observation_space=observation_space,
+            **kwargs,
         )
         utils.EzPickle.__init__(self, **kwargs)
 
+    def _get_obs(self):
+        data = self.sim.data
+        return np.concatenate(
+            [
+                data.qpos.flat[2:],
+                data.qvel.flat,
+                data.cinert.flat,
+                data.cvel.flat,
+                data.qfrc_actuator.flat,
+                data.cfrc_ext.flat,
+            ]
+        )
+
     def step(self, a):
-        posbefore = self.sim.data.qpos[0]
         self.do_simulation(a, self.frame_skip)
-        posafter, height, ang = self.sim.data.qpos[0:3]
-
-        alive_bonus = 1.0
-        reward = (posafter - posbefore) / self.dt
-        reward += alive_bonus
-        reward -= 1e-3 * np.square(a).sum()
-        terminated = not (height > 0.8 and height < 2.0 and ang > -1.0 and ang < 1.0)
-        ob = self._get_obs()
+        pos_after = self.sim.data.qpos[2]
+        data = self.sim.data
+        uph_cost = (pos_after - 0) / self.model.opt.timestep
+
+        quad_ctrl_cost = 0.1 * np.square(data.ctrl).sum()
+        quad_impact_cost = 0.5e-6 * np.square(data.cfrc_ext).sum()
+        quad_impact_cost = min(quad_impact_cost, 10)
+        reward = uph_cost - quad_ctrl_cost - quad_impact_cost + 1
 
         if self.render_mode == "human":
             self.render()
-
-        return ob, reward, terminated, False, {}
-
-    def _get_obs(self):
-        qpos = self.sim.data.qpos
-        qvel = self.sim.data.qvel
-        return np.concatenate([qpos[1:], np.clip(qvel, -10, 10)]).ravel()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
+        return (
+            self._get_obs(),
+            reward,
+            False,
+            False,
+            dict(
+                reward_linup=uph_cost,
+                reward_quadctrl=-quad_ctrl_cost,
+                reward_impact=-quad_impact_cost,
+            ),
+        )
 
     def reset_model(self):
+        c = 0.01
         self.set_state(
-            self.init_qpos
-            + self.np_random.uniform(low=-0.005, high=0.005, size=self.model.nq),
+            self.init_qpos + self.np_random.uniform(low=-c, high=c, size=self.model.nq),
             self.init_qvel
-            + self.np_random.uniform(low=-0.005, high=0.005, size=self.model.nv),
+            + self.np_random.uniform(
+                low=-c,
+                high=c,
+                size=self.model.nv,
+            ),
         )
         return self._get_obs()
 
     def viewer_setup(self):
         assert self.viewer is not None
-        self.viewer.cam.trackbodyid = 2
-        self.viewer.cam.distance = self.model.stat.extent * 0.5
-        self.viewer.cam.lookat[2] = 1.15
+        self.viewer.cam.trackbodyid = 1
+        self.viewer.cam.distance = self.model.stat.extent * 1.0
+        self.viewer.cam.lookat[2] = 0.8925
         self.viewer.cam.elevation = -20
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/walker2d_v3.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/walker2d_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         info = {
             "x_position": x_position_after,
             "x_velocity": x_velocity,
         }
 
         if self.render_mode == "human":
             self.render()
-
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return observation, reward, terminated, False, info
 
     def reset_model(self):
         noise_low = -self._reset_noise_scale
         noise_high = self._reset_noise_scale
 
         qpos = self.init_qpos + self.np_random.uniform(
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/mujoco/walker2d_v4.py` & `gymnasium-1.0.0a1/gymnasium/envs/mujoco/walker2d_v5.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+__credits__ = ["Kallinteris-Andreas"]
+
+from typing import Dict, Tuple, Union
+
 import numpy as np
 
 from gymnasium import utils
 from gymnasium.envs.mujoco import MujocoEnv
 from gymnasium.spaces import Box
 
 
@@ -10,55 +14,54 @@
     "distance": 4.0,
     "lookat": np.array((0.0, 0.0, 1.15)),
     "elevation": -20.0,
 }
 
 
 class Walker2dEnv(MujocoEnv, utils.EzPickle):
-    """
+    r"""
     ## Description
+    This environment builds on the [hopper](https://gymnasium.farama.org/environments/mujoco/hopper/) environment by adding another set of legs that allow the robot to walk forward instead of hop.
+    Like other MuJoCo environments, this environment aims to increase the number of independent state and control variables compared to classical control environments.
+    The walker is a two-dimensional bipedal robot consisting of seven main body parts - a single torso at the top (with the two legs splitting after the torso), two thighs in the middle below the torso, two legs below the thighs, and two feet attached to the legs on which the entire body rests.
+    The goal is to walk in the forward (right) direction by applying torque to the six hinges connecting the seven body parts.
 
-    This environment builds on the [hopper](https://gymnasium.farama.org/environments/mujoco/hopper/) environment
-    by adding another set of legs making it possible for the robot to walk forward instead of
-    hop. Like other Mujoco environments, this environment aims to increase the number of independent state
-    and control variables as compared to the classic control environments. The walker is a
-    two-dimensional two-legged figure that consist of seven main body parts - a single torso at the top
-    (with the two legs splitting after the torso), two thighs in the middle below the torso, two legs
-    in the bottom below the thighs, and two feet attached to the legs on which the entire body rests.
-    The goal is to walk in the in the forward (right)
-    direction by applying torques on the six hinges connecting the seven body parts.
 
     ## Action Space
+    ```{figure} action_space_figures/walker2d.png
+    :name: walker2d
+    ```
+
     The action space is a `Box(-1, 1, (6,), float32)`. An action represents the torques applied at the hinge joints.
 
-    | Num | Action                                 | Control Min | Control Max | Name (in corresponding XML file) | Joint | Unit         |
+    | Num | Action                                 | Control Min | Control Max | Name (in corresponding XML file) | Joint | Type (Unit)  |
     |-----|----------------------------------------|-------------|-------------|----------------------------------|-------|--------------|
     | 0   | Torque applied on the thigh rotor      | -1          | 1           | thigh_joint                      | hinge | torque (N m) |
     | 1   | Torque applied on the leg rotor        | -1          | 1           | leg_joint                        | hinge | torque (N m) |
     | 2   | Torque applied on the foot rotor       | -1          | 1           | foot_joint                       | hinge | torque (N m) |
     | 3   | Torque applied on the left thigh rotor | -1          | 1           | thigh_left_joint                 | hinge | torque (N m) |
     | 4   | Torque applied on the left leg rotor   | -1          | 1           | leg_left_joint                   | hinge | torque (N m) |
     | 5   | Torque applied on the left foot rotor  | -1          | 1           | foot_left_joint                  | hinge | torque (N m) |
 
+
     ## Observation Space
-    Observations consist of positional values of different body parts of the walker,
-    followed by the velocities of those individual parts (their derivatives) with all the positions ordered before all the velocities.
+    The observation space consists of the following parts (in order):
 
-    By default, observations do not include the x-coordinate of the torso. It may
-    be included by passing `exclude_current_positions_from_observation=False` during construction.
-    In that case, the observation space will be `Box(-Inf, Inf, (18,), float64)` where the first observation
-    represent the x-coordinates of the torso of the walker.
-    Regardless of whether `exclude_current_positions_from_observation` was set to true or false, the x-coordinate
-    of the torso will be returned in `info` with key `"x_position"`.
+    - *qpos (8 elements by default):* Position values of the robot's body parts.
+    - *qvel (9 elements):* The velocities of these individual body parts (their derivatives).
 
-    By default, observation is a `Box(-Inf, Inf, (17,), float64)` where the elements correspond to the following:
+    By default, the observation does not include the robot's x-coordinate (`rootx`).
+    This can be included by passing `exclude_current_positions_from_observation=False` during construction.
+    In this case, the observation space will be a `Box(-Inf, Inf, (18,), float64)`, where the first observation element is the x-coordinate of the robot.
+    Regardless of whether `exclude_current_positions_from_observation` is set to `True` or `False`, the x-coordinate are returned in `info` with the keys `"x_position"` and `"y_position"`, respectively.
 
-    | Num | Observation                                        | Min  | Max | Name (in corresponding XML file) | Joint | Unit                     |
+    By default, however, the observation space is a `Box(-Inf, Inf, (17,), float64)` where the elements are as follows:
+
+    | Num | Observation                                        | Min  | Max | Name (in corresponding XML file) | Joint | Type (Unit)              |
     | --- | -------------------------------------------------- | ---- | --- | -------------------------------- | ----- | ------------------------ |
-    | excluded | x-coordinate of the torso                     | -Inf | Inf | rootx                            | slide | position (m)             |
     | 0   | z-coordinate of the torso (height of Walker2d)     | -Inf | Inf | rootz                            | slide | position (m)             |
     | 1   | angle of the torso                                 | -Inf | Inf | rooty                            | hinge | angle (rad)              |
     | 2   | angle of the thigh joint                           | -Inf | Inf | thigh_joint                      | hinge | angle (rad)              |
     | 3   | angle of the leg joint                             | -Inf | Inf | leg_joint                        | hinge | angle (rad)              |
     | 4   | angle of the foot joint                            | -Inf | Inf | foot_joint                       | hinge | angle (rad)              |
     | 5   | angle of the left thigh joint                      | -Inf | Inf | thigh_left_joint                 | hinge | angle (rad)              |
     | 6   | angle of the left leg joint                        | -Inf | Inf | leg_left_joint                   | hinge | angle (rad)              |
@@ -68,111 +71,130 @@
     | 10  | angular velocity of the angle of the torso         | -Inf | Inf | rooty                            | hinge | angular velocity (rad/s) |
     | 11  | angular velocity of the thigh hinge                | -Inf | Inf | thigh_joint                      | hinge | angular velocity (rad/s) |
     | 12  | angular velocity of the leg hinge                  | -Inf | Inf | leg_joint                        | hinge | angular velocity (rad/s) |
     | 13  | angular velocity of the foot hinge                 | -Inf | Inf | foot_joint                       | hinge | angular velocity (rad/s) |
     | 14  | angular velocity of the thigh hinge                | -Inf | Inf | thigh_left_joint                 | hinge | angular velocity (rad/s) |
     | 15  | angular velocity of the leg hinge                  | -Inf | Inf | leg_left_joint                   | hinge | angular velocity (rad/s) |
     | 16  | angular velocity of the foot hinge                 | -Inf | Inf | foot_left_joint                  | hinge | angular velocity (rad/s) |
+    | excluded | x-coordinate of the torso                     | -Inf | Inf | rootx                            | slide | position (m)             |
+
 
     ## Rewards
-    The reward consists of three parts:
-    - *healthy_reward*: Every timestep that the walker is alive, it receives a fixed reward of value `healthy_reward`,
-    - *forward_reward*: A reward of walking forward which is measured as
-    *`forward_reward_weight` * (x-coordinate before action - x-coordinate after action)/dt*.
-    *dt* is the time between actions and is dependeent on the frame_skip parameter
-    (default is 4), where the frametime is 0.002 - making the default
-    *dt = 4 * 0.002 = 0.008*. This reward would be positive if the walker walks forward (positive x direction).
-    - *ctrl_cost*: A cost for penalising the walker if it
-    takes actions that are too large. It is measured as
-    *`ctrl_cost_weight` * sum(action<sup>2</sup>)* where *`ctrl_cost_weight`* is
-    a parameter set for the control and has a default value of 0.001
+    The total reward is: ***reward*** *=* *healthy_reward bonus + forward_reward - ctrl_cost*.
 
-    The total reward returned is ***reward*** *=* *healthy_reward bonus + forward_reward - ctrl_cost* and `info` will also contain the individual reward terms
+    - *healthy_reward*:
+    Every timestep that the Walker2d is alive, it receives a fixed reward of value `healthy_reward` (default is $1$),
+    - *forward_reward*:
+    A reward for moving forward,
+    this reward would be positive if the Swimmer moves forward (in the positive $x$ direction / in the right direction).
+    $w_{forward} \times \frac{dx}{dt}$, where
+    $dx$ is the displacement of the (front) "tip" ($x_{after-action} - x_{before-action}$),
+    $dt$ is the time between actions, which depends on the `frame_skip` parameter (default is $4$),
+    and `frametime` which is $0.002$ - so the default is $dt = 4 \times 0.002 = 0.008$,
+    $w_{forward}$ is the `forward_reward_weight` (default is $1$).
+    - *ctrl_cost*:
+    A negative reward to penalize the Walker2d for taking actions that are too large.
+    $w_{control} \times \|action\|_2^2$,
+    where $w_{control}$ is `ctrl_cost_weight` (default is $10^{-3}$).
 
-    ## Starting State
-    All observations start in state
-    (0.0, 1.25, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0)
-    with a uniform noise in the range of [-`reset_noise_scale`, `reset_noise_scale`] added to the values for stochasticity.
+    `info` contains the individual reward terms.
 
-    ## Episode End
-    The walker is said to be unhealthy if any of the following happens:
 
-    1. Any of the state space values is no longer finite
-    2. The height of the walker is ***not*** in the closed interval specified by `healthy_z_range`
-    3. The absolute value of the angle (`observation[1]` if `exclude_current_positions_from_observation=False`, else `observation[2]`) is ***not*** in the closed interval specified by `healthy_angle_range`
+    ## Starting State
+    The initial position state is $[0, 1.25, 0, 0, 0, 0, 0, 0, 0] + \mathcal{U}_{[-reset\_noise\_scale \times I_{9}, reset\_noise\_scale \times I_{9}]}$.
+    The initial velocity state is $\mathcal{U}_{[-reset\_noise\_scale \times I_{9}, reset\_noise\_scale \times I_{9}]}$.
 
-    If `terminate_when_unhealthy=True` is passed during construction (which is the default),
-    the episode ends when any of the following happens:
+    where $\mathcal{U}$ is the multivariate uniform continuous distribution.
 
-    1. Truncation: The episode duration reaches a 1000 timesteps
-    2. Termination: The walker is unhealthy
+    Note that the z-coordinate is non-zero so that the Walker2d can stand up immediately.
 
-    If `terminate_when_unhealthy=False` is passed, the episode is ended only when 1000 timesteps are exceeded.
 
-    ## Arguments
+    ## Episode End
+    ### Termination
+    If `terminate_when_unhealthy is True` (which is the default), the environment terminates when the Walker2d is unhealthy.
+    The Walker2d is unhealthy if any of the following happens:
 
-    No additional arguments are currently supported in v2 and lower.
+    1. Any of the state space values is no longer finite
+    2. The z-coordinate of the torso (the height) is **not** in the closed interval given by the `healthy_z_range` argument (default to $[0.8, 1.0]$).
+    3. The absolute value of the angle (`observation[1]` if `exclude_current_positions_from_observation=False`, else `observation[2]`) is ***not*** in the closed interval specified by the `healthy_angle_range` argument (default is $[-1, 1]$).
+
+    ### Truncation
+    The default duration of an episode is 1000 timesteps.
 
-    ```python
-    import gymnasium as gym
-    env = gym.make('Walker2d-v4')
-    ```
 
-    v3 and beyond take `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc.
+    ## Arguments
+    Walker2d provides a range of parameters to modify the observation space, reward function, initial state, and termination condition.
+    These parameters can be applied during `gymnasium.make` in the following way:
 
     ```python
     import gymnasium as gym
-    env = gym.make('Walker2d-v4', ctrl_cost_weight=0.1, ....)
+    env = gym.make('Walker2d-v5', ctrl_cost_weight=1e-3, ...)
     ```
 
-    | Parameter                                    | Type      | Default          | Description                                                                                                                                                       |
-    | -------------------------------------------- | --------- | ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-    | `xml_file`                                   | **str**   | `"walker2d.xml"` | Path to a MuJoCo model                                                                                                                                            |
-    | `forward_reward_weight`                      | **float** | `1.0`            | Weight for _forward_reward_ term (see section on reward)                                                                                                          |
-    | `ctrl_cost_weight`                           | **float** | `1e-3`           | Weight for _ctr_cost_ term (see section on reward)                                                                                                                |
-    | `healthy_reward`                             | **float** | `1.0`            | Constant reward given if the ant is "healthy" after timestep                                                                                                      |
-    | `terminate_when_unhealthy`                   | **bool**  | `True`           | If true, issue a done signal if the z-coordinate of the walker is no longer healthy                                                                               |
-    | `healthy_z_range`                            | **tuple** | `(0.8, 2)`       | The z-coordinate of the torso of the walker must be in this range to be considered healthy                                                                        |
-    | `healthy_angle_range`                        | **tuple** | `(-1, 1)`        | The angle must be in this range to be considered healthy                                                                                                          |
-    | `reset_noise_scale`                          | **float** | `5e-3`           | Scale of random perturbations of initial position and velocity (see section on Starting State)                                                                    |
-    | `exclude_current_positions_from_observation` | **bool**  | `True`           | Whether or not to omit the x-coordinate from observations. Excluding the position can serve as an inductive bias to induce position-agnostic behavior in policies |
+    | Parameter                                    | Type      | Default           | Description                                                                                                                                                                                         |
+    | -------------------------------------------- | --------- | ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+    | `xml_file`                                   | **str**   |`"walker2d_v5.xml"`| Path to a MuJoCo model                                                                                                                                                                              |
+    | `forward_reward_weight`                      | **float** | `1`               | Weight for _forward_reward_ term (see `Rewards` section)                                                                                                                                            |
+    | `ctrl_cost_weight`                           | **float** | `1e-3`            | Weight for _ctr_cost_ term (see `Rewards` section)                                                                                                                                                  |
+    | `healthy_reward`                             | **float** | `1`               | Weight for _healthy_reward_ reward (see `Rewards` section)                                                                                                                                          |
+    | `terminate_when_unhealthy`                   | **bool**  | `True`            | If True, issue a `terminated` signal is unhealthy (see `Episode End` section)                                                                                                                          |
+    | `healthy_z_range`                            | **tuple** | `(0.8, 2)`        | The z-coordinate of the torso of the walker must be in this range to be considered healthy (see `Episode End` section)                                                                              |
+    | `healthy_angle_range`                        | **tuple** | `(-1, 1)`         | The angle must be in this range to be considered healthy (see `Episode End` section)                                                                                                                |
+    | `reset_noise_scale`                          | **float** | `5e-3`            | Scale of random perturbations of initial position and velocity (see `Starting State` section)                                                                                                       |
+    | `exclude_current_positions_from_observation` | **bool**  | `True`            | Whether or not to omit the x-coordinate from observations. Excluding the position can serve as an inductive bias to induce position-agnostic behavior in policies (see `Observation Space` section) |
 
 
     ## Version History
-
+    * v5:
+        - Minimum `mujoco` version is now 2.3.3.
+        - Added support for fully custom/third party `mujoco` models using the `xml_file` argument (previously only a few changes could be made to the existing models).
+        - Added `default_camera_config` argument, a dictionary for setting the `mj_camera` properties, mainly useful for custom environments.
+        - Added `env.observation_structure`, a dictionary for specifying the observation space compose (e.g. `qpos`, `qvel`), useful for building tooling and wrappers for the MuJoCo environments.
+        - Return a non-empty `info` with `reset()`, previously an empty dictionary was returned, the new keys are the same state information as `step()`.
+        - Added `frame_skip` argument, used to configure the `dt` (duration of `step()`), default varies by environment check environment documentation pages.
+        - In v2, v3 and v4 the models have different friction values for the two feet (left foot friction == 1.9 and right foot friction == 0.9). The `Walker-v5` model is updated to have the same friction for both feet (set to 1.9). This causes the Walker2d's the right foot to slide less on the surface and therefore require more force to move (related [GitHub issue](https://github.com/Farama-Foundation/Gymnasium/issues/477)).
+        - Fixed bug: `healthy_reward` was given on every step (even if the Walker2D is unhealthy), now it is only given if the Walker2d is healthy. The `info` "reward_survive" is updated with this change (related [GitHub issue](https://github.com/Farama-Foundation/Gymnasium/issues/526)).
+        - Restored the `xml_file` argument (was removed in `v4`).
+        - Added individual reward terms in `info` (`info["reward_forward"]`, info`["reward_ctrl"]`, `info["reward_survive"]`).
+        - Added `info["z_distance_from_origin"]` which is equal to the vertical distance of the "torso" body from its initial position.
     * v4: All MuJoCo environments now use the MuJoCo bindings in mujoco >= 2.1.3
     * v3: Support for `gymnasium.make` kwargs such as `xml_file`, `ctrl_cost_weight`, `reset_noise_scale`, etc. rgb rendering comes from tracking camera (so agent does not run away from screen)
     * v2: All continuous control environments now use mujoco-py >= 1.50
     * v1: max_time_steps raised to 1000 for robot based tasks. Added reward_threshold to environments.
-    * v0: Initial versions release (1.0.0)
+    * v0: Initial versions release
     """
 
     metadata = {
         "render_modes": [
             "human",
             "rgb_array",
             "depth_array",
         ],
-        "render_fps": 125,
     }
 
     def __init__(
         self,
-        forward_reward_weight=1.0,
-        ctrl_cost_weight=1e-3,
-        healthy_reward=1.0,
-        terminate_when_unhealthy=True,
-        healthy_z_range=(0.8, 2.0),
-        healthy_angle_range=(-1.0, 1.0),
-        reset_noise_scale=5e-3,
-        exclude_current_positions_from_observation=True,
+        xml_file: str = "walker2d_v5.xml",
+        frame_skip: int = 4,
+        default_camera_config: Dict[str, Union[float, int]] = DEFAULT_CAMERA_CONFIG,
+        forward_reward_weight: float = 1.0,
+        ctrl_cost_weight: float = 1e-3,
+        healthy_reward: float = 1.0,
+        terminate_when_unhealthy: bool = True,
+        healthy_z_range: Tuple[float, float] = (0.8, 2.0),
+        healthy_angle_range: Tuple[float, float] = (-1.0, 1.0),
+        reset_noise_scale: float = 5e-3,
+        exclude_current_positions_from_observation: bool = True,
         **kwargs,
     ):
         utils.EzPickle.__init__(
             self,
+            xml_file,
+            frame_skip,
+            default_camera_config,
             forward_reward_weight,
             ctrl_cost_weight,
             healthy_reward,
             terminate_when_unhealthy,
             healthy_z_range,
             healthy_angle_range,
             reset_noise_scale,
@@ -191,38 +213,51 @@
 
         self._reset_noise_scale = reset_noise_scale
 
         self._exclude_current_positions_from_observation = (
             exclude_current_positions_from_observation
         )
 
-        if exclude_current_positions_from_observation:
-            observation_space = Box(
-                low=-np.inf, high=np.inf, shape=(17,), dtype=np.float64
-            )
-        else:
-            observation_space = Box(
-                low=-np.inf, high=np.inf, shape=(18,), dtype=np.float64
-            )
-
         MujocoEnv.__init__(
             self,
-            "walker2d.xml",
-            4,
-            observation_space=observation_space,
-            default_camera_config=DEFAULT_CAMERA_CONFIG,
+            xml_file,
+            frame_skip,
+            observation_space=None,
+            default_camera_config=default_camera_config,
             **kwargs,
         )
 
+        self.metadata = {
+            "render_modes": [
+                "human",
+                "rgb_array",
+                "depth_array",
+            ],
+            "render_fps": int(np.round(1.0 / self.dt)),
+        }
+
+        obs_size = (
+            self.data.qpos.size
+            + self.data.qvel.size
+            - exclude_current_positions_from_observation
+        )
+        self.observation_space = Box(
+            low=-np.inf, high=np.inf, shape=(obs_size,), dtype=np.float64
+        )
+
+        self.observation_structure = {
+            "skipped_qpos": 1 * exclude_current_positions_from_observation,
+            "qpos": self.data.qpos.size
+            - 1 * exclude_current_positions_from_observation,
+            "qvel": self.data.qvel.size,
+        }
+
     @property
     def healthy_reward(self):
-        return (
-            float(self.is_healthy or self._terminate_when_unhealthy)
-            * self._healthy_reward
-        )
+        return self.is_healthy * self._healthy_reward
 
     def control_cost(self, action):
         control_cost = self._ctrl_cost_weight * np.sum(np.square(action))
         return control_cost
 
     @property
     def is_healthy(self):
@@ -233,56 +268,62 @@
 
         healthy_z = min_z < z < max_z
         healthy_angle = min_angle < angle < max_angle
         is_healthy = healthy_z and healthy_angle
 
         return is_healthy
 
-    @property
-    def terminated(self):
-        terminated = not self.is_healthy if self._terminate_when_unhealthy else False
-        return terminated
-
     def _get_obs(self):
-        position = self.data.qpos.flat.copy()
-        velocity = np.clip(self.data.qvel.flat.copy(), -10, 10)
+        position = self.data.qpos.flatten()
+        velocity = np.clip(self.data.qvel.flatten(), -10, 10)
 
         if self._exclude_current_positions_from_observation:
             position = position[1:]
 
         observation = np.concatenate((position, velocity)).ravel()
         return observation
 
     def step(self, action):
         x_position_before = self.data.qpos[0]
         self.do_simulation(action, self.frame_skip)
         x_position_after = self.data.qpos[0]
         x_velocity = (x_position_after - x_position_before) / self.dt
 
-        ctrl_cost = self.control_cost(action)
-
-        forward_reward = self._forward_reward_weight * x_velocity
-        healthy_reward = self.healthy_reward
-
-        rewards = forward_reward + healthy_reward
-        costs = ctrl_cost
-
         observation = self._get_obs()
-        reward = rewards - costs
-        terminated = self.terminated
+        reward, reward_info = self._get_rew(x_velocity, action)
+        terminated = (not self.is_healthy) and self._terminate_when_unhealthy
         info = {
             "x_position": x_position_after,
+            "z_distance_from_origin": self.data.qpos[1] - self.init_qpos[1],
             "x_velocity": x_velocity,
+            **reward_info,
         }
 
         if self.render_mode == "human":
             self.render()
-
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return observation, reward, terminated, False, info
 
+    def _get_rew(self, x_velocity: float, action):
+        forward_reward = self._forward_reward_weight * x_velocity
+        healthy_reward = self.healthy_reward
+        rewards = forward_reward + healthy_reward
+
+        ctrl_cost = self.control_cost(action)
+        costs = ctrl_cost
+        reward = rewards - costs
+
+        reward_info = {
+            "reward_forward": forward_reward,
+            "reward_ctrl": -ctrl_cost,
+            "reward_survive": healthy_reward,
+        }
+
+        return reward, reward_info
+
     def reset_model(self):
         noise_low = -self._reset_noise_scale
         noise_high = self._reset_noise_scale
 
         qpos = self.init_qpos + self.np_random.uniform(
             low=noise_low, high=noise_high, size=self.model.nq
         )
@@ -290,7 +331,13 @@
             low=noise_low, high=noise_high, size=self.model.nv
         )
 
         self.set_state(qpos, qvel)
 
         observation = self._get_obs()
         return observation
+
+    def _get_reset_info(self):
+        return {
+            "x_position": self.data.qpos[0],
+            "z_distance_from_origin": self.data.qpos[1] - self.init_qpos[1],
+        }
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/phys2d/assets/clockwise.png` & `gymnasium-1.0.0a1/gymnasium/envs/phys2d/assets/clockwise.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/phys2d/pendulum.py` & `gymnasium-1.0.0a1/gymnasium/envs/phys2d/pendulum.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,116 +3,134 @@
 
 from os import path
 from typing import Any, Optional, Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
+from flax import struct
 from jax.random import PRNGKey
 
 import gymnasium as gym
+from gymnasium.envs.functional_jax_env import FunctionalJaxEnv, FunctionalJaxVectorEnv
 from gymnasium.error import DependencyNotInstalled
-from gymnasium.experimental.functional import ActType, FuncEnv, StateType
-from gymnasium.experimental.functional_jax_env import (
-    FunctionalJaxEnv,
-    FunctionalJaxVectorEnv,
-)
+from gymnasium.functional import ActType, FuncEnv, StateType
 from gymnasium.utils import EzPickle
 
 
 RenderStateType = Tuple["pygame.Surface", "pygame.time.Clock", Optional[float]]  # type: ignore  # noqa: F821
 
 
+@struct.dataclass
+class PendulumParams:
+    """Parameters for the jax Pendulum environment."""
+
+    max_speed: float = 8.0
+    dt: float = 0.05
+    g: float = 10.0
+    m: float = 1.0
+    l: float = 1.0
+    high_x: float = jnp.pi
+    high_y: float = 1.0
+    screen_dim: int = 500
+
+
 class PendulumFunctional(
-    FuncEnv[jax.Array, jax.Array, int, float, bool, RenderStateType]
+    FuncEnv[jax.Array, jax.Array, int, float, bool, RenderStateType, PendulumParams]
 ):
     """Pendulum but in jax and functional structure."""
 
-    max_speed = 8
-    max_torque = 2.0
-    dt = 0.05
-    g = 10.0
-    m = 1.0
-    l = 1.0
-    high_x = jnp.pi
-    high_y = 1.0
-
-    screen_dim = 500
+    max_torque: float = 2.0
 
     observation_space = gym.spaces.Box(-np.inf, np.inf, shape=(3,), dtype=np.float32)
     action_space = gym.spaces.Box(-max_torque, max_torque, shape=(1,), dtype=np.float32)
 
-    def initial(self, rng: PRNGKey):
+    def initial(self, rng: PRNGKey, params: PendulumParams = PendulumParams):
         """Initial state generation."""
-        high = jnp.array([self.high_x, self.high_y])
+        high = jnp.array([params.high_x, params.high_y])
         return jax.random.uniform(key=rng, minval=-high, maxval=high, shape=high.shape)
 
     def transition(
-        self, state: jax.Array, action: int | jax.Array, rng: None = None
+        self,
+        state: jax.Array,
+        action: int | jax.Array,
+        rng: None = None,
+        params: PendulumParams = PendulumParams,
     ) -> jax.Array:
         """Pendulum transition."""
         th, thdot = state  # th := theta
         u = action
 
-        g = self.g
-        m = self.m
-        l = self.l
-        dt = self.dt
+        g = params.g
+        m = params.m
+        l = params.l
+        dt = params.dt
 
         u = jnp.clip(u, -self.max_torque, self.max_torque)[0]
 
         newthdot = thdot + (3 * g / (2 * l) * jnp.sin(th) + 3.0 / (m * l**2) * u) * dt
-        newthdot = jnp.clip(newthdot, -self.max_speed, self.max_speed)
+        newthdot = jnp.clip(newthdot, -params.max_speed, params.max_speed)
         newth = th + newthdot * dt
 
         new_state = jnp.array([newth, newthdot])
         return new_state
 
-    def observation(self, state: jax.Array) -> jax.Array:
+    def observation(
+        self, state: jax.Array, params: PendulumParams = PendulumParams
+    ) -> jax.Array:
         """Generates an observation based on the state."""
         theta, thetadot = state
         return jnp.array([jnp.cos(theta), jnp.sin(theta), thetadot])
 
-    def reward(self, state: StateType, action: ActType, next_state: StateType) -> float:
+    def reward(
+        self,
+        state: StateType,
+        action: ActType,
+        next_state: StateType,
+        params: PendulumParams = PendulumParams,
+    ) -> float:
         """Generates the reward based on the state, action and next state."""
         th, thdot = state  # th := theta
         u = action
 
         u = jnp.clip(u, -self.max_torque, self.max_torque)[0]
 
         th_normalized = ((th + jnp.pi) % (2 * jnp.pi)) - jnp.pi
         costs = th_normalized**2 + 0.1 * thdot**2 + 0.001 * (u**2)
 
         return -costs
 
-    def terminal(self, state: StateType) -> bool:
+    def terminal(
+        self, state: StateType, params: PendulumParams = PendulumParams
+    ) -> bool:
         """Determines if the state is a terminal state."""
         return False
 
     def render_image(
         self,
         state: StateType,
-        render_state: tuple[pygame.Surface, pygame.time.Clock, float | None],  # type: ignore  # noqa: F821
+        render_state: RenderStateType,
+        params: PendulumParams = PendulumParams,
     ) -> tuple[RenderStateType, np.ndarray]:
         """Renders an RGB image."""
         try:
             import pygame
             from pygame import gfxdraw
         except ImportError as e:
             raise DependencyNotInstalled(
                 "pygame is not installed, run `pip install gymnasium[classic-control]`"
             ) from e
         screen, clock, last_u = render_state
 
-        surf = pygame.Surface((self.screen_dim, self.screen_dim))
+        surf = pygame.Surface((params.screen_dim, params.screen_dim))
         surf.fill((255, 255, 255))
 
         bound = 2.2
-        scale = self.screen_dim / (bound * 2)
-        offset = self.screen_dim // 2
+        scale = params.screen_dim / (bound * 2)
+        offset = params.screen_dim // 2
 
         rod_length = 1 * scale
         rod_width = 0.2 * scale
         l, r, t, b = 0, rod_length, rod_width / 2, -rod_width / 2
         coords = [(l, b), (l, t), (r, t), (r, b)]
         transformed_coords = []
         for c in coords:
@@ -148,27 +166,29 @@
                 scale_img,
                 (
                     offset - scale_img.get_rect().centerx,
                     offset - scale_img.get_rect().centery,
                 ),
             )
 
-        # drawing axle
         gfxdraw.aacircle(surf, offset, offset, int(0.05 * scale), (0, 0, 0))
         gfxdraw.filled_circle(surf, offset, offset, int(0.05 * scale), (0, 0, 0))
 
         surf = pygame.transform.flip(surf, False, True)
         screen.blit(surf, (0, 0))
 
         return (screen, clock, last_u), np.transpose(
             np.array(pygame.surfarray.pixels3d(screen)), axes=(1, 0, 2)
         )
 
     def render_init(
-        self, screen_width: int = 600, screen_height: int = 400
+        self,
+        screen_width: int = 600,
+        screen_height: int = 400,
+        params: PendulumParams = PendulumParams,
     ) -> RenderStateType:
         """Initialises the render state."""
         try:
             import pygame
         except ImportError as e:
             raise DependencyNotInstalled(
                 "pygame is not installed, run `pip install gymnasium[classic-control]`"
@@ -176,25 +196,33 @@
 
         pygame.init()
         screen = pygame.Surface((screen_width, screen_height))
         clock = pygame.time.Clock()
 
         return screen, clock, None
 
-    def render_close(self, render_state: RenderStateType):
+    def render_close(
+        self,
+        render_state: RenderStateType,
+        params: PendulumParams = PendulumParams,
+    ):
         """Closes the render state."""
         try:
             import pygame
         except ImportError as e:
             raise DependencyNotInstalled(
                 "pygame is not installed, run `pip install gymnasium[classic-control]`"
             ) from e
         pygame.display.quit()
         pygame.quit()
 
+    def get_default_params(self, **kwargs) -> PendulumParams:
+        """Returns the default parameters for the environment."""
+        return PendulumParams(**kwargs)
+
 
 class PendulumJaxEnv(FunctionalJaxEnv, EzPickle):
     """Jax-based pendulum environment using the functional version as base."""
 
     metadata = {"render_modes": ["rgb_array"], "render_fps": 30}
 
     def __init__(self, render_mode: str | None = None, **kwargs: Any):
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/registration.py` & `gymnasium-1.0.0a1/gymnasium/envs/registration.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import dataclasses
 import difflib
 import importlib
 import importlib.util
 import json
 import re
 import sys
-import traceback
 from collections import defaultdict
 from dataclasses import dataclass, field
+from enum import Enum
 from types import ModuleType
 from typing import Any, Callable, Iterable, Sequence
 
 import gymnasium as gym
 from gymnasium import Env, Wrapper, error, logger
 
 
@@ -34,14 +34,15 @@
 
 
 __all__ = [
     "registry",
     "current_namespace",
     "EnvSpec",
     "WrapperSpec",
+    "VectorizeMode",
     # Functions
     "register",
     "make",
     "make_vec",
     "spec",
     "pprint_registry",
     "register_envs",
@@ -54,15 +55,15 @@
     def __call__(self, **kwargs: Any) -> Env:
         ...
 
 
 class VectorEnvCreator(Protocol):
     """Function type expected for an environment."""
 
-    def __call__(self, **kwargs: Any) -> gym.experimental.vector.VectorEnv:
+    def __call__(self, **kwargs: Any) -> gym.vector.VectorEnv:
         ...
 
 
 @dataclass
 class WrapperSpec:
     """A specification for recording wrapper configs.
 
@@ -82,34 +83,34 @@
 
     * **id**: The string used to create the environment with :meth:`gymnasium.make`
     * **entry_point**: A string for the environment location, ``(import path):(environment name)`` or a function that creates the environment.
     * **reward_threshold**: The reward threshold for completing the environment.
     * **nondeterministic**: If the observation of an environment cannot be repeated with the same initial state, random number generator state and actions.
     * **max_episode_steps**: The max number of steps that the environment can take before truncation
     * **order_enforce**: If to enforce the order of :meth:`gymnasium.Env.reset` before :meth:`gymnasium.Env.step` and :meth:`gymnasium.Env.render` functions
-    * **autoreset**: If to automatically reset the environment on episode end
     * **disable_env_checker**: If to disable the environment checker wrapper in :meth:`gymnasium.make`, by default False (runs the environment checker)
     * **kwargs**: Additional keyword arguments passed to the environment during initialisation
     * **additional_wrappers**: A tuple of additional wrappers applied to the environment (WrapperSpec)
     * **vector_entry_point**: The location of the vectorized environment to create from
+
+    Changelogs:
+        v1.0.0 - Autoreset attribute removed
     """
 
     id: str
     entry_point: EnvCreator | str | None = field(default=None)
 
     # Environment attributes
     reward_threshold: float | None = field(default=None)
     nondeterministic: bool = field(default=False)
 
     # Wrappers
     max_episode_steps: int | None = field(default=None)
     order_enforce: bool = field(default=True)
-    autoreset: bool = field(default=False)
     disable_env_checker: bool = field(default=False)
-    apply_api_compatibility: bool = field(default=False)
 
     # Environment arguments
     kwargs: dict = field(default_factory=dict)
 
     # post-init attributes
     namespace: str | None = field(init=False)
     name: str = field(init=False)
@@ -220,20 +221,16 @@
         if print_all or self.nondeterministic is not False:
             output += f"\nnondeterministic={self.nondeterministic}"
 
         if print_all or self.max_episode_steps is not None:
             output += f"\nmax_episode_steps={self.max_episode_steps}"
         if print_all or self.order_enforce is not True:
             output += f"\norder_enforce={self.order_enforce}"
-        if print_all or self.autoreset is not False:
-            output += f"\nautoreset={self.autoreset}"
         if print_all or self.disable_env_checker is not False:
             output += f"\ndisable_env_checker={self.disable_env_checker}"
-        if print_all or self.apply_api_compatibility is not False:
-            output += f"\napplied_api_compatibility={self.apply_api_compatibility}"
 
         if print_all or self.additional_wrappers:
             wrapper_output: list[str] = []
             for wrapper_spec in self.additional_wrappers:
                 if include_entry_points:
                     wrapper_output.append(
                         f"\n\tname={wrapper_spec.name}, entry_point={wrapper_spec.entry_point}, kwargs={wrapper_spec.kwargs}"
@@ -250,14 +247,22 @@
 
         if disable_print:
             return output
         else:
             print(output)
 
 
+class VectorizeMode(Enum):
+    """All possible vectorization modes used in `make_vec`."""
+
+    ASYNC = "async"
+    SYNC = "sync"
+    VECTOR_ENTRY_POINT = "vector_entry_point"
+
+
 # Global registry of environments. Meant to be accessed through `register` and `make`
 registry: dict[str, EnvSpec] = {}
 current_namespace: str | None = None
 
 
 def parse_env_id(env_id: str) -> tuple[str | None, str, int | None]:
     """Parse environment ID string format - ``[namespace/](env-name)[-v(version)]`` where the namespace and version are optional.
@@ -543,63 +548,14 @@
     """
     mod_name, attr_name = name.split(":")
     mod = importlib.import_module(mod_name)
     fn = getattr(mod, attr_name)
     return fn
 
 
-def load_plugin_envs(entry_point: str = "gymnasium.envs"):
-    """Load modules (plugins) using the gymnasium entry points in order to register external module's environments on ``import gymnasium``.
-
-    Args:
-        entry_point: The string for the entry point.
-    """
-    # Load third-party environments
-    for plugin in metadata.entry_points(group=entry_point):
-        # Python 3.8 doesn't support plugin.module, plugin.attr
-        # So we'll have to try and parse this ourselves
-        module, attr = None, None
-        try:
-            module, attr = plugin.module, plugin.attr  # type: ignore  ## error: Cannot access member "attr" for type "EntryPoint"
-        except AttributeError:
-            if ":" in plugin.value:
-                module, attr = plugin.value.split(":", maxsplit=1)
-            else:
-                module, attr = plugin.value, None
-        except Exception as e:
-            logger.warn(
-                f"While trying to load plugin `{plugin}` from {entry_point}, an exception occurred: {e}"
-            )
-            module, attr = None, None
-        finally:
-            if attr is None:
-                raise error.Error(
-                    f"Gymnasium environment plugin `{module}` must specify a function to execute, not a root module"
-                )
-
-        context = namespace(plugin.name)
-        if plugin.name.startswith("__") and plugin.name.endswith("__"):
-            # `__internal__` is an artifact of the plugin system when the root namespace had an allow-list.
-            # The allow-list is now removed and plugins can register environments in the root namespace with the `__root__` magic key.
-            if plugin.name == "__root__" or plugin.name == "__internal__":
-                context = contextlib.nullcontext()
-            else:
-                logger.warn(
-                    f"The environment namespace magic key `{plugin.name}` is unsupported. "
-                    "To register an environment at the root namespace you should specify the `__root__` namespace."
-                )
-
-        with context:
-            fn = plugin.load()
-            try:
-                fn()
-            except Exception:
-                logger.warn(f"plugin: {plugin.value} raised {traceback.format_exc()}")
-
-
 def register_envs(env_module: ModuleType):
     """A No-op function such that it can appear to IDEs that a module is used."""
     pass
 
 
 @contextlib.contextmanager
 def namespace(ns: str):
@@ -614,20 +570,18 @@
 def register(
     id: str,
     entry_point: EnvCreator | str | None = None,
     reward_threshold: float | None = None,
     nondeterministic: bool = False,
     max_episode_steps: int | None = None,
     order_enforce: bool = True,
-    autoreset: bool = False,
     disable_env_checker: bool = False,
-    apply_api_compatibility: bool = False,
     additional_wrappers: tuple[WrapperSpec, ...] = (),
     vector_entry_point: VectorEnvCreator | str | None = None,
-    **kwargs: Any,
+    kwargs: dict | None = None,
 ):
     """Registers an environment in gymnasium with an ``id`` to use with :meth:`gymnasium.make` with the ``entry_point`` being a string or callable for creating the environment.
 
     The ``id`` parameter corresponds to the name of the environment, with the syntax as follows:
     ``[namespace/](env_name)[-v(version)]`` where ``namespace`` and ``-v(version)`` is optional.
 
     It takes arbitrary keyword arguments, which are passed to the :class:`EnvSpec` ``kwargs`` parameter.
@@ -636,28 +590,30 @@
         id: The environment id
         entry_point: The entry point for creating the environment
         reward_threshold: The reward threshold considered for an agent to have learnt the environment
         nondeterministic: If the environment is nondeterministic (even with knowledge of the initial seed and all actions, the same state cannot be reached)
         max_episode_steps: The maximum number of episodes steps before truncation. Used by the :class:`gymnasium.wrappers.TimeLimit` wrapper if not ``None``.
         order_enforce: If to enable the order enforcer wrapper to ensure users run functions in the correct order.
             If ``True``, then the :class:`gymnasium.wrappers.OrderEnforcing` is applied to the environment.
-        autoreset: If to add the :class:`gymnasium.wrappers.AutoResetWrapper` such that on ``(terminated or truncated) is True``, :meth:`gymnasium.Env.reset` is called.
         disable_env_checker: If to disable the :class:`gymnasium.wrappers.PassiveEnvChecker` to the environment.
-        apply_api_compatibility: If to apply the :class:`gymnasium.wrappers.StepAPICompatibility` wrapper to the environment.
-            Use if the environment is implemented in the gym v0.21 environment API.
         additional_wrappers: Additional wrappers to apply the environment.
         vector_entry_point: The entry point for creating the vector environment
-        **kwargs: arbitrary keyword arguments which are passed to the environment constructor on initialisation.
+        kwargs: arbitrary keyword arguments which are passed to the environment constructor on initialisation.
+
+    Changelogs:
+        v1.0.0 - `autoreset` and `apply_api_compatibility` parameter was removed
     """
     assert (
         entry_point is not None or vector_entry_point is not None
     ), "Either `entry_point` or `vector_entry_point` (or both) must be provided"
     global registry, current_namespace
     ns, name, version = parse_env_id(id)
 
+    if kwargs is None:
+        kwargs = dict()
     if current_namespace is not None:
         if (
             kwargs.get("namespace") is not None
             and kwargs.get("namespace") != current_namespace
         ):
             logger.warn(
                 f"Custom namespace `{kwargs.get('namespace')}` is being overridden by namespace `{current_namespace}`. "
@@ -665,70 +621,61 @@
                 "The namespace is specified through the entry point package metadata."
             )
         ns_id = current_namespace
     else:
         ns_id = ns
     full_env_id = get_env_id(ns_id, name, version)
 
-    if autoreset is True:
-        logger.warn(
-            "`gymnasium.register(..., autoreset=True)` is deprecated and will be removed in v1.0. If users wish to use it then add the auto reset wrapper in the `addition_wrappers` argument."
-        )
-
     new_spec = EnvSpec(
         id=full_env_id,
         entry_point=entry_point,
         reward_threshold=reward_threshold,
         nondeterministic=nondeterministic,
         max_episode_steps=max_episode_steps,
         order_enforce=order_enforce,
-        autoreset=autoreset,
         disable_env_checker=disable_env_checker,
-        apply_api_compatibility=apply_api_compatibility,
-        **kwargs,
+        kwargs=kwargs,
         additional_wrappers=additional_wrappers,
         vector_entry_point=vector_entry_point,
     )
     _check_spec_register(new_spec)
 
     if new_spec.id in registry:
         logger.warn(f"Overriding environment {new_spec.id} already in registry.")
     registry[new_spec.id] = new_spec
 
 
 def make(
     id: str | EnvSpec,
     max_episode_steps: int | None = None,
-    autoreset: bool | None = None,
-    apply_api_compatibility: bool | None = None,
     disable_env_checker: bool | None = None,
     **kwargs: Any,
 ) -> Env:
     """Creates an environment previously registered with :meth:`gymnasium.register` or a :class:`EnvSpec`.
 
     To find all available environments use ``gymnasium.envs.registry.keys()`` for all valid ids.
 
     Args:
         id: A string for the environment id or a :class:`EnvSpec`. Optionally if using a string, a module to import can be included, e.g. ``'module:Env-v0'``.
             This is equivalent to importing the module first to register the environment followed by making the environment.
-        max_episode_steps: Maximum length of an episode, can override the registered :class:`EnvSpec` ``max_episode_steps``.
-            The value is used by :class:`gymnasium.wrappers.TimeLimit`.
-        autoreset: Whether to automatically reset the environment after each episode (:class:`gymnasium.wrappers.AutoResetWrapper`).
-        apply_api_compatibility: Whether to wrap the environment with the :class:`gymnasium.wrappers.StepAPICompatibility` wrapper that
-            converts the environment step from a done bool to return termination and truncation bools.
-            By default, the argument is None in which the :class:`EnvSpec` ``apply_api_compatibility`` is used, otherwise this variable is used in favor.
+        max_episode_steps: Maximum length of an episode, can override the registered :class:`EnvSpec` ``max_episode_steps``
+            with the value being passed to :class:`gymnasium.wrappers.TimeLimit`.
+            Using ``max_episode_steps=-1`` will not apply the wrapper to the environment.
         disable_env_checker: If to add :class:`gymnasium.wrappers.PassiveEnvChecker`, ``None`` will default to the
             :class:`EnvSpec` ``disable_env_checker`` value otherwise use this value will be used.
         kwargs: Additional arguments to pass to the environment constructor.
 
     Returns:
         An instance of the environment with wrappers applied.
 
     Raises:
         Error: If the ``id`` doesn't exist in the :attr:`registry`
+
+    Changelogs:
+        v1.0.0 - `autoreset` and `apply_api_compatibility` was removed
     """
     if isinstance(id, EnvSpec):
         env_spec = id
         if not hasattr(env_spec, "additional_wrappers"):
             logger.warn(
                 f"The env spec passed to `make` does not have a `additional_wrappers`, set it to an empty tuple. Env_spec={env_spec}"
             )
@@ -786,22 +733,14 @@
             apply_render_collection = True
         else:
             logger.warn(
                 f"The environment is being initialised with render_mode={render_mode!r} "
                 f"that is not in the possible render_modes ({render_modes})."
             )
 
-    if apply_api_compatibility or (
-        apply_api_compatibility is None and env_spec.apply_api_compatibility
-    ):
-        # If we use the compatibility layer, we treat the render mode explicitly and don't pass it to the env creator
-        render_mode = env_spec_kwargs.pop("render_mode", None)
-    else:
-        render_mode = None
-
     try:
         env = env_creator(**env_spec_kwargs)
     except TypeError as e:
         if (
             str(e).find("got an unexpected keyword argument 'render_mode'") >= 0
             and apply_human_rendering
         ):
@@ -819,17 +758,15 @@
     env.unwrapped.spec = EnvSpec(
         id=env_spec.id,
         entry_point=env_spec.entry_point,
         reward_threshold=env_spec.reward_threshold,
         nondeterministic=env_spec.nondeterministic,
         max_episode_steps=None,
         order_enforce=False,
-        autoreset=False,
         disable_env_checker=True,
-        apply_api_compatibility=False,
         kwargs=env_spec_kwargs,
         additional_wrappers=(),
         vector_entry_point=env_spec.vector_entry_point,
     )
 
     # Check if pre-wrapped wrappers
     assert env.spec is not None
@@ -841,46 +778,30 @@
         for env_spec_wrapper_spec, recreated_wrapper_spec in zip(
             env_spec.additional_wrappers, env.spec.additional_wrappers
         ):
             raise ValueError(
                 f"The environment's wrapper spec {recreated_wrapper_spec} is different from the saved `EnvSpec` additional wrapper {env_spec_wrapper_spec}"
             )
 
-    # Add step API wrapper
-    if apply_api_compatibility is True or (
-        apply_api_compatibility is None and env_spec.apply_api_compatibility is True
-    ):
-        logger.warn(
-            "`gymnasium.make(..., apply_api_compatibility=True)` and `env_spec.apply_api_compatibility` is deprecated and will be removed in v1.0"
-        )
-        env = gym.wrappers.EnvCompatibility(env, render_mode)
-
     # Run the environment checker as the lowest level wrapper
     if disable_env_checker is False or (
         disable_env_checker is None and env_spec.disable_env_checker is False
     ):
         env = gym.wrappers.PassiveEnvChecker(env)
 
     # Add the order enforcing wrapper
     if env_spec.order_enforce:
         env = gym.wrappers.OrderEnforcing(env)
 
     # Add the time limit wrapper
-    if max_episode_steps is not None:
-        env = gym.wrappers.TimeLimit(env, max_episode_steps)
-    elif env_spec.max_episode_steps is not None:
-        env = gym.wrappers.TimeLimit(env, env_spec.max_episode_steps)
-
-    # Add the auto-reset wrapper
-    if autoreset is True or (autoreset is None and env_spec.autoreset is True):
-        env = gym.wrappers.AutoResetWrapper(env)
-
-        logger.warn(
-            "`gymnasium.make(..., autoreset=True)` is deprecated and will be removed in v1.0"
-        )
+    if max_episode_steps != -1:
+        if max_episode_steps is not None:
+            env = gym.wrappers.TimeLimit(env, max_episode_steps)
+        elif env_spec.max_episode_steps is not None:
+            env = gym.wrappers.TimeLimit(env, env_spec.max_episode_steps)
 
     for wrapper_spec in env_spec.additional_wrappers[num_prior_wrappers:]:
         if wrapper_spec.kwargs is None:
             raise ValueError(
                 f"{wrapper_spec.name} wrapper does not inherit from `gymnasium.utils.RecordConstructorArgs`, therefore, the wrapper cannot be recreated."
             )
 
@@ -894,123 +815,143 @@
 
     return env
 
 
 def make_vec(
     id: str | EnvSpec,
     num_envs: int = 1,
-    vectorization_mode: str = "async",
+    vectorization_mode: VectorizeMode | str | None = None,
     vector_kwargs: dict[str, Any] | None = None,
     wrappers: Sequence[Callable[[Env], Wrapper]] | None = None,
     **kwargs,
-) -> gym.experimental.vector.VectorEnv:
+) -> gym.vector.VectorEnv:
     """Create a vector environment according to the given ID.
 
-    Note:
-        This feature is experimental, and is likely to change in future releases.
-
-    To find all available environments use `gymnasium.envs.registry.keys()` for all valid ids.
+    To find all available environments use :func:`gymnasium.pprint_registry` or ``gymnasium.registry.keys()`` for all valid ids.
+    We refer to the Vector environment as the vectorizor while the environment being vectorized is the base or vectorized environment (``vectorizor(vectorized env)``).
 
     Args:
         id: Name of the environment. Optionally, a module to import can be included, eg. 'module:Env-v0'
         num_envs: Number of environments to create
-        vectorization_mode: How to vectorize the environment. Can be either "async", "sync" or "custom"
-        vector_kwargs: Additional arguments to pass to the vectorized environment constructor.
-        wrappers: A sequence of wrapper functions to apply to the environment. Can only be used in "sync" or "async" mode.
-        **kwargs: Additional arguments to pass to the environment constructor.
+        vectorization_mode: The vectorization method used, defaults to ``None`` such that if env id' spec has a ``vector_entry_point`` (not ``None``),
+            this is first used otherwise defaults to ``sync`` to use the :class:`gymnasium.vector.SyncVectorEnv`.
+            Valid modes are ``"async"``, ``"sync"`` or ``"vector_entry_point"``. Recommended to use the :class:`VectorizeMode` enum rather than strings.
+        vector_kwargs: Additional arguments to pass to the vectorizor environment constructor, i.e., ``SyncVectorEnv(..., **vector_kwargs)``.
+        wrappers: A sequence of wrapper functions to apply to the base environment. Can only be used in ``"sync"`` or ``"async"`` mode.
+        **kwargs: Additional arguments passed to the base environment constructor.
 
     Returns:
         An instance of the environment.
 
     Raises:
         Error: If the ``id`` doesn't exist then an error is raised
     """
     if vector_kwargs is None:
         vector_kwargs = {}
-
     if wrappers is None:
         wrappers = []
 
     if isinstance(id, EnvSpec):
-        spec_ = id
+        env_spec = id
+    elif isinstance(id, str):
+        env_spec = _find_spec(id)
     else:
-        spec_ = _find_spec(id)
+        raise error.Error(f"Invalid id type: {type(id)}. Expected `str` or `EnvSpec`")
 
-    _kwargs = spec_.kwargs.copy()
-    _kwargs.update(kwargs)
+    env_spec = copy.deepcopy(env_spec)
+    env_spec_kwargs = env_spec.kwargs
 
-    # Check if we have the necessary entry point
-    if vectorization_mode in ("sync", "async"):
-        if spec_.entry_point is None:
-            raise error.Error(
-                f"Cannot create vectorized environment for {id} because it doesn't have an entry point defined."
-            )
-        entry_point = spec_.entry_point
-    elif vectorization_mode in ("custom",):
-        if spec_.vector_entry_point is None:
-            raise error.Error(
-                f"Cannot create vectorized environment for {id} because it doesn't have a vector entry point defined."
-            )
-        entry_point = spec_.vector_entry_point
-    else:
-        raise error.Error(f"Invalid vectorization mode: {vectorization_mode}")
+    num_envs = env_spec_kwargs.pop("num_envs", num_envs)
+    vectorization_mode = env_spec_kwargs.pop("vectorization_mode", vectorization_mode)
+    vector_kwargs = env_spec_kwargs.pop("vector_kwargs", vector_kwargs)
+    wrappers = env_spec_kwargs.pop("wrappers", wrappers)
 
-    if callable(entry_point):
-        env_creator = entry_point
-    else:
-        # Assume it's a string
-        env_creator = load_env_creator(entry_point)
+    env_spec_kwargs.update(kwargs)
 
-    def _create_env():
-        # Env creator for use with sync and async modes
-        _kwargs_copy = _kwargs.copy()
-
-        render_mode = _kwargs.get("render_mode", None)
-        if render_mode is not None:
-            inner_render_mode = (
-                render_mode[: -len("_list")]
-                if render_mode.endswith("_list")
-                else render_mode
+    # Specify the vectorization mode if None or update to a `VectorizeMode`
+    if vectorization_mode is None:
+        if env_spec.vector_entry_point is not None:
+            vectorization_mode = VectorizeMode.VECTOR_ENTRY_POINT
+        else:
+            vectorization_mode = VectorizeMode.SYNC
+    else:
+        try:
+            vectorization_mode = VectorizeMode(vectorization_mode)
+        except ValueError:
+            raise ValueError(
+                f"Invalid vectorization mode: {vectorization_mode!r}, "
+                f"valid modes: {[mode.value for mode in VectorizeMode]}"
             )
-            _kwargs_copy["render_mode"] = inner_render_mode
+    assert isinstance(vectorization_mode, VectorizeMode)
 
-        _env = env_creator(**_kwargs_copy)
-        _env.spec = spec_
-        if spec_.max_episode_steps is not None:
-            _env = gym.wrappers.TimeLimit(_env, spec_.max_episode_steps)
+    def create_single_env() -> Env:
+        single_env = make(env_spec, **env_spec_kwargs.copy())
 
-        if render_mode is not None and render_mode.endswith("_list"):
-            _env = gym.wrappers.RenderCollection(_env)
+        if wrappers is None:
+            return single_env
 
         for wrapper in wrappers:
-            _env = wrapper(_env)
-        return _env
+            single_env = wrapper(single_env)
+        return single_env
 
-    if vectorization_mode == "sync":
-        env = gym.experimental.vector.SyncVectorEnv(
-            env_fns=[_create_env for _ in range(num_envs)],
+    if vectorization_mode == VectorizeMode.SYNC:
+        if env_spec.entry_point is None:
+            raise error.Error(
+                f"Cannot create vectorized environment for {env_spec.id} because it doesn't have an entry point defined."
+            )
+
+        env = gym.vector.SyncVectorEnv(
+            env_fns=(create_single_env for _ in range(num_envs)),
             **vector_kwargs,
         )
-    elif vectorization_mode == "async":
-        env = gym.experimental.vector.AsyncVectorEnv(
-            env_fns=[_create_env for _ in range(num_envs)],
+    elif vectorization_mode == VectorizeMode.ASYNC:
+        if env_spec.entry_point is None:
+            raise error.Error(
+                f"Cannot create vectorized environment for {env_spec.id} because it doesn't have an entry point defined."
+            )
+
+        env = gym.vector.AsyncVectorEnv(
+            env_fns=[create_single_env for _ in range(num_envs)],
             **vector_kwargs,
         )
-    elif vectorization_mode == "custom":
+
+    elif vectorization_mode == VectorizeMode.VECTOR_ENTRY_POINT:
+        entry_point = env_spec.vector_entry_point
+        if entry_point is None:
+            raise error.Error(
+                f"Cannot create vectorized environment for {id} because it doesn't have a vector entry point defined."
+            )
+        elif callable(entry_point):
+            env_creator = entry_point
+        else:  # Assume it's a string
+            env_creator = load_env_creator(entry_point)
+
         if len(wrappers) > 0:
-            raise error.Error("Cannot use custom vectorization mode with wrappers.")
-        vector_kwargs["max_episode_steps"] = spec_.max_episode_steps
+            raise error.Error(
+                "Cannot use `vector_entry_point` vectorization mode with the wrappers argument."
+            )
+        if "max_episode_steps" not in vector_kwargs:
+            assert vector_kwargs is not None
+            vector_kwargs["max_episode_steps"] = env_spec.max_episode_steps
+
         env = env_creator(num_envs=num_envs, **vector_kwargs)
     else:
-        raise error.Error(f"Invalid vectorization mode: {vectorization_mode}")
+        raise error.Error(f"Unknown vectorization mode: {vectorization_mode}")
 
     # Copies the environment creation specification and kwargs to add to the environment specification details
-    spec_ = copy.deepcopy(spec_)
-    spec_.kwargs = _kwargs
-    env.unwrapped.spec = spec_
+    copied_id_spec = copy.deepcopy(env_spec)
+    copied_id_spec.kwargs = env_spec_kwargs
+    if num_envs != 1:
+        copied_id_spec.kwargs["num_envs"] = num_envs
+    copied_id_spec.kwargs["vectorization_mode"] = vectorization_mode.value
+    if len(vector_kwargs) > 0:
+        copied_id_spec.kwargs["vector_kwargs"] = vector_kwargs
+    if len(wrappers) > 0:
+        copied_id_spec.kwargs["wrappers"] = wrappers
+    env.unwrapped.spec = copied_id_spec
 
     return env
 
 
 def spec(env_id: str) -> EnvSpec:
     """Retrieve the :class:`EnvSpec` for the environment id from the :attr:`registry`.
 
@@ -1051,15 +992,15 @@
         print_registry: Environment registry to be printed. By default, :attr:`registry`
         num_cols: Number of columns to arrange environments in, for display.
         exclude_namespaces: A list of namespaces to be excluded from printing. Helpful if only ALE environments are wanted.
         disable_print: Whether to return a string of all the namespaces and environment IDs
             or to print the string to console.
     """
     # Defaultdict to store environment ids according to namespace.
-    namespace_envs: dict[str, list[str]] = defaultdict(lambda: [])
+    namespace_envs: dict[str, list[str]] = defaultdict(list)
     max_justify = float("-inf")
 
     # Find the namespace associated with each environment spec
     for env_spec in print_registry.values():
         ns = env_spec.namespace
 
         if ns is None and isinstance(env_spec.entry_point, str):
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/tabular/blackjack.py` & `gymnasium-1.0.0a1/gymnasium/envs/tabular/blackjack.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 import math
 import os
 from typing import NamedTuple, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 import numpy as np
+from flax import struct
 from jax import random
 from jax.random import PRNGKey
 
 from gymnasium import spaces
+from gymnasium.envs.functional_jax_env import FunctionalJaxEnv
 from gymnasium.error import DependencyNotInstalled
-from gymnasium.experimental.functional import ActType, FuncEnv, StateType
-from gymnasium.experimental.functional_jax_env import FunctionalJaxEnv
+from gymnasium.functional import ActType, FuncEnv, StateType
 from gymnasium.utils import EzPickle, seeding
 from gymnasium.wrappers import HumanRendering
 
 
 RenderStateType = Tuple["pygame.Surface", str, int]  # type: ignore  # noqa: F821
 
 
@@ -154,16 +155,24 @@
         jnp.logical_and(
             jnp.count_nonzero(hand) == 2, (jnp.count_nonzero(hand == 1) > 0)
         ),
         (jnp.count_nonzero(hand == 10) > 0),
     )
 
 
+@struct.dataclass
+class BlackJackParams:
+    """Parameters for the jax Blackjack environment."""
+
+    natural: bool = False
+    sutton_and_barto: bool = True
+
+
 class BlackjackFunctional(
-    FuncEnv[jax.Array, jax.Array, int, float, bool, RenderStateType]
+    FuncEnv[jax.Array, jax.Array, int, float, bool, RenderStateType, BlackJackParams]
 ):
     """Blackjack is a card game where the goal is to beat the dealer by obtaining cards that sum to closer to 21 (without going over 21) than the dealers cards.
 
     ### Description
     Card Values:
 
     - Face cards (Jack, Queen, King) have a point value of 10.
@@ -229,23 +238,21 @@
     )
 
     metadata = {
         "render_modes": ["rgb_array"],
         "render_fps": 4,
     }
 
-    def __init__(self, natural: bool = False, sutton_and_barto: bool = True):
-        """Initializes Blackjack functional env."""
-        # Flag to payout 1.5 on a "natural" blackjack win, like casino rules
-        # Ref: http://www.bicyclecards.com/how-to-play/blackjack/
-        self.natural = natural
-        # Flag for full agreement with the (Sutton and Barto, 2018) definition. Overrides self.natural
-        self.sutton_and_barto = sutton_and_barto
-
-    def transition(self, state: EnvState, action: Union[int, jax.Array], key: PRNGKey):
+    def transition(
+        self,
+        state: EnvState,
+        action: Union[int, jax.Array],
+        key: PRNGKey,
+        params: BlackJackParams = BlackJackParams,
+    ):
         """The blackjack environment's state transition function."""
         env_state = jax.lax.cond(action, take, notake, (state, key))
 
         hand_state, key = env_state
         dealer_hand = hand_state.dealer_hand
         player_hand = hand_state.player_hand
         dealer_cards = hand_state.dealer_cards
@@ -261,15 +268,15 @@
             dealer_cards=dealer_cards,
             player_cards=player_cards,
             done=done,
         )
 
         return new_state
 
-    def initial(self, rng: PRNGKey):
+    def initial(self, rng: PRNGKey, params: BlackJackParams = BlackJackParams):
         """Blackjack initial observataion function."""
         player_hand = jnp.zeros(21)
         dealer_hand = jnp.zeros(21)
         player_hand, rng = draw_hand(rng, player_hand)
         dealer_hand, rng = draw_hand(rng, dealer_hand)
         dealer_cards = 2
         player_cards = 2
@@ -280,31 +287,39 @@
             dealer_cards=dealer_cards,
             player_cards=player_cards,
             done=0,
         )
 
         return state
 
-    def observation(self, state: EnvState) -> jax.Array:
+    def observation(
+        self, state: EnvState, params: BlackJackParams = BlackJackParams
+    ) -> jax.Array:
         """Blackjack observation."""
         return jnp.array(
             [
                 sum_hand(state.player_hand),
                 state.dealer_hand[0],
                 usable_ace(state.player_hand) * 1.0,
             ],
             dtype=np.int32,
         )
 
-    def terminal(self, state: EnvState) -> jax.Array:
+    def terminal(
+        self, state: EnvState, params: BlackJackParams = BlackJackParams
+    ) -> jax.Array:
         """Determines if a particular Blackjack observation is terminal."""
         return (state.done) > 0
 
     def reward(
-        self, state: EnvState, action: ActType, next_state: StateType
+        self,
+        state: EnvState,
+        action: ActType,
+        next_state: StateType,
+        params: BlackJackParams = BlackJackParams,
     ) -> jax.Array:
         """Calculates reward from a state."""
         state = next_state
 
         dealer_hand = state.dealer_hand
         player_hand = state.player_hand
 
@@ -312,22 +327,22 @@
         reward = (
             0.0
             + (is_bust(player_hand) * -1 * action)
             + ((jnp.logical_not(action)) * cmp(score(player_hand), score(dealer_hand)))
         )
 
         # in the natural setting, if the player wins with a natural blackjack, then reward is 1.5
-        if self.natural and not self.sutton_and_barto:
+        if params.natural and not params.sutton_and_barto:
             condition = jnp.logical_and(is_natural(player_hand), (reward == 1))
             reward = reward * jnp.logical_not(condition) + 1.5 * condition
 
         # in the sutton and barto setting, if the player gets a natural blackjack and the dealer gets
         # a non-natural blackjack, the player wins. A dealer natural blackjack and a player
         # non-natural blackjack should result in a tie.
-        if self.sutton_and_barto:
+        if params.sutton_and_barto:
             condition = jnp.logical_and(
                 is_natural(player_hand), jnp.logical_not(is_natural(dealer_hand))
             )
             reward = reward * jnp.logical_not(condition) + 1 * condition
         return reward
 
     def render_init(
@@ -351,14 +366,15 @@
 
         return screen, dealer_top_card_value_str, dealer_top_card_suit
 
     def render_image(
         self,
         state: StateType,
         render_state: RenderStateType,
+        params: BlackJackParams = BlackJackParams,
     ) -> Tuple[RenderStateType, np.ndarray]:
         """Renders an image from a state."""
         try:
             import pygame
         except ImportError:
             raise DependencyNotInstalled(
                 "pygame is not installed, run `pip install gymnasium[toy_text]`"
@@ -468,14 +484,18 @@
         except ImportError as e:
             raise DependencyNotInstalled(
                 "pygame is not installed, run `pip install gymnasium[classic_control]`"
             ) from e
         pygame.display.quit()
         pygame.quit()
 
+    def get_default_params(self, **kwargs) -> BlackJackParams:
+        """Get the default params."""
+        return BlackJackParams(**kwargs)
+
 
 class BlackJackJaxEnv(FunctionalJaxEnv, EzPickle):
     """A Gymnasium Env wrapper for the functional blackjack env."""
 
     metadata = {"render_modes": ["rgb_array"], "render_fps": 50}
 
     def __init__(self, render_mode: Optional[str] = None, **kwargs):
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/tabular/cliffwalking.py` & `gymnasium-1.0.0a1/gymnasium/envs/tabular/cliffwalking.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 from jax.random import PRNGKey
 
 from gymnasium import spaces
+from gymnasium.envs.functional_jax_env import FunctionalJaxEnv
 from gymnasium.error import DependencyNotInstalled
-from gymnasium.experimental.functional import ActType, FuncEnv, StateType
-from gymnasium.experimental.functional_jax_env import FunctionalJaxEnv
+from gymnasium.functional import ActType, FuncEnv, StateType
 from gymnasium.utils import EzPickle
 from gymnasium.wrappers import HumanRendering
 
 
 if TYPE_CHECKING:
     import pygame
 
@@ -58,15 +58,15 @@
         (player_position[0] == 3)
         * (player_position[1] >= 1)
         * (player_position[1] <= 10)
     )
 
 
 class CliffWalkingFunctional(
-    FuncEnv[jax.Array, jax.Array, int, float, bool, RenderStateType]
+    FuncEnv[jax.Array, jax.Array, int, float, bool, RenderStateType, None]
 ):
     """Cliff walking involves crossing a gridworld from start to goal while avoiding falling off a cliff.
 
     ## Description
     The game starts with the player at location [3, 0] of the 4x12 grid world with the
     goal located at [3, 11]. If the player reaches the goal the episode ends.
 
@@ -92,17 +92,17 @@
 
     ## Observation Space
     There are 3 x 12 + 1 possible states. The player cannot be at the cliff, nor at
     the goal as the latter results in the end of the episode. What remains are all
     the positions of the first 3 rows plus the bottom-left cell.
 
     The observation is a value representing the player's current position as
-    current_row * nrows + current_col (where both the row and col start at 0).
+    current_row * ncols + current_col (where both the row and col start at 0).
 
-    For example, the stating position can be calculated as follows: 3 * 12 + 0 = 36.
+    For example, the starting position can be calculated as follows: 3 * 12 + 0 = 36.
 
     The observation is returned as an `numpy.ndarray` with shape `(1,)` and dtype `numpy.int32` .
 
     ## Starting State
     The episode starts with the player in state `[36]` (location [3, 0]).
 
     ## Reward
@@ -135,15 +135,21 @@
     )  # A discrete state corresponds to each possible location
 
     metadata = {
         "render_modes": ["rgb_array"],
         "render_fps": 4,
     }
 
-    def transition(self, state: EnvState, action: int | jax.Array, key: PRNGKey):
+    def transition(
+        self,
+        state: EnvState,
+        action: int | jax.Array,
+        key: PRNGKey,
+        params: None = None,
+    ):
         """The Cliffwalking environment's state transition function."""
         new_position = state.player_position
 
         # where is the agent trying to go?
         new_position = jnp.array(
             [
                 new_position[0] + (1 * (action == 2)) + (-1 * (action == 0)),
@@ -171,33 +177,37 @@
             player_position=new_position.reshape((2,)),
             last_action=action[0],
             fallen=fallen,
         )
 
         return new_state
 
-    def initial(self, rng: PRNGKey) -> EnvState:
+    def initial(self, rng: PRNGKey, params: None = None) -> EnvState:
         """Cliffwalking initial observation function."""
         player_position = jnp.array([3, 0])
 
         state = EnvState(player_position=player_position, last_action=-1, fallen=False)
         return state
 
-    def observation(self, state: EnvState) -> int:
+    def observation(self, state: EnvState, params: None = None) -> int:
         """Cliffwalking observation."""
         return jnp.array(
             state.player_position[0] * 12 + state.player_position[1]
         ).reshape((1,))
 
-    def terminal(self, state: EnvState) -> jax.Array:
+    def terminal(self, state: EnvState, params: None = None) -> jax.Array:
         """Determines if a particular Cliffwalking observation is terminal."""
         return jnp.array_equal(state.player_position, jnp.array([3, 11]))
 
     def reward(
-        self, state: EnvState, action: ActType, next_state: StateType
+        self,
+        state: EnvState,
+        action: ActType,
+        next_state: StateType,
+        params: None = None,
     ) -> jax.Array:
         """Calculates reward from a state."""
         state = next_state
         reward = -1 + (-99 * state.fallen[0])
         return jax.lax.convert_element_type(reward, jnp.float32)
 
     def render_init(
@@ -281,17 +291,15 @@
             mountain_bg_img=tuple(mountain_bg_img),
             near_cliff_imgs=tuple(near_cliff_imgs),
             near_cliff_img=tuple(near_cliff_img),
             cliff_img=cliff_img,
         )
 
     def render_image(
-        self,
-        state: StateType,
-        render_state: RenderStateType,
+        self, state: StateType, render_state: RenderStateType, params: None = None
     ) -> tuple[RenderStateType, np.ndarray]:
         """Renders an image from a state."""
         try:
             import pygame
         except ImportError:
             raise DependencyNotInstalled(
                 "pygame is not installed, run `pip install gymnasium[toy_text]`"
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/blackjack.py` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/blackjack.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,21 +86,21 @@
     The observation consists of a 3-tuple containing: the player's current sum,
     the value of the dealer's one showing card (1-10 where 1 is ace),
     and whether the player holds a usable ace (0 or 1).
 
     The observation is returned as `(int(), int(), int())`.
 
     ## Starting State
-    The starting state is initialised in the following range.
+    The starting state is initialised with the following values.
 
-    | Observation               | Min  | Max  |
-    |---------------------------|------|------|
-    | Player current sum        |  4   |  12  |
-    | Dealer showing card value |  2   |  11  |
-    | Usable Ace                |  0   |  1   |
+    | Observation               | Values         |
+    |---------------------------|----------------|
+    | Player current sum        |  4, 5, ..., 21 |
+    | Dealer showing card value |  1, 2, ..., 10 |
+    | Usable Ace                |  0, 1          |
 
     ## Rewards
     - win game: +1
     - lose game: -1
     - draw game: 0
     - win game with natural blackjack:
     +1.5 (if <a href="#nat">natural</a> is True)
@@ -189,14 +189,15 @@
                 and reward == 1.0
             ):
                 # Natural gives extra points, but doesn't autowin. Legacy implementation
                 reward = 1.5
 
         if self.render_mode == "human":
             self.render()
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
         return self._get_obs(), reward, terminated, False, {}
 
     def _get_obs(self):
         return (sum_hand(self.player), self.dealer[0], usable_ace(self.player))
 
     def reset(
         self,
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/cliffwalking.py` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/cliffwalking.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,17 +47,17 @@
 
     ## Observation Space
     There are 3 x 12 + 1 possible states. The player cannot be at the cliff, nor at
     the goal as the latter results in the end of the episode. What remains are all
     the positions of the first 3 rows plus the bottom-left cell.
 
     The observation is a value representing the player's current position as
-    current_row * nrows + current_col (where both the row and col start at 0).
+    current_row * ncols + current_col (where both the row and col start at 0).
 
-    For example, the stating position can be calculated as follows: 3 * 12 + 0 = 36.
+    For example, the starting position can be calculated as follows: 3 * 12 + 0 = 36.
 
     The observation is returned as an `int()`.
 
     ## Starting State
     The episode starts with the player in state `[36]` (location [3, 0]).
 
     ## Reward
@@ -175,15 +175,16 @@
         i = categorical_sample([t[0] for t in transitions], self.np_random)
         p, s, r, t = transitions[i]
         self.s = s
         self.lastaction = a
 
         if self.render_mode == "human":
             self.render()
-        return (int(s), r, t, False, {"prob": p})
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
+        return int(s), r, t, False, {"prob": p}
 
     def reset(self, *, seed: Optional[int] = None, options: Optional[dict] = None):
         super().reset(seed=seed)
         self.s = categorical_sample(self.initial_state_distrib, self.np_random)
         self.lastaction = None
 
         if self.render_mode == "human":
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/font/Minecraft.ttf` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/font/Minecraft.ttf`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/frozen_lake.py` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/frozen_lake.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     - 0: Move left
     - 1: Move down
     - 2: Move right
     - 3: Move up
 
     ## Observation Space
     The observation is a value representing the player's current position as
-    current_row * nrows + current_col (where both the row and col start at 0).
+    current_row * ncols + current_col (where both the row and col start at 0).
 
     For example, the goal position in the 4x4 map can be calculated as follows: 3 * 4 + 3 = 15.
     The number of possible observations is dependent on the size of the map.
 
     The observation is returned as an `int()`.
 
     ## Starting State
@@ -302,15 +302,16 @@
         i = categorical_sample([t[0] for t in transitions], self.np_random)
         p, s, r, t = transitions[i]
         self.s = s
         self.lastaction = a
 
         if self.render_mode == "human":
             self.render()
-        return (int(s), r, t, False, {"prob": p})
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
+        return int(s), r, t, False, {"prob": p}
 
     def reset(
         self,
         *,
         seed: Optional[int] = None,
         options: Optional[dict] = None,
     ):
```

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/C2.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C2.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/C3.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C3.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/C4.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C4.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/C5.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C5.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/C6.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C6.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/C7.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C7.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/C8.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C8.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/C9.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/C9.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/CA.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/CA.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/CJ.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/CJ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/CK.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/CK.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/CQ.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/CQ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/CT.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/CT.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/Card.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/Card.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/D2.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D2.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/D3.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D3.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/D4.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D4.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/D5.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D5.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/D6.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D6.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/D7.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D7.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/D8.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D8.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/D9.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/D9.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/DA.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/DA.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/DJ.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/DJ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/DK.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/DK.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/DQ.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/DQ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/DT.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/DT.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/H2.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H2.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/H3.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H3.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/H4.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H4.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/H5.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H5.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/H6.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H6.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/H7.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H7.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/H8.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H8.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/H9.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/H9.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/HA.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/HA.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/HJ.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/HJ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/HK.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/HK.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/HQ.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/HQ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/HT.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/HT.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/S2.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S2.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/S3.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S3.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/S4.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S4.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/S5.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S5.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/S6.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S6.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/S7.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S7.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/S8.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S8.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/S9.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/S9.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/SA.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/SA.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/SJ.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/SJ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/SK.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/SK.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/SQ.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/SQ.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/ST.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/ST.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/cab_front.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/cab_front.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/cab_left.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/cab_left.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/cab_rear.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/cab_rear.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/cab_right.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/cab_right.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/cookie.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/cookie.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/cracked_hole.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/cracked_hole.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/elf_down.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/elf_down.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/elf_left.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/elf_left.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/elf_right.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/elf_right.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/elf_up.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/elf_up.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/goal.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/goal.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/gridworld_median_bottom.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/gridworld_median_bottom.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/gridworld_median_horiz.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/gridworld_median_horiz.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/gridworld_median_left.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/gridworld_median_left.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/gridworld_median_right.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/gridworld_median_right.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/gridworld_median_top.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/gridworld_median_top.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/gridworld_median_vert.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/gridworld_median_vert.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/hole.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/hole.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/hotel.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/hotel.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/mountain_bg1.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/mountain_bg1.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/mountain_bg2.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/mountain_bg2.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/mountain_near-cliff1.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/mountain_near-cliff1.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/mountain_near-cliff2.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/mountain_near-cliff2.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/passenger.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/passenger.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/stool.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/stool.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/img/taxi_background.png` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/img/taxi_background.png`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/envs/toy_text/taxi.py` & `gymnasium-1.0.0a1/gymnasium/envs/toy_text/taxi.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,16 @@
         i = categorical_sample([t[0] for t in transitions], self.np_random)
         p, s, r, t = transitions[i]
         self.s = s
         self.lastaction = a
 
         if self.render_mode == "human":
             self.render()
-        return (int(s), r, t, False, {"prob": p, "action_mask": self.action_mask(s)})
+        # truncation=False as the time limit is handled by the `TimeLimit` wrapper added during `make`
+        return int(s), r, t, False, {"prob": p, "action_mask": self.action_mask(s)}
 
     def reset(
         self,
         *,
         seed: Optional[int] = None,
         options: Optional[dict] = None,
     ):
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/functional.py` & `gymnasium-1.0.0a1/gymnasium/functional.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,94 +10,116 @@
 
 StateType = TypeVar("StateType")
 ActType = TypeVar("ActType")
 ObsType = TypeVar("ObsType")
 RewardType = TypeVar("RewardType")
 TerminalType = TypeVar("TerminalType")
 RenderStateType = TypeVar("RenderStateType")
+Params = TypeVar("Params")
 
 
 class FuncEnv(
-    Generic[StateType, ObsType, ActType, RewardType, TerminalType, RenderStateType]
+    Generic[
+        StateType, ObsType, ActType, RewardType, TerminalType, RenderStateType, Params
+    ]
 ):
     """Base class (template) for functional envs.
 
     This API is meant to be used in a stateless manner, with the environment state being passed around explicitly.
     That being said, nothing here prevents users from using the environment statefully, it's just not recommended.
     A functional env consists of the following functions (in this case, instance methods):
-    - initial: returns the initial state of the POMDP
-    - observation: returns the observation in a given state
-    - transition: returns the next state after taking an action in a given state
-    - reward: returns the reward for a given (state, action, next_state) tuple
-    - terminal: returns whether a given state is terminal
-    - state_info: optional, returns a dict of info about a given state
-    - step_info: optional, returns a dict of info about a given (state, action, next_state) tuple
+
+     * initial: returns the initial state of the POMDP
+     * observation: returns the observation in a given state
+     * transition: returns the next state after taking an action in a given state
+     * reward: returns the reward for a given (state, action, next_state) tuple
+     * terminal: returns whether a given state is terminal
+     * state_info: optional, returns a dict of info about a given state
+     * step_info: optional, returns a dict of info about a given (state, action, next_state) tuple
 
     The class-based structure serves the purpose of allowing environment constants to be defined in the class,
     and then using them by name in the code itself.
 
     For the moment, this is predominantly for internal use. This API is likely to change, but in the future
     we intend to flesh it out and officially expose it to end users.
     """
 
     observation_space: Space
     action_space: Space
 
     def __init__(self, options: dict[str, Any] | None = None):
         """Initialize the environment constants."""
         self.__dict__.update(options or {})
+        self.default_params = self.get_default_params()
 
-    def initial(self, rng: Any) -> StateType:
-        """Initial state."""
+    def initial(self, rng: Any, params: Params | None = None) -> StateType:
+        """Generates the initial state of the environment with a random number generator."""
         raise NotImplementedError
 
-    def transition(self, state: StateType, action: ActType, rng: Any) -> StateType:
-        """Transition."""
+    def transition(
+        self, state: StateType, action: ActType, rng: Any, params: Params | None = None
+    ) -> StateType:
+        """Updates (transitions) the state with an action and random number generator."""
         raise NotImplementedError
 
-    def observation(self, state: StateType) -> ObsType:
-        """Observation."""
+    def observation(self, state: StateType, params: Params | None = None) -> ObsType:
+        """Generates an observation for a given state of an environment."""
         raise NotImplementedError
 
     def reward(
-        self, state: StateType, action: ActType, next_state: StateType
+        self,
+        state: StateType,
+        action: ActType,
+        next_state: StateType,
+        params: Params | None = None,
     ) -> RewardType:
-        """Reward."""
+        """Computes the reward for a given transition between `state`, `action` to `next_state`."""
         raise NotImplementedError
 
-    def terminal(self, state: StateType) -> TerminalType:
-        """Terminal state."""
+    def terminal(self, state: StateType, params: Params | None = None) -> TerminalType:
+        """Returns if the state is a final terminal state."""
         raise NotImplementedError
 
-    def state_info(self, state: StateType) -> dict:
+    def state_info(self, state: StateType, params: Params | None = None) -> dict:
         """Info dict about a single state."""
         return {}
 
-    def step_info(
-        self, state: StateType, action: ActType, next_state: StateType
+    def transition_info(
+        self,
+        state: StateType,
+        action: ActType,
+        next_state: StateType,
+        params: Params | None = None,
     ) -> dict:
         """Info dict about a full transition."""
         return {}
 
     def transform(self, func: Callable[[Callable], Callable]):
         """Functional transformations."""
         self.initial = func(self.initial)
         self.transition = func(self.transition)
         self.observation = func(self.observation)
         self.reward = func(self.reward)
         self.terminal = func(self.terminal)
         self.state_info = func(self.state_info)
-        self.step_info = func(self.step_info)
+        self.step_info = func(self.transition_info)
 
     def render_image(
-        self, state: StateType, render_state: RenderStateType
+        self,
+        state: StateType,
+        render_state: RenderStateType,
+        params: Params | None = None,
     ) -> tuple[RenderStateType, np.ndarray]:
         """Show the state."""
         raise NotImplementedError
 
     def render_init(self, **kwargs) -> RenderStateType:
         """Initialize the render state."""
         raise NotImplementedError
 
     def render_close(self, render_state: RenderStateType):
         """Close the render state."""
         raise NotImplementedError
+
+    def get_default_params(self, **kwargs) -> Params | None:
+        """Get the default params."""
+        return None
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/functional_jax_env.py` & `gymnasium-1.0.0a1/gymnasium/envs/functional_jax_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import jax
 import jax.numpy as jnp
 import jax.random as jrng
 import numpy as np
 
 import gymnasium as gym
 from gymnasium.envs.registration import EnvSpec
-from gymnasium.experimental.functional import ActType, FuncEnv, StateType
-from gymnasium.experimental.wrappers.jax_to_numpy import jax_to_numpy
+from gymnasium.functional import ActType, FuncEnv, StateType
 from gymnasium.utils import seeding
 from gymnasium.vector.utils import batch_space
+from gymnasium.wrappers.jax_to_numpy import jax_to_numpy
 
 
 class FunctionalJaxEnv(gym.Env):
     """A conversion layer for jax-based environments."""
 
     state: StateType
     rng: jrng.PRNGKey
@@ -85,15 +85,15 @@
 
         rng, self.rng = jrng.split(self.rng)
 
         next_state = self.func_env.transition(self.state, action, rng)
         observation = self.func_env.observation(next_state)
         reward = self.func_env.reward(self.state, action, next_state)
         terminated = self.func_env.terminal(next_state)
-        info = self.func_env.step_info(self.state, action, next_state)
+        info = self.func_env.transition_info(self.state, action, next_state)
         self.state = next_state
 
         observation = jax_to_numpy(observation)
 
         return observation, float(reward), bool(terminated), False, info
 
     def render(self):
@@ -109,15 +109,15 @@
     def close(self):
         """Closes the environments and render state if set."""
         if self.render_state is not None:
             self.func_env.render_close(self.render_state)
             self.render_state = None
 
 
-class FunctionalJaxVectorEnv(gym.experimental.vector.VectorEnv):
+class FunctionalJaxVectorEnv(gym.vector.VectorEnv):
     """A vector env implementation for functional Jax envs."""
 
     state: StateType
     rng: jrng.PRNGKey
 
     def __init__(
         self,
@@ -147,14 +147,16 @@
         self.render_mode = render_mode
         self.reward_range = reward_range
         self.spec = spec
         self.time_limit = max_episode_steps
 
         self.steps = jnp.zeros(self.num_envs, dtype=jnp.int32)
 
+        self.autoreset_envs = jnp.zeros(self.num_envs, dtype=jnp.bool_)
+
         self._is_box_action_space = isinstance(self.action_space, gym.spaces.Box)
 
         if self.render_mode == "rgb_array":
             self.render_state = self.func_env.render_init()
         else:
             self.render_state = None
 
@@ -207,59 +209,40 @@
         terminated = self.func_env.terminal(next_state)
         truncated = (
             self.steps >= self.time_limit
             if self.time_limit > 0
             else jnp.zeros_like(terminated)
         )
 
-        info = self.func_env.step_info(self.state, action, next_state)
+        info = self.func_env.transition_info(self.state, action, next_state)
 
         done = jnp.logical_or(terminated, truncated)
-        if jnp.any(done):
-            final_obs = self.func_env.observation(next_state)
 
-            to_reset = jnp.where(done)[0]
+        if jnp.any(self.autoreset_envs):
+            to_reset = jnp.where(self.autoreset_envs)[0]
             reset_count = to_reset.shape[0]
 
             rng, self.rng = jrng.split(self.rng)
             rng = jrng.split(rng, reset_count)
 
             new_initials = self.func_env.initial(rng)
 
             next_state = self.state.at[to_reset].set(new_initials)
             self.steps = self.steps.at[to_reset].set(0)
 
-            # Get the final observations and infos
-            info["final_observation"] = np.array([None for _ in range(self.num_envs)])
-            info["final_info"] = np.array([None for _ in range(self.num_envs)])
-
-            info["_final_observation"] = np.array([False for _ in range(self.num_envs)])
-            info["_final_info"] = np.array([False for _ in range(self.num_envs)])
-
-            # TODO: this can maybe be optimized, but right now I don't know how
-            for i in to_reset:
-                info["final_observation"][i] = final_obs[i]
-                info["final_info"][i] = {
-                    k: v[i]
-                    for k, v in info.items()
-                    if k
-                    not in {
-                        "final_observation",
-                        "final_info",
-                        "_final_observation",
-                        "_final_info",
-                    }
-                }
-
-                info["_final_observation"][i] = True
-                info["_final_info"][i] = True
+        self.autoreset_envs = done
 
         observation = self.func_env.observation(next_state)
         observation = jax_to_numpy(observation)
 
+        reward = jax_to_numpy(reward)
+
+        terminated = jax_to_numpy(terminated)
+        truncated = jax_to_numpy(truncated)
+
         self.state = next_state
 
         return observation, reward, terminated, truncated, info
 
     def render(self):
         """Returns the render state if `render_mode` is "rgb_array"."""
         if self.render_mode == "rgb_array":
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/vector/__init__.py` & `gymnasium-1.0.0a1/gymnasium/vector/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Experimental vector env API."""
-from gymnasium.experimental.vector import utils
-from gymnasium.experimental.vector.async_vector_env import AsyncVectorEnv
-from gymnasium.experimental.vector.sync_vector_env import SyncVectorEnv
-from gymnasium.experimental.vector.vector_env import (
+from gymnasium.vector import utils
+from gymnasium.vector.async_vector_env import AsyncVectorEnv
+from gymnasium.vector.sync_vector_env import SyncVectorEnv
+from gymnasium.vector.vector_env import (
     VectorActionWrapper,
     VectorEnv,
     VectorObservationWrapper,
     VectorRewardWrapper,
     VectorWrapper,
 )
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/vector/async_vector_env.py` & `gymnasium-1.0.0a1/gymnasium/vector/async_vector_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,79 +9,105 @@
 from multiprocessing import Queue
 from multiprocessing.connection import Connection
 from typing import Any, Callable, Sequence
 
 import numpy as np
 
 from gymnasium import logger
-from gymnasium.core import Env, ObsType
+from gymnasium.core import ActType, Env, ObsType, RenderFrame
 from gymnasium.error import (
     AlreadyPendingCallError,
     ClosedEnvironmentError,
     CustomSpaceError,
     NoAsyncCallError,
 )
-from gymnasium.experimental.vector.utils import (
+from gymnasium.vector.utils import (
     CloudpickleWrapper,
     batch_space,
     clear_mpi_env_vars,
     concatenate,
     create_empty_array,
     create_shared_memory,
     iterate,
     read_from_shared_memory,
     write_to_shared_memory,
 )
-from gymnasium.experimental.vector.vector_env import VectorEnv
+from gymnasium.vector.vector_env import ArrayType, VectorEnv
 
 
-__all__ = ["AsyncVectorEnv"]
+__all__ = ["AsyncVectorEnv", "AsyncState"]
 
 
 class AsyncState(Enum):
+    """The AsyncVectorEnv possible states given the different actions."""
+
     DEFAULT = "default"
     WAITING_RESET = "reset"
     WAITING_STEP = "step"
     WAITING_CALL = "call"
 
 
 class AsyncVectorEnv(VectorEnv):
     """Vectorized environment that runs multiple environments in parallel.
 
     It uses ``multiprocessing`` processes, and pipes for communication.
 
     Example:
         >>> import gymnasium as gym
-        >>> env = gym.vector.AsyncVectorEnv([
+        >>> envs = gym.make_vec("Pendulum-v1", num_envs=2, vectorization_mode="async")
+        >>> envs
+        AsyncVectorEnv(Pendulum-v1, num_envs=2)
+        >>> envs = gym.vector.AsyncVectorEnv([
         ...     lambda: gym.make("Pendulum-v1", g=9.81),
         ...     lambda: gym.make("Pendulum-v1", g=1.62)
         ... ])
-        >>> env.reset(seed=42)
-        (array([[-0.14995256,  0.9886932 , -0.12224312],
-               [ 0.5760367 ,  0.8174238 , -0.91244936]], dtype=float32), {})
+        >>> envs
+        AsyncVectorEnv(num_envs=2)
+        >>> observations, infos = envs.reset(seed=42)
+        >>> observations
+        array([[-0.14995256,  0.9886932 , -0.12224312],
+               [ 0.5760367 ,  0.8174238 , -0.91244936]], dtype=float32)
+        >>> infos
+        {}
+        >>> _ = envs.action_space.seed(123)
+        >>> observations, rewards, terminations, truncations, infos = envs.step(envs.action_space.sample())
+        >>> observations
+        array([[-0.1851753 ,  0.98270553,  0.714599  ],
+               [ 0.6193494 ,  0.7851154 , -1.0808398 ]], dtype=float32)
+        >>> rewards
+        array([-2.96495728, -1.00214607])
+        >>> terminations
+        array([False, False])
+        >>> truncations
+        array([False, False])
+        >>> infos
+        {}
     """
 
     def __init__(
         self,
         env_fns: Sequence[Callable[[], Env]],
         shared_memory: bool = True,
         copy: bool = True,
         context: str | None = None,
         daemon: bool = True,
-        worker: callable | None = None,
+        worker: Callable[
+            [int, Callable[[], Env], Connection, Connection, bool, Queue], None
+        ]
+        | None = None,
     ):
         """Vectorized environment that runs multiple environments in parallel.
 
         Args:
             env_fns: Functions that create the environments.
             shared_memory: If ``True``, then the observations from the worker processes are communicated back through
                 shared variables. This can improve the efficiency if the observations are large (e.g. images).
-            copy: If ``True``, then the :meth:`~AsyncVectorEnv.reset` and :meth:`~AsyncVectorEnv.step` methods
+            copy: If ``True``, then the :meth:`AsyncVectorEnv.reset` and :meth:`AsyncVectorEnv.step` methods
                 return a copy of the observations.
-            context: Context for `multiprocessing`_. If ``None``, then the default context is used.
+            context: Context for `multiprocessing`. If ``None``, then the default context is used.
             daemon: If ``True``, then subprocesses have ``daemon`` flag turned on; that is, they will quit if
                 the head process quits. However, ``daemon=True`` prevents subprocesses to spawn children,
                 so for some environments you may want to have it set to ``False``.
             worker: If set, then use that worker in a subprocess instead of a default one.
                 Can be useful to override some inner vector env logic, for instance, how resets on termination or truncation are handled.
 
         Warnings:
@@ -91,63 +117,64 @@
 
         Raises:
             RuntimeError: If the observation space of some sub-environment does not match observation_space
                 (or, by default, the observation space of the first sub-environment).
             ValueError: If observation_space is a custom space (i.e. not a default space in Gym,
                 such as gymnasium.spaces.Box, gymnasium.spaces.Discrete, or gymnasium.spaces.Dict) and shared_memory is True.
         """
-        super().__init__()
-
-        ctx = multiprocessing.get_context(context)
         self.env_fns = env_fns
-        self.num_envs = len(env_fns)
         self.shared_memory = shared_memory
         self.copy = copy
 
+        self.num_envs = len(env_fns)
+
         # This would be nice to get rid of, but without it there's a deadlock between shared memory and pipes
+        # Create a dummy environment to gather the metadata and observation / action space of the environment
         dummy_env = env_fns[0]()
+
+        # As we support `make_vec(spec)` then we can't include a `spec = dummy_env.spec` as this doesn't guarantee we can actual recreate the vector env.
         self.metadata = dummy_env.metadata
+        self.render_mode = dummy_env.render_mode
 
         self.single_observation_space = dummy_env.observation_space
         self.single_action_space = dummy_env.action_space
 
         self.observation_space = batch_space(
             self.single_observation_space, self.num_envs
         )
         self.action_space = batch_space(self.single_action_space, self.num_envs)
 
         dummy_env.close()
         del dummy_env
 
+        # Generate the multiprocessing context for the observation buffer
+        ctx = multiprocessing.get_context(context)
         if self.shared_memory:
             try:
                 _obs_buffer = create_shared_memory(
                     self.single_observation_space, n=self.num_envs, ctx=ctx
                 )
                 self.observations = read_from_shared_memory(
                     self.single_observation_space, _obs_buffer, n=self.num_envs
                 )
             except CustomSpaceError as e:
                 raise ValueError(
-                    "Using `shared_memory=True` in `AsyncVectorEnv` "
-                    "is incompatible with non-standard Gymnasium observation spaces "
-                    "(i.e. custom spaces inheriting from `gymnasium.Space`), and is "
-                    "only compatible with default Gymnasium spaces (e.g. `Box`, "
-                    "`Tuple`, `Dict`) for batching. Set `shared_memory=False` "
-                    "if you use custom observation spaces."
+                    "Using `shared_memory=True` in `AsyncVectorEnv` is incompatible with non-standard Gymnasium observation spaces (i.e. custom spaces inheriting from `gymnasium.Space`), "
+                    "and is only compatible with default Gymnasium spaces (e.g. `Box`, `Tuple`, `Dict`) for batching. "
+                    "Set `shared_memory=False` if you use custom observation spaces."
                 ) from e
         else:
             _obs_buffer = None
             self.observations = create_empty_array(
                 self.single_observation_space, n=self.num_envs, fn=np.zeros
             )
 
         self.parent_pipes, self.processes = [], []
         self.error_queue = ctx.Queue()
-        target = worker or _worker
+        target = worker or _async_worker
         with clear_mpi_env_vars():
             for idx, env_fn in enumerate(self.env_fns):
                 parent_pipe, child_pipe = ctx.Pipe()
                 process = ctx.Process(
                     target=target,
                     name=f"Worker<{type(self).__name__}>-{idx}",
                     args=(
@@ -166,14 +193,32 @@
                 process.daemon = daemon
                 process.start()
                 child_pipe.close()
 
         self._state = AsyncState.DEFAULT
         self._check_spaces()
 
+    def reset(
+        self,
+        *,
+        seed: int | list[int] | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> tuple[ObsType, dict[str, Any]]:
+        """Resets all sub-environments in parallel and return a batch of concatenated observations and info.
+
+        Args:
+            seed: The environment reset seeds
+            options: If to return the options
+
+        Returns:
+            A batch of observations and info from the vectorized environment.
+        """
+        self.reset_async(seed=seed, options=options)
+        return self.reset_wait()
+
     def reset_async(
         self,
         seed: int | list[int] | None = None,
         options: dict | None = None,
     ):
         """Send calls to the :obj:`reset` methods of the sub-environments.
 
@@ -189,42 +234,37 @@
                 method (e.g. :meth:`step_async`). This can be caused by two consecutive
                 calls to :meth:`reset_async`, with no call to :meth:`reset_wait` in between.
         """
         self._assert_is_running()
 
         if seed is None:
             seed = [None for _ in range(self.num_envs)]
-        if isinstance(seed, int):
+        elif isinstance(seed, int):
             seed = [seed + i for i in range(self.num_envs)]
         assert len(seed) == self.num_envs
 
         if self._state != AsyncState.DEFAULT:
             raise AlreadyPendingCallError(
                 f"Calling `reset_async` while waiting for a pending call to `{self._state.value}` to complete",
                 str(self._state.value),
             )
 
-        for pipe, single_seed in zip(self.parent_pipes, seed):
-            single_kwargs = {}
-            if single_seed is not None:
-                single_kwargs["seed"] = single_seed
-            if options is not None:
-                single_kwargs["options"] = options
-
-            pipe.send(("reset", single_kwargs))
+        for pipe, env_seed in zip(self.parent_pipes, seed):
+            env_kwargs = {"seed": env_seed, "options": options}
+            pipe.send(("reset", env_kwargs))
         self._state = AsyncState.WAITING_RESET
 
     def reset_wait(
         self,
         timeout: int | float | None = None,
-    ) -> tuple[ObsType, list[dict]]:
+    ) -> tuple[ObsType, dict[str, Any]]:
         """Waits for the calls triggered by :meth:`reset_async` to finish and returns the results.
 
         Args:
-            timeout: Number of seconds before the call to `reset_wait` times out. If `None`, the call to `reset_wait` never times out.
+            timeout: Number of seconds before the call to ``reset_wait`` times out. If `None`, the call to ``reset_wait`` never times out.
 
         Returns:
             A tuple of batched observations and list of dictionaries
 
         Raises:
             ClosedEnvironmentError: If the environment was closed (if :meth:`close` was previously called).
             NoAsyncCallError: If :meth:`reset_wait` was called without any prior call to :meth:`reset_async`.
@@ -233,59 +273,55 @@
         self._assert_is_running()
         if self._state != AsyncState.WAITING_RESET:
             raise NoAsyncCallError(
                 "Calling `reset_wait` without any prior " "call to `reset_async`.",
                 AsyncState.WAITING_RESET.value,
             )
 
-        if not self._poll(timeout):
+        if not self._poll_pipe_envs(timeout):
             self._state = AsyncState.DEFAULT
             raise multiprocessing.TimeoutError(
                 f"The call to `reset_wait` has timed out after {timeout} second(s)."
             )
 
         results, successes = zip(*[pipe.recv() for pipe in self.parent_pipes])
         self._raise_if_errors(successes)
-        self._state = AsyncState.DEFAULT
 
         infos = {}
         results, info_data = zip(*results)
         for i, info in enumerate(info_data):
             infos = self._add_info(infos, info, i)
 
         if not self.shared_memory:
             self.observations = concatenate(
                 self.single_observation_space, results, self.observations
             )
 
+        self._state = AsyncState.DEFAULT
         return (deepcopy(self.observations) if self.copy else self.observations), infos
 
-    def reset(
-        self,
-        *,
-        seed: int | list[int] | None = None,
-        options: dict | None = None,
-    ):
-        """Reset all parallel environments and return a batch of initial observations and info.
+    def step(
+        self, actions: ActType
+    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict[str, Any]]:
+        """Take an action for each parallel environment.
 
         Args:
-            seed: The environment reset seeds
-            options: If to return the options
+            actions: element of :attr:`action_space` batch of actions.
 
         Returns:
-            A batch of observations and info from the vectorized environment.
+            Batch of (observations, rewards, terminations, truncations, infos)
         """
-        self.reset_async(seed=seed, options=options)
-        return self.reset_wait()
+        self.step_async(actions)
+        return self.step_wait()
 
     def step_async(self, actions: np.ndarray):
-        """Send the calls to :obj:`step` to each sub-environment.
+        """Send the calls to :meth:`Env.step` to each sub-environment.
 
         Args:
-            actions: Batch of actions. element of :attr:`~VectorEnv.action_space`
+            actions: Batch of actions. element of :attr:`VectorEnv.action_space`
 
         Raises:
             ClosedEnvironmentError: If the environment was closed (if :meth:`close` was previously called).
             AlreadyPendingCallError: If the environment is already waiting for a pending call to another
                 method (e.g. :meth:`reset_async`). This can be caused by two consecutive
                 calls to :meth:`step_async`, with no call to :meth:`step_wait` in
                 between.
@@ -293,16 +329,16 @@
         self._assert_is_running()
         if self._state != AsyncState.DEFAULT:
             raise AlreadyPendingCallError(
                 f"Calling `step_async` while waiting for a pending call to `{self._state.value}` to complete.",
                 str(self._state.value),
             )
 
-        actions = iterate(self.action_space, actions)
-        for pipe, action in zip(self.parent_pipes, actions):
+        iter_actions = iterate(self.action_space, actions)
+        for pipe, action in zip(self.parent_pipes, iter_actions):
             pipe.send(("step", action))
         self._state = AsyncState.WAITING_STEP
 
     def step_wait(
         self, timeout: int | float | None = None
     ) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, dict]:
         """Wait for the calls to :obj:`step` in each sub-environment to finish.
@@ -321,63 +357,68 @@
         self._assert_is_running()
         if self._state != AsyncState.WAITING_STEP:
             raise NoAsyncCallError(
                 "Calling `step_wait` without any prior call " "to `step_async`.",
                 AsyncState.WAITING_STEP.value,
             )
 
-        if not self._poll(timeout):
+        if not self._poll_pipe_envs(timeout):
             self._state = AsyncState.DEFAULT
             raise multiprocessing.TimeoutError(
                 f"The call to `step_wait` has timed out after {timeout} second(s)."
             )
 
-        observations_list, rewards, terminateds, truncateds, infos = [], [], [], [], {}
+        observations, rewards, terminations, truncations, infos = [], [], [], [], {}
         successes = []
-        for i, pipe in enumerate(self.parent_pipes):
-            result, success = pipe.recv()
-            obs, rew, terminated, truncated, info = result
+        for env_idx, pipe in enumerate(self.parent_pipes):
+            env_step_return, success = pipe.recv()
 
             successes.append(success)
             if success:
-                observations_list.append(obs)
-                rewards.append(rew)
-                terminateds.append(terminated)
-                truncateds.append(truncated)
-                infos = self._add_info(infos, info, i)
+                observations.append(env_step_return[0])
+                rewards.append(env_step_return[1])
+                terminations.append(env_step_return[2])
+                truncations.append(env_step_return[3])
+                infos = self._add_info(infos, env_step_return[4], env_idx)
 
         self._raise_if_errors(successes)
-        self._state = AsyncState.DEFAULT
 
         if not self.shared_memory:
             self.observations = concatenate(
                 self.single_observation_space,
-                observations_list,
+                observations,
                 self.observations,
             )
 
+        self._state = AsyncState.DEFAULT
         return (
             deepcopy(self.observations) if self.copy else self.observations,
-            np.array(rewards),
-            np.array(terminateds, dtype=np.bool_),
-            np.array(truncateds, dtype=np.bool_),
+            np.array(rewards, dtype=np.float64),
+            np.array(terminations, dtype=np.bool_),
+            np.array(truncations, dtype=np.bool_),
             infos,
         )
 
-    def step(self, actions):
-        """Take an action for each parallel environment.
+    def call(self, name: str, *args: Any, **kwargs: Any) -> tuple[Any, ...]:
+        """Call a method from each parallel environment with args and kwargs.
 
         Args:
-            actions: element of :attr:`action_space` Batch of actions.
+            name (str): Name of the method or property to call.
+            *args: Position arguments to apply to the method call.
+            **kwargs: Keyword arguments to apply to the method call.
 
         Returns:
-            Batch of (observations, rewards, terminations, truncations, infos)
+            List of the results of the individual calls to the method or property for each environment.
         """
-        self.step_async(actions)
-        return self.step_wait()
+        self.call_async(name, *args, **kwargs)
+        return self.call_wait()
+
+    def render(self) -> tuple[RenderFrame, ...] | None:
+        """Returns a list of rendered frames from the environments."""
+        return self.call("render")
 
     def call_async(self, name: str, *args, **kwargs):
         """Calls the method with name asynchronously and apply args and kwargs to the method.
 
         Args:
             name: Name of the method or property to call.
             *args: Arguments to apply to the method call.
@@ -386,70 +427,55 @@
         Raises:
             ClosedEnvironmentError: If the environment was closed (if :meth:`close` was previously called).
             AlreadyPendingCallError: Calling `call_async` while waiting for a pending call to complete
         """
         self._assert_is_running()
         if self._state != AsyncState.DEFAULT:
             raise AlreadyPendingCallError(
-                "Calling `call_async` while waiting "
-                f"for a pending call to `{self._state.value}` to complete.",
+                f"Calling `call_async` while waiting for a pending call to `{self._state.value}` to complete.",
                 str(self._state.value),
             )
 
         for pipe in self.parent_pipes:
             pipe.send(("_call", (name, args, kwargs)))
         self._state = AsyncState.WAITING_CALL
 
-    def call_wait(self, timeout: int | float | None = None) -> list:
+    def call_wait(self, timeout: int | float | None = None) -> tuple[Any, ...]:
         """Calls all parent pipes and waits for the results.
 
         Args:
-            timeout: Number of seconds before the call to `step_wait` times out.
-                If `None` (default), the call to `step_wait` never times out.
+            timeout: Number of seconds before the call to :meth:`step_wait` times out.
+                If ``None`` (default), the call to :meth:`step_wait` never times out.
 
         Returns:
             List of the results of the individual calls to the method or property for each environment.
 
         Raises:
-            NoAsyncCallError: Calling `call_wait` without any prior call to `call_async`.
-            TimeoutError: The call to `call_wait` has timed out after timeout second(s).
+            NoAsyncCallError: Calling :meth:`call_wait` without any prior call to :meth:`call_async`.
+            TimeoutError: The call to :meth:`call_wait` has timed out after timeout second(s).
         """
         self._assert_is_running()
         if self._state != AsyncState.WAITING_CALL:
             raise NoAsyncCallError(
                 "Calling `call_wait` without any prior call to `call_async`.",
                 AsyncState.WAITING_CALL.value,
             )
 
-        if not self._poll(timeout):
+        if not self._poll_pipe_envs(timeout):
             self._state = AsyncState.DEFAULT
             raise multiprocessing.TimeoutError(
                 f"The call to `call_wait` has timed out after {timeout} second(s)."
             )
 
         results, successes = zip(*[pipe.recv() for pipe in self.parent_pipes])
         self._raise_if_errors(successes)
         self._state = AsyncState.DEFAULT
 
         return results
 
-    def call(self, name: str, *args, **kwargs) -> list[Any]:
-        """Call a method, or get a property, from each parallel environment.
-
-        Args:
-            name (str): Name of the method or property to call.
-            *args: Arguments to apply to the method call.
-            **kwargs: Keyword arguments to apply to the method call.
-
-        Returns:
-            List of the results of the individual calls to the method or property for each environment.
-        """
-        self.call_async(name, *args, **kwargs)
-        return self.call_wait()
-
     def get_attr(self, name: str):
         """Get a property from each parallel environment.
 
         Args:
             name (str): Name of the property to be get from each individual environment.
 
         Returns:
@@ -464,30 +490,28 @@
             name: Name of the property to be set in each individual environment.
             values: Values of the property to be set to. If ``values`` is a list or
                 tuple, then it corresponds to the values for each individual
                 environment, otherwise a single value is set for all environments.
 
         Raises:
             ValueError: Values must be a list or tuple with length equal to the number of environments.
-            AlreadyPendingCallError: Calling `set_attr` while waiting for a pending call to complete.
+            AlreadyPendingCallError: Calling :meth:`set_attr` while waiting for a pending call to complete.
         """
         self._assert_is_running()
         if not isinstance(values, (list, tuple)):
             values = [values for _ in range(self.num_envs)]
         if len(values) != self.num_envs:
             raise ValueError(
-                "Values must be a list or tuple with length equal to the "
-                f"number of environments. Got `{len(values)}` values for "
-                f"{self.num_envs} environments."
+                "Values must be a list or tuple with length equal to the number of environments. "
+                f"Got `{len(values)}` values for {self.num_envs} environments."
             )
 
         if self._state != AsyncState.DEFAULT:
             raise AlreadyPendingCallError(
-                "Calling `set_attr` while waiting "
-                f"for a pending call to `{self._state.value}` to complete.",
+                f"Calling `set_attr` while waiting for a pending call to `{self._state.value}` to complete.",
                 str(self._state.value),
             )
 
         for pipe, value in zip(self.parent_pipes, values):
             pipe.send(("_setattr", (name, value)))
         _, successes = zip(*[pipe.recv() for pipe in self.parent_pipes])
         self._raise_if_errors(successes)
@@ -529,36 +553,41 @@
 
         for pipe in self.parent_pipes:
             if pipe is not None:
                 pipe.close()
         for process in self.processes:
             process.join()
 
-    def _poll(self, timeout=None):
+    def _poll_pipe_envs(self, timeout: int | None = None):
         self._assert_is_running()
+
         if timeout is None:
             return True
+
         end_time = time.perf_counter() + timeout
-        delta = None
         for pipe in self.parent_pipes:
             delta = max(end_time - time.perf_counter(), 0)
+
             if pipe is None:
                 return False
             if pipe.closed or (not pipe.poll(delta)):
                 return False
         return True
 
     def _check_spaces(self):
         self._assert_is_running()
         spaces = (self.single_observation_space, self.single_action_space)
+
         for pipe in self.parent_pipes:
             pipe.send(("_check_spaces", spaces))
+
         results, successes = zip(*[pipe.recv() for pipe in self.parent_pipes])
         self._raise_if_errors(successes)
         same_observation_spaces, same_action_spaces = zip(*results)
+
         if not all(same_observation_spaces):
             raise RuntimeError(
                 f"Some environments have an observation space different from `{self.single_observation_space}`. "
                 "In order to batch observations, the observation spaces from all environments must be equal."
             )
         if not all(same_action_spaces):
             raise RuntimeError(
@@ -576,110 +605,110 @@
         if all(successes):
             return
 
         num_errors = self.num_envs - sum(successes)
         assert num_errors > 0
         for i in range(num_errors):
             index, exctype, value = self.error_queue.get()
+
             logger.error(
                 f"Received the following error from Worker-{index}: {exctype.__name__}: {value}"
             )
             logger.error(f"Shutting down Worker-{index}.")
+
             self.parent_pipes[index].close()
             self.parent_pipes[index] = None
 
             if i == num_errors - 1:
                 logger.error("Raising the last exception back to the main process.")
                 raise exctype(value)
 
     def __del__(self):
         """On deleting the object, checks that the vector environment is closed."""
         if not getattr(self, "closed", True) and hasattr(self, "_state"):
             self.close(terminate=True)
 
 
-def _worker(
+def _async_worker(
     index: int,
     env_fn: callable,
     pipe: Connection,
     parent_pipe: Connection,
     shared_memory: bool,
     error_queue: Queue,
 ):
     env = env_fn()
     observation_space = env.observation_space
     action_space = env.action_space
+    autoreset = False
+
     parent_pipe.close()
+
     try:
         while True:
             command, data = pipe.recv()
 
             if command == "reset":
                 observation, info = env.reset(**data)
                 if shared_memory:
                     write_to_shared_memory(
                         observation_space, index, observation, shared_memory
                     )
                     observation = None
+                    autoreset = False
                 pipe.send(((observation, info), True))
-
             elif command == "step":
-                (
-                    observation,
-                    reward,
-                    terminated,
-                    truncated,
-                    info,
-                ) = env.step(data)
-                if terminated or truncated:
-                    old_observation, old_info = observation, info
+                if autoreset:
                     observation, info = env.reset()
-                    info["final_observation"] = old_observation
-                    info["final_info"] = old_info
+                    reward, terminated, truncated = 0, False, False
+                else:
+                    (
+                        observation,
+                        reward,
+                        terminated,
+                        truncated,
+                        info,
+                    ) = env.step(data)
+                autoreset = terminated or truncated
 
                 if shared_memory:
                     write_to_shared_memory(
                         observation_space, index, observation, shared_memory
                     )
                     observation = None
 
                 pipe.send(((observation, reward, terminated, truncated, info), True))
-            elif command == "seed":
-                env.seed(data)
-                pipe.send((None, True))
             elif command == "close":
                 pipe.send((None, True))
                 break
             elif command == "_call":
                 name, args, kwargs = data
-                if name in ["reset", "step", "seed", "close"]:
+                if name in ["reset", "step", "close", "set_wrapper_attr"]:
                     raise ValueError(
-                        f"Trying to call function `{name}` with "
-                        f"`_call`. Use `{name}` directly instead."
+                        f"Trying to call function `{name}` with `call`, use `{name}` directly instead."
                     )
-                function = getattr(env, name)
-                if callable(function):
-                    pipe.send((function(*args, **kwargs), True))
+
+                attr = env.get_wrapper_attr(name)
+                if callable(attr):
+                    pipe.send((attr(*args, **kwargs), True))
                 else:
-                    pipe.send((function, True))
+                    pipe.send((attr, True))
             elif command == "_setattr":
                 name, value = data
-                setattr(env, name, value)
+                env.set_wrapper_attr(name, value)
                 pipe.send((None, True))
             elif command == "_check_spaces":
                 pipe.send(
                     (
                         (data[0] == observation_space, data[1] == action_space),
                         True,
                     )
                 )
             else:
                 raise RuntimeError(
-                    f"Received unknown command `{command}`. Must "
-                    "be one of {`reset`, `step`, `seed`, `close`, `_call`, "
-                    "`_setattr`, `_check_spaces`}."
+                    f"Received unknown command `{command}`. Must be one of [`reset`, `step`, `close`, `_call`, `_setattr`, `_check_spaces`]."
                 )
     except (KeyboardInterrupt, Exception):
         error_queue.put((index,) + sys.exc_info()[:2])
         pipe.send((None, False))
     finally:
         env.close()
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/vector/sync_vector_env.py` & `gymnasium-1.0.0a1/gymnasium/vector/sync_vector_env.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,229 +1,268 @@
-"""A synchronous vector environment."""
+"""Implementation of a synchronous (for loop) vectorization method of any environment."""
 from __future__ import annotations
 
 from copy import deepcopy
-from typing import Any, Callable, Iterator
+from typing import Any, Callable, Iterator, Sequence
 
 import numpy as np
 
 from gymnasium import Env
-from gymnasium.experimental.vector.utils import (
-    batch_space,
-    concatenate,
-    create_empty_array,
-    iterate,
-)
-from gymnasium.experimental.vector.vector_env import VectorEnv
+from gymnasium.core import ActType, ObsType, RenderFrame
+from gymnasium.vector.utils import batch_space, concatenate, create_empty_array, iterate
+from gymnasium.vector.vector_env import ArrayType, VectorEnv
 
 
 __all__ = ["SyncVectorEnv"]
 
 
 class SyncVectorEnv(VectorEnv):
     """Vectorized environment that serially runs multiple environments.
 
     Example:
         >>> import gymnasium as gym
-        >>> env = gym.vector.SyncVectorEnv([
+        >>> envs = gym.make_vec("Pendulum-v1", num_envs=2, vectorization_mode="sync")
+        >>> envs
+        SyncVectorEnv(Pendulum-v1, num_envs=2)
+        >>> envs = gym.vector.SyncVectorEnv([
         ...     lambda: gym.make("Pendulum-v1", g=9.81),
         ...     lambda: gym.make("Pendulum-v1", g=1.62)
         ... ])
-        >>> env.reset(seed=42)
-        (array([[-0.14995256,  0.9886932 , -0.12224312],
-               [ 0.5760367 ,  0.8174238 , -0.91244936]], dtype=float32), {})
+        >>> envs
+        SyncVectorEnv(num_envs=2)
+        >>> obs, infos = envs.reset(seed=42)
+        >>> obs
+        array([[-0.14995256,  0.9886932 , -0.12224312],
+               [ 0.5760367 ,  0.8174238 , -0.91244936]], dtype=float32)
+        >>> infos
+        {}
+        >>> _ = envs.action_space.seed(42)
+        >>> actions = envs.action_space.sample()
+        >>> obs, rewards, terminates, truncates, infos = envs.step(actions)
+        >>> obs
+        array([[-0.1878752 ,  0.98219293,  0.7695615 ],
+               [ 0.6102389 ,  0.79221743, -0.8498053 ]], dtype=float32)
+        >>> rewards
+        array([-2.96562607, -0.99902063])
+        >>> terminates
+        array([False, False])
+        >>> truncates
+        array([False, False])
+        >>> infos
+        {}
+        >>> envs.close()
     """
 
     def __init__(
         self,
-        env_fns: Iterator[Callable[[], Env]],
+        env_fns: Iterator[Callable[[], Env]] | Sequence[Callable[[], Env]],
         copy: bool = True,
     ):
         """Vectorized environment that serially runs multiple environments.
 
         Args:
             env_fns: iterable of callable functions that create the environments.
             copy: If ``True``, then the :meth:`reset` and :meth:`step` methods return a copy of the observations.
 
         Raises:
             RuntimeError: If the observation space of some sub-environment does not match observation_space
                 (or, by default, the observation space of the first sub-environment).
         """
-        super().__init__()
+        self.copy = copy
         self.env_fns = env_fns
+
+        # Initialise all sub-environments
         self.envs = [env_fn() for env_fn in env_fns]
+
+        # Define core attributes using the sub-environments
+        # As we support `make_vec(spec)` then we can't include a `spec = self.envs[0].spec` as this doesn't guarantee we can actual recreate the vector env.
         self.num_envs = len(self.envs)
-        self.copy = copy
         self.metadata = self.envs[0].metadata
+        self.render_mode = self.envs[0].render_mode
 
-        self.spec = self.envs[0].spec
-
+        # Initialises the single spaces from the sub-environments
         self.single_observation_space = self.envs[0].observation_space
         self.single_action_space = self.envs[0].action_space
+        self._check_spaces()
 
+        # Initialise the obs and action space based on the single versions and num of sub-environments
         self.observation_space = batch_space(
             self.single_observation_space, self.num_envs
         )
         self.action_space = batch_space(self.single_action_space, self.num_envs)
 
-        self._check_spaces()
-        self.observations = create_empty_array(
+        # Initialise attributes used in `step` and `reset`
+        self._observations = create_empty_array(
             self.single_observation_space, n=self.num_envs, fn=np.zeros
         )
         self._rewards = np.zeros((self.num_envs,), dtype=np.float64)
-        self._terminateds = np.zeros((self.num_envs,), dtype=np.bool_)
-        self._truncateds = np.zeros((self.num_envs,), dtype=np.bool_)
+        self._terminations = np.zeros((self.num_envs,), dtype=np.bool_)
+        self._truncations = np.zeros((self.num_envs,), dtype=np.bool_)
+
+        self._autoreset_envs = np.zeros((self.num_envs,), dtype=np.bool_)
 
     def reset(
         self,
+        *,
         seed: int | list[int] | None = None,
-        options: dict | None = None,
-    ):
-        """Waits for the calls triggered by :meth:`reset_async` to finish and returns the results.
+        options: dict[str, Any] | None = None,
+    ) -> tuple[ObsType, dict[str, Any]]:
+        """Resets each of the sub-environments and concatenate the results together.
 
         Args:
-            seed: The reset environment seed
-            options: Option information for the environment reset
+            seed: Seeds used to reset the sub-environments, either
+                * ``None`` - random seeds for all environment
+                * ``int`` - ``[seed, seed+1, ..., seed+n]``
+                * List of ints - ``[1, 2, 3, ..., n]``
+            options: Option information used for each sub-environment
 
         Returns:
-            The reset observation of the environment and reset information
+            Concatenated observations and info from each sub-environment
         """
         if seed is None:
             seed = [None for _ in range(self.num_envs)]
-        if isinstance(seed, int):
+        elif isinstance(seed, int):
             seed = [seed + i for i in range(self.num_envs)]
         assert len(seed) == self.num_envs
 
-        self._terminateds[:] = False
-        self._truncateds[:] = False
-        observations = []
-        infos = {}
+        self._terminations = np.zeros((self.num_envs,), dtype=np.bool_)
+        self._truncations = np.zeros((self.num_envs,), dtype=np.bool_)
+
+        observations, infos = [], {}
         for i, (env, single_seed) in enumerate(zip(self.envs, seed)):
-            kwargs = {}
-            if single_seed is not None:
-                kwargs["seed"] = single_seed
-            if options is not None:
-                kwargs["options"] = options
-
-            observation, info = env.reset(**kwargs)
-            observations.append(observation)
-            infos = self._add_info(infos, info, i)
+            env_obs, env_info = env.reset(seed=single_seed, options=options)
 
-        self.observations = concatenate(
-            self.single_observation_space, observations, self.observations
+            observations.append(env_obs)
+            infos = self._add_info(infos, env_info, i)
+
+        # Concatenate the observations
+        self._observations = concatenate(
+            self.single_observation_space, observations, self._observations
         )
-        return (deepcopy(self.observations) if self.copy else self.observations), infos
 
-    def step(self, actions):
+        return deepcopy(self._observations) if self.copy else self._observations, infos
+
+    def step(
+        self, actions: ActType
+    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict[str, Any]]:
         """Steps through each of the environments returning the batched results.
 
         Returns:
             The batched environment step results
         """
         actions = iterate(self.action_space, actions)
 
         observations, infos = [], {}
-        for i, (env, action) in enumerate(zip(self.envs, actions)):
-            (
-                observation,
-                self._rewards[i],
-                self._terminateds[i],
-                self._truncateds[i],
-                info,
-            ) = env.step(action)
-
-            if self._terminateds[i] or self._truncateds[i]:
-                old_observation, old_info = observation, info
-                observation, info = env.reset()
-                info["final_observation"] = old_observation
-                info["final_info"] = old_info
-            observations.append(observation)
-            infos = self._add_info(infos, info, i)
-        self.observations = concatenate(
-            self.single_observation_space, observations, self.observations
+        for i, action in enumerate(actions):
+            if self._autoreset_envs[i]:
+                env_obs, env_info = self.envs[i].reset()
+
+                self._rewards[i] = 0.0
+                self._terminations[i] = False
+                self._truncations[i] = False
+            else:
+                (
+                    env_obs,
+                    self._rewards[i],
+                    self._terminations[i],
+                    self._truncations[i],
+                    env_info,
+                ) = self.envs[i].step(action)
+
+            observations.append(env_obs)
+            infos = self._add_info(infos, env_info, i)
+
+        # Concatenate the observations
+        self._observations = concatenate(
+            self.single_observation_space, observations, self._observations
         )
+        self._autoreset_envs = np.logical_or(self._terminations, self._truncations)
 
         return (
-            deepcopy(self.observations) if self.copy else self.observations,
+            deepcopy(self._observations) if self.copy else self._observations,
             np.copy(self._rewards),
-            np.copy(self._terminateds),
-            np.copy(self._truncateds),
+            np.copy(self._terminations),
+            np.copy(self._truncations),
             infos,
         )
 
-    def call(self, name, *args, **kwargs) -> tuple:
-        """Calls the method with name and applies args and kwargs.
+    def render(self) -> tuple[RenderFrame, ...] | None:
+        """Returns the rendered frames from the environments."""
+        return tuple(env.render() for env in self.envs)
+
+    def call(self, name: str, *args: Any, **kwargs: Any) -> tuple[Any, ...]:
+        """Calls a sub-environment method with name and applies args and kwargs.
 
         Args:
             name: The method name
             *args: The method args
             **kwargs: The method kwargs
 
         Returns:
             Tuple of results
         """
         results = []
         for env in self.envs:
-            function = getattr(env, name)
+            function = env.get_wrapper_attr(name)
+
             if callable(function):
                 results.append(function(*args, **kwargs))
             else:
                 results.append(function)
 
         return tuple(results)
 
-    def get_attr(self, name: str):
+    def get_attr(self, name: str) -> Any:
         """Get a property from each parallel environment.
 
         Args:
-            name (str): Name of the property to be get from each individual environment.
+            name (str): Name of the property to get from each individual environment.
 
         Returns:
             The property with name
         """
         return self.call(name)
 
-    def set_attr(self, name: str, values: list | tuple | Any):
+    def set_attr(self, name: str, values: list[Any] | tuple[Any, ...] | Any):
         """Sets an attribute of the sub-environments.
 
         Args:
             name: The property name to change
             values: Values of the property to be set to. If ``values`` is a list or
                 tuple, then it corresponds to the values for each individual
                 environment, otherwise, a single value is set for all environments.
 
         Raises:
             ValueError: Values must be a list or tuple with length equal to the number of environments.
         """
         if not isinstance(values, (list, tuple)):
             values = [values for _ in range(self.num_envs)]
+
         if len(values) != self.num_envs:
             raise ValueError(
-                "Values must be a list or tuple with length equal to the "
-                f"number of environments. Got `{len(values)}` values for "
-                f"{self.num_envs} environments."
+                "Values must be a list or tuple with length equal to the number of environments. "
+                f"Got `{len(values)}` values for {self.num_envs} environments."
             )
 
         for env, value in zip(self.envs, values):
-            setattr(env, name, value)
+            env.set_wrapper_attr(name, value)
 
-    def close_extras(self, **kwargs):
+    def close_extras(self, **kwargs: Any):
         """Close the environments."""
         [env.close() for env in self.envs]
 
     def _check_spaces(self) -> bool:
+        """Check that each of the environments obs and action spaces are equivalent to the single obs and action space."""
         for env in self.envs:
             if not (env.observation_space == self.single_observation_space):
                 raise RuntimeError(
-                    "Some environments have an observation space different from "
-                    f"`{self.single_observation_space}`. In order to batch observations, "
-                    "the observation spaces from all environments must be equal."
+                    f"Some environments have an observation space different from `{self.single_observation_space}`. "
+                    "In order to batch observations, the observation spaces from all environments must be equal."
                 )
 
             if not (env.action_space == self.single_action_space):
                 raise RuntimeError(
-                    "Some environments have an action space different from "
-                    f"`{self.single_action_space}`. In order to batch actions, the "
-                    "action spaces from all environments must be equal."
+                    f"Some environments have an action space different from `{self.single_action_space}`. "
+                    "In order to batch actions, the action spaces from all environments must be equal."
                 )
 
         return True
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/vector/utils/__init__.py` & `gymnasium-1.0.0a1/gymnasium/vector/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 """Module for gymnasium experimental vector utility functions."""
 
-from gymnasium.experimental.vector.utils.misc import (
-    CloudpickleWrapper,
-    clear_mpi_env_vars,
-)
-from gymnasium.experimental.vector.utils.shared_memory import (
+from gymnasium.vector.utils.misc import CloudpickleWrapper, clear_mpi_env_vars
+from gymnasium.vector.utils.shared_memory import (
     create_shared_memory,
     read_from_shared_memory,
     write_to_shared_memory,
 )
-from gymnasium.experimental.vector.utils.space_utils import (
+from gymnasium.vector.utils.space_utils import (
     batch_space,
     concatenate,
     create_empty_array,
     iterate,
 )
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/vector/utils/misc.py` & `gymnasium-1.0.0a1/gymnasium/vector/utils/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         return self.fn()
 
 
 @contextlib.contextmanager
 def clear_mpi_env_vars():
     """Clears the MPI of environment variables.
 
-    `from mpi4py import MPI` will call `MPI_Init` by default.
+    ``from mpi4py import MPI`` will call ``MPI_Init`` by default.
     If the child process has MPI environment variables, MPI will think that the child process
     is an MPI process just like the parent and do bad things such as hang.
 
     This context manager is a hacky way to clear those environment variables
     temporarily such as when we are starting multiprocessing Processes.
 
     Yields:
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/vector/utils/shared_memory.py` & `gymnasium-1.0.0a1/gymnasium/vector/utils/shared_memory.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/experimental/vector/utils/space_utils.py` & `gymnasium-1.0.0a1/gymnasium/vector/utils/space_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         items: Samples to be concatenated.
         out: The output object. This object is a (possibly nested) numpy array.
 
     Returns:
         The output object. This object is a (possibly nested) numpy array.
 
     Raises:
-        ValueError: Space is not an instance of :class:`gym.Space`
+        ValueError: Space is not an instance of :class:`gymnasium.Space`
 
     Example:
         >>> from gymnasium.spaces import Box, Dict
         >>> import numpy as np
         >>> space = Dict({
         ... 'position': Box(low=0, high=1, shape=(2, 3), seed=42, dtype=np.float32),
         ... 'velocity': Box(low=0, high=1, shape=(2, 2), seed=42, dtype=np.float32)})
@@ -307,22 +307,22 @@
 ) -> tuple[Any, ...] | dict[str, Any] | np.ndarray:
     """Create an empty (possibly nested) (normally numpy-based) array, used in conjunction with ``concatenate(..., out=array)``.
 
     In most cases, the array will be contained within the batched space, however, this is not guaranteed.
 
     Args:
         space: Observation space of a single environment in the vectorized environment.
-        n: Number of environments in the vectorized environment. If `None`, creates an empty sample from `space`.
-        fn: Function to apply when creating the empty numpy array. Examples of such functions are `np.empty` or `np.zeros`.
+        n: Number of environments in the vectorized environment. If ``None``, creates an empty sample from ``space``.
+        fn: Function to apply when creating the empty numpy array. Examples of such functions are ``np.empty`` or ``np.zeros``.
 
     Returns:
         The output object. This object is a (possibly nested) numpy array.
 
     Raises:
-        ValueError: Space is not a valid :class:`gym.Space` instance
+        ValueError: Space is not a valid :class:`gymnasium.Space` instance
 
     Example:
         >>> from gymnasium.spaces import Box, Dict
         >>> import numpy as np
         >>> space = Dict({
         ... 'position': Box(low=0, high=1, shape=(3,), dtype=np.float32),
         ... 'velocity': Box(low=0, high=1, shape=(2,), dtype=np.float32)})
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/vector/vector_env.py` & `gymnasium-1.0.0a1/gymnasium/vector/vector_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Generic, TypeVar
 
 import numpy as np
 
 import gymnasium as gym
-from gymnasium.core import ActType, ObsType
+from gymnasium.core import ActType, ObsType, RenderFrame
 from gymnasium.utils import seeding
 
 
 if TYPE_CHECKING:
     from gymnasium.envs.registration import EnvSpec
 
 ArrayType = TypeVar("ArrayType")
@@ -27,57 +27,86 @@
 
 
 class VectorEnv(Generic[ObsType, ActType, ArrayType]):
     """Base class for vectorized environments to run multiple independent copies of the same environment in parallel.
 
     Vector environments can provide a linear speed-up in the steps taken per second through sampling multiple
     sub-environments at the same time. To prevent terminated environments waiting until all sub-environments have
-    terminated or truncated, the vector environments autoreset sub-environments after they terminate or truncated.
-    As a result, the final step's observation and info are overwritten by the reset's observation and info.
-    Therefore, the observation and info for the final step of a sub-environment is stored in the info parameter,
+    terminated or truncated, the vector environments automatically reset sub-environments after they terminate or truncated (within the same step call).
+    As a result, the step's observation and info are overwritten by the reset's observation and info.
+    To preserve this data, the observation and info for the final step of a sub-environment is stored in the info parameter,
     using `"final_observation"` and `"final_info"` respectively. See :meth:`step` for more information.
 
-    The vector environments batch `observations`, `rewards`, `terminations`, `truncations` and `info` for each
-    parallel environment. In addition, :meth:`step` expects to receive a batch of actions for each parallel environment.
+    The vector environments batches `observations`, `rewards`, `terminations`, `truncations` and `info` for each
+    sub-environment. In addition, :meth:`step` expects to receive a batch of actions for each parallel environment.
 
-    Gymnasium contains two types of Vector environments: :class:`AsyncVectorEnv` and :class:`SyncVectorEnv`.
+    Gymnasium contains two generalised Vector environments: :class:`AsyncVectorEnv` and :class:`SyncVectorEnv` along with
+    several custom vector environment implementations.
 
     The Vector Environments have the additional attributes for users to understand the implementation
 
     - :attr:`num_envs` - The number of sub-environment in the vector environment
     - :attr:`observation_space` - The batched observation space of the vector environment
     - :attr:`single_observation_space` - The observation space of a single sub-environment
     - :attr:`action_space` - The batched action space of the vector environment
     - :attr:`single_action_space` - The action space of a single sub-environment
 
-    Note:
-        The info parameter of :meth:`reset` and :meth:`step` was originally implemented before OpenAI Gym v25 was a list
-        of dictionary for each sub-environment. However, this was modified in OpenAI Gym v25+ and in Gymnasium to a
-        dictionary with a NumPy array for each key. To use the old info style using the :class:`VectorListInfo`.
+    Examples:
+        >>> import gymnasium as gym
+        >>> envs = gym.make_vec("CartPole-v1", num_envs=3, vectorization_mode="sync", wrappers=(gym.wrappers.TimeAwareObservation,))
+        >>> envs = gym.wrappers.vector.ClipReward(envs, min_reward=0.2, max_reward=0.8)
+        >>> envs
+        <ClipReward, SyncVectorEnv(CartPole-v1, num_envs=3)>
+        >>> observations, infos = envs.reset(seed=123)
+        >>> observations
+        array([[ 0.01823519, -0.0446179 , -0.02796401, -0.03156282,  0.        ],
+               [ 0.02852531,  0.02858594,  0.0469136 ,  0.02480598,  0.        ],
+               [ 0.03517495, -0.000635  , -0.01098382, -0.03203924,  0.        ]])
+        >>> infos
+        {}
+        >>> _ = envs.action_space.seed(123)
+        >>> observations, rewards, terminations, truncations, infos = envs.step(envs.action_space.sample())
+        >>> observations
+        array([[ 0.01734283,  0.15089367, -0.02859527, -0.33293587,  1.        ],
+               [ 0.02909703, -0.16717631,  0.04740972,  0.3319138 ,  1.        ],
+               [ 0.03516225, -0.19559774, -0.01162461,  0.25715804,  1.        ]])
+        >>> rewards
+        array([0.8, 0.8, 0.8])
+        >>> terminations
+        array([False, False, False])
+        >>> truncations
+        array([False, False, False])
+        >>> infos
+        {}
+        >>> envs.close()
 
     Note:
-        To render the sub-environments, use :meth:`call` with "render" arguments. Remember to set the `render_modes`
-        for all the sub-environments during initialization.
+        The info parameter of :meth:`reset` and :meth:`step` was originally implemented before v0.25 as a list
+        of dictionary for each sub-environment. However, this was modified in v0.25+ to be a
+        dictionary with a NumPy array for each key. To use the old info style, utilise the :class:`DictInfoToList` wrapper.
 
     Note:
         All parallel environments should share the identical observation and action spaces.
         In other words, a vector of multiple different environments is not supported.
+
+    Note:
+        :func:`make_vec` is the equivalent function to :func:`make` for vector environments.
     """
 
-    spec: EnvSpec
+    spec: EnvSpec | None = None
+    render_mode: str | None = None
+    closed: bool = False
 
     observation_space: gym.Space
     action_space: gym.Space
     single_observation_space: gym.Space
     single_action_space: gym.Space
 
     num_envs: int
 
-    closed = False
-
     _np_random: np.random.Generator | None = None
 
     def reset(
         self,
         *,
         seed: int | list[int] | None = None,
         options: dict[str, Any] | None = None,
@@ -89,68 +118,76 @@
             options: If to return the options
 
         Returns:
             A batch of observations and info from the vectorized environment.
 
         Example:
             >>> import gymnasium as gym
-            >>> envs = gym.vector.make("CartPole-v1", num_envs=3)
-            >>> envs.reset(seed=42)
-            (array([[ 0.0273956 , -0.00611216,  0.03585979,  0.0197368 ],
+            >>> envs = gym.make_vec("CartPole-v1", num_envs=3, vectorization_mode="sync")
+            >>> observations, infos = envs.reset(seed=42)
+            >>> observations
+            array([[ 0.0273956 , -0.00611216,  0.03585979,  0.0197368 ],
                    [ 0.01522993, -0.04562247, -0.04799704,  0.03392126],
                    [-0.03774345, -0.02418869, -0.00942293,  0.0469184 ]],
-                  dtype=float32), {})
+                  dtype=float32)
+            >>> infos
+            {}
         """
         if seed is not None:
             self._np_random, seed = seeding.np_random(seed)
 
     def step(
         self, actions: ActType
-    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict]:
+    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict[str, Any]]:
         """Take an action for each parallel environment.
 
         Args:
-            actions: element of :attr:`action_space` Batch of actions.
+            actions: Batch of actions with the :attr:`action_space` shape.
 
         Returns:
             Batch of (observations, rewards, terminations, truncations, infos)
 
         Note:
             As the vector environments autoreset for a terminating and truncating sub-environments,
             the returned observation and info is not the final step's observation or info which is instead stored in
             info as `"final_observation"` and `"final_info"`.
 
         Example:
             >>> import gymnasium as gym
             >>> import numpy as np
-            >>> envs = gym.vector.make("CartPole-v1", num_envs=3)
+            >>> envs = gym.make_vec("CartPole-v1", num_envs=3, vectorization_mode="sync")
             >>> _ = envs.reset(seed=42)
-            >>> actions = np.array([1, 0, 1])
-            >>> observations, rewards, termination, truncation, infos = envs.step(actions)
+            >>> actions = np.array([1, 0, 1], dtype=np.int32)
+            >>> observations, rewards, terminations, truncations, infos = envs.step(actions)
             >>> observations
             array([[ 0.02727336,  0.18847767,  0.03625453, -0.26141977],
                    [ 0.01431748, -0.24002443, -0.04731862,  0.3110827 ],
                    [-0.03822722,  0.1710671 , -0.00848456, -0.2487226 ]],
                   dtype=float32)
             >>> rewards
             array([1., 1., 1.])
-            >>> termination
+            >>> terminations
             array([False, False, False])
-            >>> termination
+            >>> terminations
             array([False, False, False])
             >>> infos
             {}
         """
-        pass
 
-    def close_extras(self, **kwargs):
-        """Clean up the extra resources e.g. beyond what's in this base class."""
-        pass
+    def render(self) -> tuple[RenderFrame, ...] | None:
+        """Returns the rendered frames from the parallel environments.
+
+        Returns:
+            A tuple of rendered frames from the parallel environments
+        """
+        raise NotImplementedError(
+            f"{self.__str__()} render function is not implemented."
+        )
 
-    def close(self, **kwargs):
+    def close(self, **kwargs: Any):
         """Close all parallel environments and release resources.
 
         It also closes all the existing image viewers, then calls :meth:`close_extras` and set
         :attr:`closed` as ``True``.
 
         Warnings:
             This function itself does not close the environments, it should be handled
@@ -165,14 +202,18 @@
         """
         if self.closed:
             return
 
         self.close_extras(**kwargs)
         self.closed = True
 
+    def close_extras(self, **kwargs: Any):
+        """Clean up the extra resources e.g. beyond what's in this base class."""
+        pass
+
     @property
     def np_random(self) -> np.random.Generator:
         """Returns the environment's internal :attr:`_np_random` that if not set will initialise with a random seed.
 
         Returns:
             Instances of `np.random.Generator`
         """
@@ -185,152 +226,151 @@
         self._np_random = value
 
     @property
     def unwrapped(self):
         """Return the base environment."""
         return self
 
-    def _add_info(self, infos: dict, info: dict, env_num: int) -> dict:
+    def _add_info(
+        self, vector_infos: dict[str, Any], env_info: dict[str, Any], env_num: int
+    ) -> dict[str, Any]:
         """Add env info to the info dictionary of the vectorized environment.
 
         Given the `info` of a single environment add it to the `infos` dictionary
         which represents all the infos of the vectorized environment.
         Every `key` of `info` is paired with a boolean mask `_key` representing
         whether or not the i-indexed environment has this `info`.
 
         Args:
-            infos (dict): the infos of the vectorized environment
-            info (dict): the info coming from the single environment
+            vector_infos (dict): the infos of the vectorized environment
+            env_info (dict): the info coming from the single environment
             env_num (int): the index of the single environment
 
         Returns:
             infos (dict): the (updated) infos of the vectorized environment
-
         """
-        for k in info.keys():
-            if k not in infos:
-                info_array, array_mask = self._init_info_arrays(type(info[k]))
+        for key, value in env_info.items():
+            # If value is a dictionary, then we apply the `_add_info` recursively.
+            if isinstance(value, dict):
+                array = self._add_info(vector_infos.get(key, {}), value, env_num)
+            # Otherwise, we are a base case to group the data
             else:
-                info_array, array_mask = infos[k], infos[f"_{k}"]
-
-            info_array[env_num], array_mask[env_num] = info[k], True
-            infos[k], infos[f"_{k}"] = info_array, array_mask
-        return infos
-
-    def _init_info_arrays(self, dtype: type) -> tuple[np.ndarray, np.ndarray]:
-        """Initialize the info array.
-
-        Initialize the info array. If the dtype is numeric
-        the info array will have the same dtype, otherwise
-        will be an array of `None`. Also, a boolean array
-        of the same length is returned. It will be used for
-        assessing which environment has info data.
-
-        Args:
-            dtype (type): data type of the info coming from the env.
+                # If the key doesn't exist in the vector infos, then we can create an array of that batch type
+                if key not in vector_infos:
+                    if type(value) in [int, float, bool] or issubclass(
+                        type(value), np.number
+                    ):
+                        array = np.zeros(self.num_envs, dtype=type(value))
+                    elif isinstance(value, np.ndarray):
+                        # We assume that all instances of the np.array info are of the same shape
+                        array = np.zeros(
+                            (self.num_envs, *value.shape), dtype=value.dtype
+                        )
+                    else:
+                        # For unknown objects, we use a Numpy object array
+                        array = np.full(self.num_envs, fill_value=None, dtype=object)
+                # Otherwise, just use the array that already exists
+                else:
+                    array = vector_infos[key]
+
+                # Assign the data in the `env_num` position
+                #   We only want to run this for the base-case data (not recursive data forcing the ugly function structure)
+                array[env_num] = value
+
+            # Get the array mask and if it doesn't already exist then create a zero bool array
+            array_mask = vector_infos.get(
+                f"_{key}", np.zeros(self.num_envs, dtype=np.bool_)
+            )
+            array_mask[env_num] = True
 
-        Returns:
-            array (np.ndarray): the initialized info array.
-            array_mask (np.ndarray): the initialized boolean array.
+            # Update the vector info with the updated data and mask information
+            vector_infos[key], vector_infos[f"_{key}"] = array, array_mask
 
-        """
-        if dtype in [int, float, bool] or issubclass(dtype, np.number):
-            array = np.zeros(self.num_envs, dtype=dtype)
-        else:
-            array = np.zeros(self.num_envs, dtype=object)
-            array[:] = None
-        array_mask = np.zeros(self.num_envs, dtype=bool)
-        return array, array_mask
+        return vector_infos
 
     def __del__(self):
         """Closes the vector environment."""
         if not getattr(self, "closed", True):
             self.close()
 
     def __repr__(self) -> str:
         """Returns a string representation of the vector environment.
 
         Returns:
             A string containing the class name, number of environments and environment spec id
         """
-        if getattr(self, "spec", None) is None:
-            return f"{self.__class__.__name__}({self.num_envs})"
+        if self.spec is None:
+            return f"{self.__class__.__name__}(num_envs={self.num_envs})"
         else:
-            return f"{self.__class__.__name__}({self.spec.id}, {self.num_envs})"
+            return (
+                f"{self.__class__.__name__}({self.spec.id}, num_envs={self.num_envs})"
+            )
 
 
 class VectorWrapper(VectorEnv):
     """Wraps the vectorized environment to allow a modular transformation.
 
     This class is the base class for all wrappers for vectorized environments. The subclass
     could override some methods to change the behavior of the original vectorized environment
     without touching the original code.
 
     Note:
         Don't forget to call ``super().__init__(env)`` if the subclass overrides :meth:`__init__`.
     """
 
-    _observation_space: gym.Space | None = None
-    _action_space: gym.Space | None = None
-    _single_observation_space: gym.Space | None = None
-    _single_action_space: gym.Space | None = None
-
     def __init__(self, env: VectorEnv):
-        """Initialize the vectorized environment wrapper."""
-        super().__init__()
+        """Initialize the vectorized environment wrapper.
 
-        assert isinstance(env, VectorEnv)
+        Args:
+            env: The environment to wrap
+        """
         self.env = env
+        assert isinstance(env, VectorEnv)
 
-    # explicitly forward the methods defined in VectorEnv
-    # to self.env (instead of the base class)
+        self._observation_space: gym.Space | None = None
+        self._action_space: gym.Space | None = None
+        self._single_observation_space: gym.Space | None = None
+        self._single_action_space: gym.Space | None = None
 
     def reset(
         self,
         *,
         seed: int | list[int] | None = None,
         options: dict[str, Any] | None = None,
     ) -> tuple[ObsType, dict[str, Any]]:
         """Reset all environment using seed and options."""
         return self.env.reset(seed=seed, options=options)
 
     def step(
         self, actions: ActType
-    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict]:
-        """Step all environments."""
+    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict[str, Any]]:
+        """Step through all environments using the actions returning the batched data."""
         return self.env.step(actions)
 
+    def render(self) -> tuple[RenderFrame, ...] | None:
+        """Returns the render mode from the base vector environment."""
+        return self.env.render()
+
     def close(self, **kwargs: Any):
         """Close all environments."""
         return self.env.close(**kwargs)
 
     def close_extras(self, **kwargs: Any):
         """Close all extra resources."""
         return self.env.close_extras(**kwargs)
 
-    # implicitly forward all other methods and attributes to self.env
-    def __getattr__(self, name: str) -> Any:
-        """Forward all other attributes to the base environment."""
-        if name.startswith("_"):
-            raise AttributeError(f"attempted to get missing private attribute '{name}'")
-        return getattr(self.env, name)
-
     @property
     def unwrapped(self):
         """Return the base non-wrapped environment."""
         return self.env.unwrapped
 
     def __repr__(self):
         """Return the string representation of the vectorized environment."""
         return f"<{self.__class__.__name__}, {self.env}>"
 
-    def __del__(self):
-        """Close the vectorized environment."""
-        self.env.__del__()
-
     @property
     def spec(self) -> EnvSpec | None:
         """Gets the specification of the wrapped environment."""
         return self.env.spec
 
     @property
     def observation_space(self) -> gym.Space:
@@ -381,78 +421,70 @@
         self._single_action_space = space
 
     @property
     def num_envs(self) -> int:
         """Gets the wrapped vector environment's num of the sub-environments."""
         return self.env.num_envs
 
+    @property
+    def render_mode(self) -> tuple[RenderFrame, ...] | None:
+        """Returns the `render_mode` from the base environment."""
+        return self.env.render_mode
+
 
 class VectorObservationWrapper(VectorWrapper):
-    """Wraps the vectorized environment to allow a modular transformation of the observation. Equivalent to :class:`gym.ObservationWrapper` for vectorized environments."""
+    """Wraps the vectorized environment to allow a modular transformation of the observation.
+
+    Equivalent to :class:`gymnasium.ObservationWrapper` for vectorized environments.
+    """
 
     def reset(
         self,
         *,
         seed: int | list[int] | None = None,
         options: dict[str, Any] | None = None,
     ) -> tuple[ObsType, dict[str, Any]]:
         """Modifies the observation returned from the environment ``reset`` using the :meth:`observation`."""
-        obs, info = self.env.reset(seed=seed, options=options)
-        return self.vector_observation(obs), info
+        observations, infos = self.env.reset(seed=seed, options=options)
+        return self.observations(observations), infos
 
     def step(
         self, actions: ActType
-    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict]:
+    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict[str, Any]]:
         """Modifies the observation returned from the environment ``step`` using the :meth:`observation`."""
-        observation, reward, termination, truncation, info = self.env.step(actions)
+        observations, rewards, terminations, truncations, infos = self.env.step(actions)
         return (
-            self.vector_observation(observation),
-            reward,
-            termination,
-            truncation,
-            self.update_final_obs(info),
+            self.observations(observations),
+            rewards,
+            terminations,
+            truncations,
+            infos,
         )
 
-    def vector_observation(self, observation: ObsType) -> ObsType:
+    def observations(self, observations: ObsType) -> ObsType:
         """Defines the vector observation transformation.
 
         Args:
-            observation: A vector observation from the environment
+            observations: A vector observation from the environment
 
         Returns:
             the transformed observation
         """
         raise NotImplementedError
 
-    def single_observation(self, observation: ObsType) -> ObsType:
-        """Defines the single observation transformation.
-
-        Args:
-            observation: A single observation from the environment
-
-        Returns:
-            The transformed observation
-        """
-        raise NotImplementedError
-
-    def update_final_obs(self, info: dict[str, Any]) -> dict[str, Any]:
-        """Updates the `final_obs` in the info using `single_observation`."""
-        if "final_observation" in info:
-            for i, obs in enumerate(info["final_observation"]):
-                if obs is not None:
-                    info["final_observation"][i] = self.single_observation(obs)
-        return info
-
 
 class VectorActionWrapper(VectorWrapper):
-    """Wraps the vectorized environment to allow a modular transformation of the actions. Equivalent of :class:`~gym.ActionWrapper` for vectorized environments."""
+    """Wraps the vectorized environment to allow a modular transformation of the actions.
+
+    Equivalent of :class:`gymnasium.ActionWrapper` for vectorized environments.
+    """
 
     def step(
         self, actions: ActType
-    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict]:
+    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict[str, Any]]:
         """Steps through the environment using a modified action by :meth:`action`."""
         return self.env.step(self.actions(actions))
 
     def actions(self, actions: ActType) -> ActType:
         """Transform the actions before sending them to the environment.
 
         Args:
@@ -461,26 +493,29 @@
         Returns:
             ActType: the transformed actions
         """
         raise NotImplementedError
 
 
 class VectorRewardWrapper(VectorWrapper):
-    """Wraps the vectorized environment to allow a modular transformation of the reward. Equivalent of :class:`~gym.RewardWrapper` for vectorized environments."""
+    """Wraps the vectorized environment to allow a modular transformation of the reward.
+
+    Equivalent of :class:`gymnasium.RewardWrapper` for vectorized environments.
+    """
 
     def step(
         self, actions: ActType
-    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict]:
+    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict[str, Any]]:
         """Steps through the environment returning a reward modified by :meth:`reward`."""
-        observation, reward, termination, truncation, info = self.env.step(actions)
-        return observation, self.reward(reward), termination, truncation, info
+        observations, rewards, terminations, truncations, infos = self.env.step(actions)
+        return observations, self.rewards(rewards), terminations, truncations, infos
 
-    def reward(self, reward: ArrayType) -> ArrayType:
+    def rewards(self, rewards: ArrayType) -> ArrayType:
         """Transform the reward before returning it.
 
         Args:
-            reward (array): the reward to transform
+            rewards (array): the reward to transform
 
         Returns:
             array: the transformed reward
         """
         raise NotImplementedError
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/__init__.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,153 @@
-"""`__init__` for experimental wrappers, to avoid loading the wrappers if unnecessary, we can hack python."""
+"""Wrappers are a convenient way to modify an existing environment without having to alter the underlying code directly.
+
+Using wrappers will allow you to avoid a lot of boilerplate code and make your environment more modular.
+Importantly wrappers can be chained to combine their effects and most environments that are generated via
+:meth:`gymnasium.make` will already be wrapped by default.
+
+In order to wrap an environment, you must first initialize a base environment. Then you can pass this environment along
+with (possibly optional) parameters to the wrapper's constructor.
+
+    >>> import gymnasium as gym
+    >>> from gymnasium.wrappers import RescaleAction
+    >>> base_env = gym.make("Hopper-v4")
+    >>> base_env.action_space
+    Box(-1.0, 1.0, (3,), float32)
+    >>> wrapped_env = RescaleAction(base_env, min_action=0, max_action=1)
+    >>> wrapped_env.action_space
+    Box(0.0, 1.0, (3,), float32)
+
+You can access the environment underneath the **first** wrapper by using the :attr:`gymnasium.Wrapper.env` attribute.
+As the :class:`gymnasium.Wrapper` class inherits from :class:`gymnasium.Env` then :attr:`gymnasium.Wrapper.env` can be another wrapper.
+
+    >>> wrapped_env
+    <RescaleAction<TimeLimit<OrderEnforcing<PassiveEnvChecker<HopperEnv<Hopper-v4>>>>>>
+    >>> wrapped_env.env
+    <TimeLimit<OrderEnforcing<PassiveEnvChecker<HopperEnv<Hopper-v4>>>>>
+
+If you want to get to the environment underneath **all** of the layers of wrappers, you can use the
+:attr:`gymnasium.Wrapper.unwrapped` attribute.
+If the environment is already a bare environment, the :attr:`gymnasium.Wrapper.unwrapped` attribute will just return itself.
+
+    >>> wrapped_env
+    <RescaleAction<TimeLimit<OrderEnforcing<PassiveEnvChecker<HopperEnv<Hopper-v4>>>>>>
+    >>> wrapped_env.unwrapped # doctest: +SKIP
+    <gymnasium.envs.mujoco.hopper_v4.HopperEnv object at 0x7fbb5efd0490>
+
+There are three common things you might want a wrapper to do:
+
+- Transform actions before applying them to the base environment
+- Transform observations that are returned by the base environment
+- Transform rewards that are returned by the base environment
+
+Such wrappers can be easily implemented by inheriting from :class:`gymnasium.ActionWrapper`,
+:class:`gymnasium.ObservationWrapper`, or :class:`gymnasium.RewardWrapper` and implementing the respective transformation.
+If you need a wrapper to do more complicated tasks, you can inherit from the :class:`gymnasium.Wrapper` class directly.
+
+If you'd like to implement your own custom wrapper, check out `the corresponding tutorial <../../tutorials/implementing_custom_wrappers>`_.
+"""
 # pyright: reportUnsupportedDunderAll=false
 import importlib
-import re
 
-from gymnasium.error import DeprecatedWrapper
-from gymnasium.experimental.wrappers import vector
-from gymnasium.experimental.wrappers.atari_preprocessing import AtariPreprocessingV0
-from gymnasium.experimental.wrappers.common import (
-    AutoresetV0,
-    OrderEnforcingV0,
-    PassiveEnvCheckerV0,
-    RecordEpisodeStatisticsV0,
-)
-from gymnasium.experimental.wrappers.lambda_action import (
-    ClipActionV0,
-    LambdaActionV0,
-    RescaleActionV0,
+from gymnasium.wrappers import vector
+from gymnasium.wrappers.atari_preprocessing import AtariPreprocessing
+from gymnasium.wrappers.common import (
+    Autoreset,
+    OrderEnforcing,
+    PassiveEnvChecker,
+    RecordEpisodeStatistics,
+    TimeLimit,
 )
-from gymnasium.experimental.wrappers.lambda_observation import (
-    DtypeObservationV0,
-    FilterObservationV0,
-    FlattenObservationV0,
-    GrayscaleObservationV0,
-    LambdaObservationV0,
-    PixelObservationV0,
-    RescaleObservationV0,
-    ReshapeObservationV0,
-    ResizeObservationV0,
+from gymnasium.wrappers.rendering import HumanRendering, RecordVideo, RenderCollection
+from gymnasium.wrappers.stateful_action import StickyAction
+from gymnasium.wrappers.stateful_observation import (
+    DelayObservation,
+    FrameStackObservation,
+    MaxAndSkipObservation,
+    NormalizeObservation,
+    TimeAwareObservation,
 )
-from gymnasium.experimental.wrappers.lambda_reward import ClipRewardV0, LambdaRewardV0
-from gymnasium.experimental.wrappers.rendering import (
-    HumanRenderingV0,
-    RecordVideoV0,
-    RenderCollectionV0,
+from gymnasium.wrappers.stateful_reward import NormalizeReward
+from gymnasium.wrappers.transform_action import (
+    ClipAction,
+    RescaleAction,
+    TransformAction,
 )
-from gymnasium.experimental.wrappers.stateful_action import StickyActionV0
-from gymnasium.experimental.wrappers.stateful_observation import (
-    DelayObservationV0,
-    FrameStackObservationV0,
-    MaxAndSkipObservationV0,
-    NormalizeObservationV0,
-    TimeAwareObservationV0,
+from gymnasium.wrappers.transform_observation import (
+    AddRenderObservation,
+    DtypeObservation,
+    FilterObservation,
+    FlattenObservation,
+    GrayscaleObservation,
+    RescaleObservation,
+    ReshapeObservation,
+    ResizeObservation,
+    TransformObservation,
 )
-from gymnasium.experimental.wrappers.stateful_reward import NormalizeRewardV1
-
-
-# Todo - Add legacy wrapper to new wrapper error for users when merged into gymnasium.wrappers
+from gymnasium.wrappers.transform_reward import ClipReward, TransformReward
 
 
 __all__ = [
     "vector",
     # --- Observation wrappers ---
-    "AtariPreprocessingV0",
-    "DelayObservationV0",
-    "DtypeObservationV0",
-    "FilterObservationV0",
-    "FlattenObservationV0",
-    "FrameStackObservationV0",
-    "GrayscaleObservationV0",
-    "LambdaObservationV0",
-    "MaxAndSkipObservationV0",
-    "NormalizeObservationV0",
-    "PixelObservationV0",
-    "ResizeObservationV0",
-    "ReshapeObservationV0",
-    "RescaleObservationV0",
-    "TimeAwareObservationV0",
+    "AtariPreprocessing",
+    "DelayObservation",
+    "DtypeObservation",
+    "FilterObservation",
+    "FlattenObservation",
+    "FrameStackObservation",
+    "GrayscaleObservation",
+    "TransformObservation",
+    "MaxAndSkipObservation",
+    "NormalizeObservation",
+    "AddRenderObservation",
+    "ResizeObservation",
+    "ReshapeObservation",
+    "RescaleObservation",
+    "TimeAwareObservation",
     # --- Action Wrappers ---
-    "ClipActionV0",
-    "LambdaActionV0",
-    "RescaleActionV0",
+    "ClipAction",
+    "TransformAction",
+    "RescaleAction",
     # "NanAction",
-    "StickyActionV0",
+    "StickyAction",
     # --- Reward wrappers ---
-    "ClipRewardV0",
-    "LambdaRewardV0",
-    "NormalizeRewardV1",
+    "ClipReward",
+    "TransformReward",
+    "NormalizeReward",
     # --- Common ---
-    "AutoresetV0",
-    "PassiveEnvCheckerV0",
-    "OrderEnforcingV0",
-    "RecordEpisodeStatisticsV0",
+    "TimeLimit",
+    "Autoreset",
+    "PassiveEnvChecker",
+    "OrderEnforcing",
+    "RecordEpisodeStatistics",
     # --- Rendering ---
-    "RenderCollectionV0",
-    "RecordVideoV0",
-    "HumanRenderingV0",
+    "RenderCollection",
+    "RecordVideo",
+    "HumanRendering",
     # --- Conversion ---
-    "JaxToNumpyV0",
-    "JaxToTorchV0",
-    "NumpyToTorchV0",
+    "JaxToNumpy",
+    "JaxToTorch",
+    "NumpyToTorch",
 ]
 
 # As these wrappers requires `jax` or `torch`, they are loaded by runtime for users trying to access them
 #   to avoid `import jax` or `import torch` on `import gymnasium`.
 _wrapper_to_class = {
     # data converters
-    "JaxToNumpyV0": "jax_to_numpy",
-    "JaxToTorchV0": "jax_to_torch",
-    "NumpyToTorchV0": "numpy_to_torch",
+    "JaxToNumpy": "jax_to_numpy",
+    "JaxToTorch": "jax_to_torch",
+    "NumpyToTorch": "numpy_to_torch",
+}
+
+_renamed_wrapper = {
+    "AutoResetWrapper": "Autoreset",
+    "FrameStack": "FrameStackObservation",
+    "PixelObservationWrapper": "AddRenderObservation",
+    "VectorListInfo": "vector.DictInfoToList",
 }
 
 
 def __getattr__(wrapper_name: str):
     """Load a wrapper by name.
 
     This optimizes the loading of gymnasium wrappers by only loading the wrapper if it is used.
@@ -115,50 +161,17 @@
 
     Raises:
         AttributeError: If the wrapper does not exist.
         DeprecatedWrapper: If the version is not the latest.
     """
     # Check if the requested wrapper is in the _wrapper_to_class dictionary
     if wrapper_name in _wrapper_to_class:
-        import_stmt = (
-            f"gymnasium.experimental.wrappers.{_wrapper_to_class[wrapper_name]}"
-        )
+        import_stmt = f"gymnasium.wrappers.{_wrapper_to_class[wrapper_name]}"
         module = importlib.import_module(import_stmt)
         return getattr(module, wrapper_name)
 
-    # Define a regex pattern to match the integer suffix (version number) of the wrapper
-    int_suffix_pattern = r"(\d+)$"
-    version_match = re.search(int_suffix_pattern, wrapper_name)
-
-    # If a version number is found, extract it and the base wrapper name
-    if version_match:
-        version = int(version_match.group())
-        base_name = wrapper_name[: -len(version_match.group())]
-    else:
-        version = float("inf")
-        base_name = wrapper_name[:-2]
-
-    # Filter the list of all wrappers to include only those with the same base name
-    matching_wrappers = [name for name in __all__ if name.startswith(base_name)]
-
-    # If no matching wrappers are found, raise an AttributeError
-    if not matching_wrappers:
-        raise AttributeError(f"module {__name__!r} has no attribute {wrapper_name!r}")
-
-    # Find the latest version of the matching wrappers
-    latest_wrapper = max(
-        matching_wrappers, key=lambda s: int(re.findall(int_suffix_pattern, s)[0])
-    )
-    latest_version = int(re.findall(int_suffix_pattern, latest_wrapper)[0])
-
-    # If the requested wrapper is an older version, raise a DeprecatedWrapper exception
-    if version < latest_version:
-        raise DeprecatedWrapper(
-            f"{wrapper_name!r} is now deprecated, use {latest_wrapper!r} instead.\n"
-            f"To see the changes made, go to "
-            f"https://gymnasium.farama.org/api/experimental/wrappers/#gymnasium.experimental.wrappers.{latest_wrapper}"
-        )
-    # If the requested version is invalid, raise an AttributeError
-    else:
+    elif wrapper_name in _renamed_wrapper:
         raise AttributeError(
-            f"module {__name__!r} has no attribute {wrapper_name!r}, did you mean {latest_wrapper!r}"
+            f"{wrapper_name!r} has been renamed with `wrappers.{_renamed_wrapper[wrapper_name]}`"
         )
+
+    raise AttributeError(f"module {__name__!r} has no attribute {wrapper_name!r}")
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/atari_preprocessing.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/atari_preprocessing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 """Implementation of Atari 2600 Preprocessing following the guidelines of Machado et al., 2018."""
+from __future__ import annotations
+
+from typing import Any, SupportsFloat
+
 import numpy as np
 
 import gymnasium as gym
+from gymnasium.core import WrapperActType, WrapperObsType
 from gymnasium.spaces import Box
 
 
-__all__ = ["AtariPreprocessingV0"]
+__all__ = ["AtariPreprocessing"]
+
 
+class AtariPreprocessing(gym.Wrapper, gym.utils.RecordConstructorArgs):
+    """Implements the common preprocessing techniques for Atari environments (excluding frame stacking).
 
-class AtariPreprocessingV0(gym.Wrapper, gym.utils.RecordConstructorArgs):
-    """Atari 2600 preprocessing wrapper.
+    For frame stacking use :class:`gymnasium.wrappers.FrameStackObservation`.
+    No vector version of the wrapper exists
 
     This class follows the guidelines in Machado et al. (2018),
     "Revisiting the Arcade Learning Environment: Evaluation Protocols and Open Problems for General Agents".
 
     Specifically, the following preprocess stages applies to the atari environment:
 
     - Noop Reset: Obtains the initial state by taking a random number of no-ops on reset, default max 30 no-ops.
-    - Frame skipping: The number of frames skipped between steps, 4 by default
-    - Max-pooling: Pools over the most recent two observations from the frame skips
+    - Frame skipping: The number of frames skipped between steps, 4 by default.
+    - Max-pooling: Pools over the most recent two observations from the frame skips.
     - Termination signal when a life is lost: When the agent losses a life during the environment, then the environment is terminated.
         Turned off by default. Not recommended by Machado et al. (2018).
-    - Resize to a square image: Resizes the atari environment original observation shape from 210x180 to 84x84 by default
-    - Grayscale observation: If the observation is colour or greyscale, by default, greyscale.
-    - Scale observation: If to scale the observation between [0, 1) or [0, 255), by default, not scaled.
+    - Resize to a square image: Resizes the atari environment original observation shape from 210x180 to 84x84 by default.
+    - Grayscale observation: Makes the observation greyscale, enabled by default.
+    - Grayscale new axis: Extends the last channel of the observation such that the image is 3-dimensional, not enabled by default.
+    - Scale observation: Whether to scale the observation between [0, 1) or [0, 255), not scaled by default.
+
+    Example:
+        >>> import gymnasium as gym # doctest: +SKIP
+        >>> env = gym.make("ALE/Adventure-v5") # doctest: +SKIP
+        >>> env = AtariPreprocessing(env, noop_max=10, frame_skip=0, screen_size=84, terminal_on_life_loss=True, grayscale_obs=False, grayscale_newaxis=False) # doctest: +SKIP
+
+    Change logs:
+     * Added in gym v0.12.2 (gym #1455)
     """
 
     def __init__(
         self,
         env: gym.Env,
         noop_max: int = 30,
         frame_skip: int = 4,
@@ -39,15 +56,15 @@
     ):
         """Wrapper for Atari 2600 preprocessing.
 
         Args:
             env (Env): The environment to apply the preprocessing
             noop_max (int): For No-op reset, the max number no-ops actions are taken at reset, to turn off, set to 0.
             frame_skip (int): The number of frames between new observation the agents observations effecting the frequency at which the agent experiences the game.
-            screen_size (int): resize Atari frame
+            screen_size (int): resize Atari frame.
             terminal_on_life_loss (bool): `if True`, then :meth:`step()` returns `terminated=True` whenever a
                 life is lost.
             grayscale_obs (bool): if True, then gray scale observation is returned, otherwise, RGB observation
                 is returned.
             grayscale_newaxis (bool): `if True and grayscale_obs=True`, then a channel axis is added to
                 grayscale observations to make them 3-dimensional.
             scale_obs (bool): if True, then observation normalized in range [0,1) is returned. It also limits memory
@@ -75,24 +92,18 @@
             raise gym.error.DependencyNotInstalled(
                 "opencv-python package not installed, run `pip install gymnasium[other]` to get dependencies for atari"
             )
 
         assert frame_skip > 0
         assert screen_size > 0
         assert noop_max >= 0
-        if frame_skip > 1:
-            if (
-                env.spec is not None
-                and "NoFrameskip" not in env.spec.id
-                and getattr(env.unwrapped, "_frameskip", None) != 1
-            ):
-                raise ValueError(
-                    "Disable frame-skipping in the original env. Otherwise, more than one "
-                    "frame-skip will happen as through this wrapper"
-                )
+        if frame_skip > 1 and getattr(env.unwrapped, "_frameskip", None) != 1:
+            raise ValueError(
+                "Disable frame-skipping in the original env. Otherwise, more than one frame-skip will happen as through this wrapper"
+            )
         self.noop_max = noop_max
         assert env.unwrapped.get_action_meanings()[0] == "NOOP"
 
         self.frame_skip = frame_skip
         self.screen_size = screen_size
         self.terminal_on_life_loss = terminal_on_life_loss
         self.grayscale_obs = grayscale_obs
@@ -126,15 +137,17 @@
         )
 
     @property
     def ale(self):
         """Make ale as a class property to avoid serialization error."""
         return self.env.unwrapped.ale
 
-    def step(self, action):
+    def step(
+        self, action: WrapperActType
+    ) -> tuple[WrapperObsType, SupportsFloat, bool, bool, dict[str, Any]]:
         """Applies the preprocessing for an :meth:`env.step`."""
         total_reward, terminated, truncated, info = 0.0, False, False, {}
 
         for t in range(self.frame_skip):
             _, reward, terminated, truncated, info = self.env.step(action)
             total_reward += reward
             self.game_over = terminated
@@ -155,29 +168,31 @@
             elif t == self.frame_skip - 1:
                 if self.grayscale_obs:
                     self.ale.getScreenGrayscale(self.obs_buffer[0])
                 else:
                     self.ale.getScreenRGB(self.obs_buffer[0])
         return self._get_obs(), total_reward, terminated, truncated, info
 
-    def reset(self, **kwargs):
+    def reset(
+        self, *, seed: int | None = None, options: dict[str, Any] | None = None
+    ) -> tuple[WrapperObsType, dict[str, Any]]:
         """Resets the environment using preprocessing."""
         # NoopReset
-        _, reset_info = self.env.reset(**kwargs)
+        _, reset_info = self.env.reset(seed=seed, options=options)
 
         noops = (
             self.env.unwrapped.np_random.integers(1, self.noop_max + 1)
             if self.noop_max > 0
             else 0
         )
         for _ in range(noops):
             _, _, terminated, truncated, step_info = self.env.step(0)
             reset_info.update(step_info)
             if terminated or truncated:
-                _, reset_info = self.env.reset(**kwargs)
+                _, reset_info = self.env.reset(seed=seed, options=options)
 
         self.lives = self.ale.lives()
         if self.grayscale_obs:
             self.ale.getScreenGrayscale(self.obs_buffer[0])
         else:
             self.ale.getScreenRGB(self.obs_buffer[0])
         self.obs_buffer[1].fill(0)
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/jax_to_numpy.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/jax_to_numpy.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     import jax
     import jax.numpy as jnp
 except ImportError:
     raise DependencyNotInstalled(
         "Jax is not installed therefore cannot call `numpy_to_jax`, run `pip install gymnasium[jax]`"
     )
 
-__all__ = ["JaxToNumpyV0", "jax_to_numpy", "numpy_to_jax"]
+__all__ = ["JaxToNumpy", "jax_to_numpy", "numpy_to_jax"]
 
 
 @functools.singledispatch
 def numpy_to_jax(value: Any) -> Any:
     """Converts a value to a Jax Array."""
     raise Exception(
         f"No known conversion for Numpy type ({type(value)}) to Jax registered. Report as issue on github."
@@ -55,15 +55,20 @@
 
 
 @numpy_to_jax.register(abc.Iterable)
 def _iterable_numpy_to_jax(
     value: Iterable[np.ndarray | Any],
 ) -> Iterable[jax.Array | Any]:
     """Converts an Iterable from Numpy Arrays to an iterable of Jax Array."""
-    return type(value)(numpy_to_jax(v) for v in value)
+    if hasattr(value, "_make"):
+        # namedtuple - underline used to prevent potential name conflicts
+        # noinspection PyProtectedMember
+        return type(value)._make(numpy_to_jax(v) for v in value)
+    else:
+        return type(value)(numpy_to_jax(v) for v in value)
 
 
 @functools.singledispatch
 def jax_to_numpy(value: Any) -> Any:
     """Converts a value to a numpy array."""
     raise Exception(
         f"No known conversion for Jax type ({type(value)}) to NumPy registered. Report as issue on github."
@@ -85,28 +90,55 @@
 
 
 @jax_to_numpy.register(abc.Iterable)
 def _iterable_jax_to_numpy(
     value: Iterable[np.ndarray | Any],
 ) -> Iterable[jax.Array | Any]:
     """Converts an Iterable from Numpy arrays to an iterable of Jax Array."""
-    return type(value)(jax_to_numpy(v) for v in value)
+    if hasattr(value, "_make"):
+        # namedtuple - underline used to prevent potential name conflicts
+        # noinspection PyProtectedMember
+        return type(value)._make(jax_to_numpy(v) for v in value)
+    else:
+        return type(value)(jax_to_numpy(v) for v in value)
 
 
-class JaxToNumpyV0(
+class JaxToNumpy(
     gym.Wrapper[WrapperObsType, WrapperActType, ObsType, ActType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Wraps a jax environment so that it can be interacted with through numpy arrays.
+    """Wraps a Jax-based environment such that it can be interacted with NumPy arrays.
 
     Actions must be provided as numpy arrays and observations will be returned as numpy arrays.
+    A vector version of the wrapper exists, :class:`gymnasium.wrappers.vector.JaxToNumpy`.
 
     Notes:
         The Jax To Numpy and Numpy to Jax conversion does not guarantee a roundtrip (jax -> numpy -> jax) and vice versa.
         The reason for this is jax does not support non-array values, therefore numpy ``int_32(5) -> DeviceArray([5], dtype=jnp.int23)``
+
+    Example:
+        >>> import gymnasium as gym                                     # doctest: +SKIP
+        >>> env = gym.make("JaxEnv-vx")                                 # doctest: +SKIP
+        >>> env = JaxToNumpy(env)                                       # doctest: +SKIP
+        >>> obs, _ = env.reset(seed=123)                                # doctest: +SKIP
+        >>> type(obs)                                                   # doctest: +SKIP
+        <class 'numpy.ndarray'>
+        >>> action = env.action_space.sample()                          # doctest: +SKIP
+        >>> obs, reward, terminated, truncated, info = env.step(action) # doctest: +SKIP
+        >>> type(obs)                                                   # doctest: +SKIP
+        <class 'numpy.ndarray'>
+        >>> type(reward)                                                # doctest: +SKIP
+        <class 'float'>
+        >>> type(terminated)                                            # doctest: +SKIP
+        <class 'bool'>
+        >>> type(truncated)                                             # doctest: +SKIP
+        <class 'bool'>
+
+    Change logs:
+     * v1.0.0 - Initially added
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType]):
         """Wraps a jax environment such that the input and outputs are numpy arrays.
 
         Args:
             env: the jax environment to wrap
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/jax_to_torch.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/numpy_to_torch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,130 +1,137 @@
-# This wrapper will convert torch inputs for the actions and observations to Jax arrays
-# for an underlying Jax environment then convert the return observations from Jax arrays
-# back to torch tensors.
-#
-# Functionality for converting between torch and jax types originally copied from
-# https://github.com/google/brax/blob/9d6b7ced2a13da0d074b5e9fbd3aad8311e26997/brax/io/torch.py
-# Under the Apache 2.0 license. Copyright is held by the authors
-
-"""Helper functions and wrapper class for converting between PyTorch and Jax."""
+"""Helper functions and wrapper class for converting between PyTorch and NumPy."""
 from __future__ import annotations
 
 import functools
 import numbers
 from collections import abc
 from typing import Any, Iterable, Mapping, SupportsFloat, Union
 
+import numpy as np
+
 import gymnasium as gym
-from gymnasium.core import RenderFrame, WrapperActType, WrapperObsType
+from gymnasium.core import WrapperActType, WrapperObsType
 from gymnasium.error import DependencyNotInstalled
-from gymnasium.experimental.wrappers.jax_to_numpy import jax_to_numpy
 
 
 try:
-    import jax
-    import jax.numpy as jnp
-    from jax import dlpack as jax_dlpack
-except ImportError:
-    raise DependencyNotInstalled(
-        "Jax is not installed therefore cannot call `torch_to_jax`, run `pip install gymnasium[jax]`"
-    )
-
-try:
     import torch
-    from torch.utils import dlpack as torch_dlpack
 
     Device = Union[str, torch.device]
 except ImportError:
     raise DependencyNotInstalled(
-        "Torch is not installed therefore cannot call `torch_to_jax`, run `pip install torch`"
+        "Torch is not installed therefore cannot call `torch_to_numpy`, run `pip install torch`"
     )
 
 
-__all__ = ["JaxToTorchV0", "jax_to_torch", "torch_to_jax", "Device"]
+__all__ = ["NumpyToTorch", "torch_to_numpy", "numpy_to_torch"]
 
 
 @functools.singledispatch
-def torch_to_jax(value: Any) -> Any:
-    """Converts a PyTorch Tensor into a Jax Array."""
+def torch_to_numpy(value: Any) -> Any:
+    """Converts a PyTorch Tensor into a NumPy Array."""
     raise Exception(
-        f"No known conversion for Torch type ({type(value)}) to Jax registered. Report as issue on github."
+        f"No known conversion for Torch type ({type(value)}) to NumPy registered. Report as issue on github."
     )
 
 
-@torch_to_jax.register(numbers.Number)
-def _number_torch_to_jax(value: numbers.Number) -> Any:
-    """Convert a python number (int, float, complex) to a jax array."""
-    return jnp.array(value)
+@torch_to_numpy.register(numbers.Number)
+@torch_to_numpy.register(torch.Tensor)
+def _number_torch_to_numpy(value: numbers.Number | torch.Tensor) -> Any:
+    """Convert a python number (int, float, complex) and torch.Tensor to a numpy array."""
+    return np.array(value)
 
 
-@torch_to_jax.register(torch.Tensor)
-def _tensor_torch_to_jax(value: torch.Tensor) -> jax.Array:
-    """Converts a PyTorch Tensor into a Jax Array."""
-    tensor = torch_dlpack.to_dlpack(value)  # pyright: ignore[reportPrivateImportUsage]
-    tensor = jax_dlpack.from_dlpack(tensor)  # pyright: ignore[reportPrivateImportUsage]
-    return tensor
-
-
-@torch_to_jax.register(abc.Mapping)
-def _mapping_torch_to_jax(value: Mapping[str, Any]) -> Mapping[str, Any]:
+@torch_to_numpy.register(abc.Mapping)
+def _mapping_torch_to_numpy(value: Mapping[str, Any]) -> Mapping[str, Any]:
     """Converts a mapping of PyTorch Tensors into a Dictionary of Jax Array."""
-    return type(value)(**{k: torch_to_jax(v) for k, v in value.items()})
+    return type(value)(**{k: torch_to_numpy(v) for k, v in value.items()})
 
 
-@torch_to_jax.register(abc.Iterable)
-def _iterable_torch_to_jax(value: Iterable[Any]) -> Iterable[Any]:
+@torch_to_numpy.register(abc.Iterable)
+def _iterable_torch_to_numpy(value: Iterable[Any]) -> Iterable[Any]:
     """Converts an Iterable from PyTorch Tensors to an iterable of Jax Array."""
-    return type(value)(torch_to_jax(v) for v in value)
+    if hasattr(value, "_make"):
+        # namedtuple - underline used to prevent potential name conflicts
+        # noinspection PyProtectedMember
+        return type(value)._make(torch_to_numpy(v) for v in value)
+    else:
+        return type(value)(torch_to_numpy(v) for v in value)
 
 
 @functools.singledispatch
-def jax_to_torch(value: Any, device: Device | None = None) -> Any:
+def numpy_to_torch(value: Any, device: Device | None = None) -> Any:
     """Converts a Jax Array into a PyTorch Tensor."""
     raise Exception(
-        f"No known conversion for Jax type ({type(value)}) to PyTorch registered. Report as issue on github."
+        f"No known conversion for NumPy type ({type(value)}) to PyTorch registered. Report as issue on github."
     )
 
 
-@jax_to_torch.register(jax.Array)
-def _devicearray_jax_to_torch(
-    value: jax.Array, device: Device | None = None
-) -> torch.Tensor:
+@numpy_to_torch.register(numbers.Number)
+@numpy_to_torch.register(np.ndarray)
+def _numpy_to_torch(value: np.ndarray, device: Device | None = None) -> torch.Tensor:
     """Converts a Jax Array into a PyTorch Tensor."""
-    assert jax_dlpack is not None and torch_dlpack is not None
-    dlpack = jax_dlpack.to_dlpack(value)  # pyright: ignore[reportPrivateImportUsage]
-    tensor = torch_dlpack.from_dlpack(dlpack)
+    assert torch is not None
+    tensor = torch.tensor(value)
     if device:
         return tensor.to(device=device)
     return tensor
 
 
-@jax_to_torch.register(abc.Mapping)
-def _jax_mapping_to_torch(
+@numpy_to_torch.register(abc.Mapping)
+def _numpy_mapping_to_torch(
     value: Mapping[str, Any], device: Device | None = None
 ) -> Mapping[str, Any]:
     """Converts a mapping of Jax Array into a Dictionary of PyTorch Tensors."""
-    return type(value)(**{k: jax_to_torch(v, device) for k, v in value.items()})
+    return type(value)(**{k: numpy_to_torch(v, device) for k, v in value.items()})
 
 
-@jax_to_torch.register(abc.Iterable)
-def _jax_iterable_to_torch(
+@numpy_to_torch.register(abc.Iterable)
+def _numpy_iterable_to_torch(
     value: Iterable[Any], device: Device | None = None
 ) -> Iterable[Any]:
     """Converts an Iterable from Jax Array to an iterable of PyTorch Tensors."""
-    return type(value)(jax_to_torch(v, device) for v in value)
+    if hasattr(value, "_make"):
+        # namedtuple - underline used to prevent potential name conflicts
+        # noinspection PyProtectedMember
+        return type(value)._make(numpy_to_torch(v) for v in value)
+    else:
+        return type(value)(numpy_to_torch(v) for v in value)
 
 
-class JaxToTorchV0(gym.Wrapper, gym.utils.RecordConstructorArgs):
-    """Wraps a Jax-based environment so that it can be interacted with through PyTorch Tensors.
+class NumpyToTorch(gym.Wrapper, gym.utils.RecordConstructorArgs):
+    """Wraps a NumPy-based environment such that it can be interacted with PyTorch Tensors.
 
     Actions must be provided as PyTorch Tensors and observations will be returned as PyTorch Tensors.
+    A vector version of the wrapper exists, :class:`gymnasium.wrappers.vector.NumpyToTorch`.
 
     Note:
         For ``rendered`` this is returned as a NumPy array not a pytorch Tensor.
+
+    Example:
+        >>> import torch
+        >>> import gymnasium as gym
+        >>> env = gym.make("CartPole-v1")
+        >>> env = NumpyToTorch(env)
+        >>> obs, _ = env.reset(seed=123)
+        >>> type(obs)
+        <class 'torch.Tensor'>
+        >>> action = torch.tensor(env.action_space.sample())
+        >>> obs, reward, terminated, truncated, info = env.step(action)
+        >>> type(obs)
+        <class 'torch.Tensor'>
+        >>> type(reward)
+        <class 'float'>
+        >>> type(terminated)
+        <class 'bool'>
+        >>> type(truncated)
+        <class 'bool'>
+
+    Change logs:
+     * v1.0.0 - Initially added
     """
 
     def __init__(self, env: gym.Env, device: Device | None = None):
         """Wrapper class to change inputs and outputs of environment to PyTorch tensors.
 
         Args:
             env: The Jax-based environment to wrap
@@ -134,31 +141,31 @@
         gym.Wrapper.__init__(self, env)
 
         self.device: Device | None = device
 
     def step(
         self, action: WrapperActType
     ) -> tuple[WrapperObsType, SupportsFloat, bool, bool, dict]:
-        """Performs the given action within the environment.
+        """Using a PyTorch based action that is converted to NumPy to be used by the environment.
 
         Args:
-            action: The action to perform as a PyTorch Tensor
+            action: A PyTorch-based action
 
         Returns:
-            The next observation, reward, termination, truncation, and extra info
+            The PyTorch-based Tensor next observation, reward, termination, truncation, and extra info
         """
-        jax_action = torch_to_jax(action)
+        jax_action = torch_to_numpy(action)
         obs, reward, terminated, truncated, info = self.env.step(jax_action)
 
         return (
-            jax_to_torch(obs, self.device),
+            numpy_to_torch(obs, self.device),
             float(reward),
             bool(terminated),
             bool(truncated),
-            jax_to_torch(info, self.device),
+            numpy_to_torch(info, self.device),
         )
 
     def reset(
         self, *, seed: int | None = None, options: dict[str, Any] | None = None
     ) -> tuple[WrapperObsType, dict[str, Any]]:
         """Resets the environment returning PyTorch-based observation and info.
 
@@ -166,14 +173,10 @@
             seed: The seed for resetting the environment
             options: The options for resetting the environment, these are converted to jax arrays.
 
         Returns:
             PyTorch-based observations and info
         """
         if options:
-            options = torch_to_jax(options)
-
-        return jax_to_torch(self.env.reset(seed=seed, options=options), self.device)
+            options = torch_to_numpy(options)
 
-    def render(self) -> RenderFrame | list[RenderFrame] | None:
-        """Returns the rendered frames as a NumPy array."""
-        return jax_to_numpy(self.env.render())
+        return numpy_to_torch(self.env.reset(seed=seed, options=options), self.device)
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/lambda_action.py` & `gymnasium-1.0.0a1/tests/test_core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,204 @@
-"""A collection of wrappers that all use the LambdaAction class.
-
-* ``LambdaActionV0`` - Transforms the actions based on a function
-* ``ClipActionV0`` - Clips the action within a bounds
-* ``RescaleActionV0`` - Rescales the action within a minimum and maximum actions
-"""
+"""Checks that the core Gymnasium API is implemented as expected."""
 from __future__ import annotations
 
-from typing import Callable
+import re
+from typing import Any, SupportsFloat
 
 import numpy as np
+import pytest
 
 import gymnasium as gym
-from gymnasium.core import ActType, ObsType, WrapperActType
-from gymnasium.spaces import Box, Space
+from gymnasium import ActionWrapper, Env, ObservationWrapper, RewardWrapper, Wrapper
+from gymnasium.core import ActType, ObsType, WrapperActType, WrapperObsType
+from gymnasium.spaces import Box
+from gymnasium.utils import seeding
+from gymnasium.wrappers import OrderEnforcing
+from tests.testing_env import GenericTestEnv
+
+
+class ExampleEnv(Env):
+    """Example testing environment."""
+
+    def __init__(self):
+        """Constructor for example environment."""
+        self.observation_space = Box(0, 1)
+        self.action_space = Box(0, 1)
+
+    def step(
+        self, action: ActType
+    ) -> tuple[ObsType, float, bool, bool, dict[str, Any]]:
+        """Steps through the environment."""
+        return 0, 0, False, False, {}
 
+    def reset(
+        self,
+        *,
+        seed: int | None = None,
+        options: dict | None = None,
+    ) -> tuple[ObsType, dict]:
+        """Resets the environment."""
+        return 0, {}
+
+
+def test_example_env():
+    """Tests a gymnasium environment."""
+    env = ExampleEnv()
+
+    assert env.metadata == {"render_modes": []}
+    assert env.render_mode is None
+    assert env.spec is None
+    assert env._np_random is None  # pyright: ignore [reportPrivateUsage]
+
+
+class ExampleWrapper(Wrapper):
+    """An example testing wrapper."""
+
+    def __init__(self, env: Env[ObsType, ActType]):
+        """Constructor that sets the reward."""
+        super().__init__(env)
+
+        self.new_reward = 3
+
+    def reset(
+        self, *, seed: int | None = None, options: dict[str, Any] | None = None
+    ) -> tuple[WrapperObsType, dict[str, Any]]:
+        """Resets the environment ."""
+        return super().reset(seed=seed, options=options)
+
+    def step(
+        self, action: WrapperActType
+    ) -> tuple[WrapperObsType, float, bool, bool, dict[str, Any]]:
+        """Steps through the environment."""
+        obs, reward, termination, truncation, info = self.env.step(action)
+        return obs, self.new_reward, termination, truncation, info
+
+    def access_hidden_np_random(self):
+        """This should raise an error when called as wrappers should not access their own `_np_random` instances and should use the unwrapped environments."""
+        return self._np_random
+
+
+def test_example_wrapper():
+    """Tests the gymnasium wrapper works as expected."""
+    env = ExampleEnv()
+    wrapper_env = ExampleWrapper(env)
+
+    assert env.metadata == wrapper_env.metadata
+    wrapper_env.metadata = {"render_modes": ["rgb_array"]}
+    assert env.metadata != wrapper_env.metadata
+
+    assert env.render_mode == wrapper_env.render_mode
+
+    assert env.spec == wrapper_env.spec
+
+    env.observation_space = Box(0, 1)
+    env.action_space = Box(0, 1)
+    assert env.observation_space == wrapper_env.observation_space
+    assert env.action_space == wrapper_env.action_space
+    wrapper_env.observation_space = Box(1, 2)
+    wrapper_env.action_space = Box(1, 2)
+    assert env.observation_space != wrapper_env.observation_space
+    assert env.action_space != wrapper_env.action_space
+
+    wrapper_env.np_random, _ = seeding.np_random()
+    assert (
+        env._np_random  # pyright: ignore [reportPrivateUsage]
+        is env.np_random
+        is wrapper_env.np_random
+    )
+    assert 0 <= wrapper_env.np_random.uniform() <= 1
+    with pytest.raises(
+        AttributeError,
+        match=re.escape(
+            "Can't access `_np_random` of a wrapper, use `.unwrapped._np_random` or `.np_random`."
+        ),
+    ):
+        print(wrapper_env.access_hidden_np_random())
 
-__all__ = ["LambdaActionV0", "ClipActionV0", "RescaleActionV0"]
 
+class ExampleRewardWrapper(RewardWrapper):
+    """Example reward wrapper for testing."""
 
-class LambdaActionV0(
-    gym.ActionWrapper[ObsType, WrapperActType, ActType], gym.utils.RecordConstructorArgs
-):
-    """A wrapper that provides a function to modify the action passed to :meth:`step`."""
+    def reward(self, reward: SupportsFloat) -> SupportsFloat:
+        """Reward function."""
+        return 1
 
-    def __init__(
-        self,
-        env: gym.Env[ObsType, ActType],
-        func: Callable[[WrapperActType], ActType],
-        action_space: Space[WrapperActType] | None,
-    ):
-        """Initialize LambdaAction.
 
-        Args:
-            env: The environment to wrap
-            func: Function to apply to the :meth:`step`'s ``action``
-            action_space: The updated action space of the wrapper given the function.
-        """
-        gym.utils.RecordConstructorArgs.__init__(
-            self, func=func, action_space=action_space
-        )
-        gym.Wrapper.__init__(self, env)
-
-        if action_space is not None:
-            self.action_space = action_space
-
-        self.func = func
-
-    def action(self, action: WrapperActType) -> ActType:
-        """Apply function to action."""
-        return self.func(action)
-
-
-class ClipActionV0(
-    LambdaActionV0[ObsType, WrapperActType, ActType], gym.utils.RecordConstructorArgs
-):
-    """Clip the continuous action within the valid :class:`Box` observation space bound.
-
-    Example:
-        >>> import gymnasium as gym
-        >>> from gymnasium.experimental.wrappers import ClipActionV0
-        >>> import numpy as np
-        >>> env = gym.make("Hopper-v4", disable_env_checker=True)
-        >>> env = ClipActionV0(env)
-        >>> env.action_space
-        Box(-inf, inf, (3,), float32)
-        >>> _ = env.reset(seed=42)
-        >>> _ = env.step(np.array([5.0, -2.0, 0.0], dtype=np.float32))
-        ... # Executes the action np.array([1.0, -1.0, 0]) in the base environment
-    """
-
-    def __init__(self, env: gym.Env[ObsType, ActType]):
-        """A wrapper for clipping continuous actions within the valid bound.
-
-        Args:
-            env: The environment to wrap
-        """
-        assert isinstance(env.action_space, Box)
-
-        gym.utils.RecordConstructorArgs.__init__(self)
-        LambdaActionV0.__init__(
-            self,
-            env=env,
-            func=lambda action: np.clip(
-                action, env.action_space.low, env.action_space.high
-            ),
-            action_space=Box(
-                -np.inf,
-                np.inf,
-                shape=env.action_space.shape,
-                dtype=env.action_space.dtype,
-            ),
-        )
-
-
-class RescaleActionV0(
-    LambdaActionV0[ObsType, WrapperActType, ActType], gym.utils.RecordConstructorArgs
-):
-    """Affinely rescales the continuous action space of the environment to the range [min_action, max_action].
-
-    The base environment :attr:`env` must have an action space of type :class:`spaces.Box`. If :attr:`min_action`
-    or :attr:`max_action` are numpy arrays, the shape must match the shape of the environment's action space.
-
-    Example:
-        >>> import gymnasium as gym
-        >>> from gymnasium.experimental.wrappers import RescaleActionV0
-        >>> import numpy as np
-        >>> env = gym.make("Hopper-v4", disable_env_checker=True)
-        >>> _ = env.reset(seed=42)
-        >>> obs, _, _, _, _ = env.step(np.array([1, 1, 1], dtype=np.float32))
-        >>> _ = env.reset(seed=42)
-        >>> min_action = -0.5
-        >>> max_action = np.array([0.0, 0.5, 0.75], dtype=np.float32)
-        >>> wrapped_env = RescaleActionV0(env, min_action=min_action, max_action=max_action)
-        >>> wrapped_env_obs, _, _, _, _ = wrapped_env.step(max_action)
-        >>> np.alltrue(obs == wrapped_env_obs)
-        True
-    """
+class ExampleObservationWrapper(ObservationWrapper):
+    """Example observation wrapper for testing."""
 
-    def __init__(
-        self,
-        env: gym.Env[ObsType, ActType],
-        min_action: float | int | np.ndarray,
-        max_action: float | int | np.ndarray,
-    ):
-        """Constructor for the Rescale Action wrapper.
+    def observation(self, observation: ObsType) -> ObsType:
+        """Observation function."""
+        return np.array([1])
+
+
+class ExampleActionWrapper(ActionWrapper):
+    """Example action wrapper for testing."""
+
+    def action(self, action: ActType) -> ActType:
+        """Action function."""
+        return np.array([1])
+
+
+def test_reward_observation_action_wrapper():
+    """Tests the observation, action and reward wrapper examples."""
+    env = GenericTestEnv()
+
+    reward_env = ExampleRewardWrapper(env)
+    reward_env.reset()
+    _, reward, _, _, _ = reward_env.step(0)
+    assert reward == 1
+
+    observation_env = ExampleObservationWrapper(env)
+    obs, _ = observation_env.reset()
+    assert obs == np.array([1])
+    obs, _, _, _, _ = observation_env.step(0)
+    assert obs == np.array([1])
+
+    env = GenericTestEnv(step_func=lambda self, action: (action, 0, False, False, {}))
+    action_env = ExampleActionWrapper(env)
+    obs, _, _, _, _ = action_env.step(0)
+    assert obs == np.array([1])
+
+
+def test_get_set_wrapper_attr():
+    env = gym.make("CartPole-v1")
+
+    # Test get_wrapper_attr
+    with pytest.raises(AttributeError):
+        env.gravity
+    assert env.unwrapped.gravity is not None
+    assert env.get_wrapper_attr("gravity") is not None
+
+    with pytest.raises(AttributeError):
+        env.unknown_attr
+    with pytest.raises(AttributeError):
+        env.get_wrapper_attr("unknown_attr")
+
+    # Test set_wrapper_attr
+    env.set_wrapper_attr("gravity", 10.0)
+    with pytest.raises(AttributeError):
+        env.gravity
+    assert env.unwrapped.gravity == 10.0
+    assert env.get_wrapper_attr("gravity") == 10.0
+
+    env.gravity = 5.0
+    assert env.gravity == 5.0
+    assert env.get_wrapper_attr("gravity") == 5.0
+    assert env.env.get_wrapper_attr("gravity") == 10.0
+
+    # Test with OrderEnforcing (intermediate wrapper)
+    assert not isinstance(env, OrderEnforcing)
+
+    with pytest.raises(AttributeError):
+        env._disable_render_order_enforcing
+    with pytest.raises(AttributeError):
+        env.unwrapped._disable_render_order_enforcing
+    assert env.get_wrapper_attr("_disable_render_order_enforcing") is False
+
+    env.set_wrapper_attr("_disable_render_order_enforcing", True)
 
-        Args:
-            env (Env): The environment to wrap
-            min_action (float, int or np.ndarray): The min values for each action. This may be a numpy array or a scalar.
-            max_action (float, int or np.ndarray): The max values for each action. This may be a numpy array or a scalar.
-        """
-        gym.utils.RecordConstructorArgs.__init__(
-            self, min_action=min_action, max_action=max_action
-        )
-
-        assert isinstance(env.action_space, Box)
-        assert not np.any(env.action_space.low == np.inf) and not np.any(
-            env.action_space.high == np.inf
-        )
-
-        if not isinstance(min_action, np.ndarray):
-            assert np.issubdtype(type(min_action), np.integer) or np.issubdtype(
-                type(min_action), np.floating
-            )
-            min_action = np.full(env.action_space.shape, min_action)
-
-        assert min_action.shape == env.action_space.shape
-        assert not np.any(min_action == np.inf)
-
-        if not isinstance(max_action, np.ndarray):
-            assert np.issubdtype(type(max_action), np.integer) or np.issubdtype(
-                type(max_action), np.floating
-            )
-            max_action = np.full(env.action_space.shape, max_action)
-        assert max_action.shape == env.action_space.shape
-        assert not np.any(max_action == np.inf)
-
-        assert isinstance(env.action_space, Box)
-        assert np.all(np.less_equal(min_action, max_action))
-
-        # Imagine the x-axis between the old Box and the y-axis being the new Box
-        gradient = (env.action_space.high - env.action_space.low) / (
-            max_action - min_action
-        )
-        intercept = gradient * -min_action + env.action_space.low
-
-        LambdaActionV0.__init__(
-            self,
-            env=env,
-            func=lambda action: gradient * action + intercept,
-            action_space=Box(
-                low=min_action,
-                high=max_action,
-                shape=env.action_space.shape,
-                dtype=env.action_space.dtype,
-            ),
-        )
+    with pytest.raises(AttributeError):
+        env._disable_render_order_enforcing
+    with pytest.raises(AttributeError):
+        env.unwrapped._disable_render_order_enforcing
+    assert env.get_wrapper_attr("_disable_render_order_enforcing") is True
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/lambda_observation.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/transform_observation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,80 @@
 """A collection of observation wrappers using a lambda function.
 
-* ``LambdaObservationV0`` - Transforms the observation with a function
-* ``FilterObservationV0`` - Filters a ``Tuple`` or ``Dict`` to only include certain keys
-* ``FlattenObservationV0`` - Flattens the observations
-* ``GrayscaleObservationV0`` - Converts a RGB observation to a grayscale observation
-* ``ResizeObservationV0`` - Resizes an array-based observation (normally a RGB observation)
-* ``ReshapeObservationV0`` - Reshapes an array-based observation
-* ``RescaleObservationV0`` - Rescales an observation to between a minimum and maximum value
-* ``DtypeObservationV0`` - Convert an observation to a dtype
-* ``PixelObservationV0`` - Allows the observation to the rendered frame
+* ``TransformObservation`` - Transforms the observation with a function
+* ``FilterObservation`` - Filters a ``Tuple`` or ``Dict`` to only include certain keys
+* ``FlattenObservation`` - Flattens the observations
+* ``GrayscaleObservation`` - Converts a RGB observation to a grayscale observation
+* ``ResizeObservation`` - Resizes an array-based observation (normally a RGB observation)
+* ``ReshapeObservation`` - Reshapes an array-based observation
+* ``RescaleObservation`` - Rescales an observation to between a minimum and maximum value
+* ``DtypeObservation`` - Convert an observation to a dtype
+* ``RenderObservation`` - Allows the observation to the rendered frame
 """
 from __future__ import annotations
 
 from typing import Any, Callable, Final, Sequence
 
 import numpy as np
 
 import gymnasium as gym
 from gymnasium import spaces
 from gymnasium.core import ActType, ObsType, WrapperObsType
 from gymnasium.error import DependencyNotInstalled
 
 
 __all__ = [
-    "LambdaObservationV0",
-    "FilterObservationV0",
-    "FlattenObservationV0",
-    "GrayscaleObservationV0",
-    "ResizeObservationV0",
-    "ReshapeObservationV0",
-    "RescaleObservationV0",
-    "DtypeObservationV0",
-    "PixelObservationV0",
+    "TransformObservation",
+    "FilterObservation",
+    "FlattenObservation",
+    "GrayscaleObservation",
+    "ResizeObservation",
+    "ReshapeObservation",
+    "RescaleObservation",
+    "DtypeObservation",
+    "AddRenderObservation",
 ]
 
 
-class LambdaObservationV0(
+class TransformObservation(
     gym.ObservationWrapper[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Transforms an observation via a function provided to the wrapper.
+    """Applies a function to the ``observation`` received from the environment's :meth:`Env.reset` and :meth:`Env.step` that is passed back to the user.
 
     The function :attr:`func` will be applied to all observations.
-    If the observations from :attr:`func` are outside the bounds of the ``env``'s observation space, provide an :attr:`observation_space`.
+    If the observations from :attr:`func` are outside the bounds of the ``env``'s observation space, provide an updated :attr:`observation_space`.
+
+    A vector version of the wrapper exists :class:`gymnasium.wrappers.vector.TransformObservation`.
 
     Example:
         >>> import gymnasium as gym
-        >>> from gymnasium.experimental.wrappers import LambdaObservationV0
+        >>> from gymnasium.wrappers import TransformObservation
         >>> import numpy as np
         >>> np.random.seed(0)
         >>> env = gym.make("CartPole-v1")
-        >>> env = LambdaObservationV0(env, lambda obs: obs + 0.1 * np.random.random(obs.shape), env.observation_space)
+        >>> env.reset(seed=42)
+        (array([ 0.0273956 , -0.00611216,  0.03585979,  0.0197368 ], dtype=float32), {})
+        >>> env = gym.make("CartPole-v1")
+        >>> env = TransformObservation(env, lambda obs: obs + 0.1 * np.random.random(obs.shape), env.observation_space)
         >>> env.reset(seed=42)
         (array([0.08227695, 0.06540678, 0.09613613, 0.07422512]), {})
+
+    Change logs:
+     * v0.15.4 - Initially added
+     * v1.0.0 - Add requirement of ``observation_space``
     """
 
     def __init__(
         self,
         env: gym.Env[ObsType, ActType],
         func: Callable[[ObsType], Any],
         observation_space: gym.Space[WrapperObsType] | None,
     ):
-        """Constructor for the lambda observation wrapper.
+        """Constructor for the transform observation wrapper.
 
         Args:
             env: The environment to wrap
             func: A function that will transform an observation. If this transformed observation is outside the observation space of ``env.observation_space`` then provide an `observation_space`.
             observation_space: The observation spaces of the wrapper, if None, then it is assumed the same as ``env.observation_space``.
         """
         gym.utils.RecordConstructorArgs.__init__(
@@ -79,46 +88,55 @@
         self.func = func
 
     def observation(self, observation: ObsType) -> Any:
         """Apply function to the observation."""
         return self.func(observation)
 
 
-class FilterObservationV0(
-    LambdaObservationV0[WrapperObsType, ActType, ObsType],
+class FilterObservation(
+    TransformObservation[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Filters Dict or Tuple observation space by the keys or indexes.
+    """Filters a Dict or Tuple observation spaces by a set of keys or indexes.
+
+    A vector version of the wrapper exists :class:`gymnasium.wrappers.vector.FilterObservation`.
 
     Example:
         >>> import gymnasium as gym
-        >>> from gymnasium.wrappers import TransformObservation
-        >>> from gymnasium.experimental.wrappers import FilterObservationV0
+        >>> from gymnasium.wrappers import FilterObservation
         >>> env = gym.make("CartPole-v1")
-        >>> env = gym.wrappers.TransformObservation(env, lambda obs: {'obs': obs, 'time': 0})
-        >>> env.observation_space = gym.spaces.Dict(obs=env.observation_space, time=gym.spaces.Discrete(1))
+        >>> env = gym.wrappers.TimeAwareObservation(env, flatten=False)
+        >>> env.observation_space
+        Dict('obs': Box([-4.8000002e+00 -3.4028235e+38 -4.1887903e-01 -3.4028235e+38], [4.8000002e+00 3.4028235e+38 4.1887903e-01 3.4028235e+38], (4,), float32), 'time': Box(0, 500, (1,), int32))
         >>> env.reset(seed=42)
-        ({'obs': array([ 0.0273956 , -0.00611216,  0.03585979,  0.0197368 ], dtype=float32), 'time': 0}, {})
-        >>> env = FilterObservationV0(env, filter_keys=['time'])
+        ({'obs': array([ 0.0273956 , -0.00611216,  0.03585979,  0.0197368 ], dtype=float32), 'time': array([0], dtype=int32)}, {})
+        >>> env = FilterObservation(env, filter_keys=['time'])
         >>> env.reset(seed=42)
-        ({'time': 0}, {})
+        ({'time': array([0], dtype=int32)}, {})
         >>> env.step(0)
-        ({'time': 0}, 1.0, False, False, {})
+        ({'time': array([1], dtype=int32)}, 1.0, False, False, {})
+
+    Change logs:
+     * v0.12.3 - Initially added, originally called `FilterObservationWrapper`
+     * v1.0.0 - Rename to `FilterObservation` and add support for tuple observation spaces with integer ``filter_keys``
     """
 
     def __init__(
         self, env: gym.Env[ObsType, ActType], filter_keys: Sequence[str | int]
     ):
         """Constructor for the filter observation wrapper.
 
         Args:
             env: The environment to wrap
-            filter_keys: The subspaces to be included, use a list of strings or integers for ``Dict`` and ``Tuple`` spaces respectivesly
+            filter_keys: The set of subspaces to be *included*, use a list of strings for ``Dict`` and integers for ``Tuple`` spaces
         """
-        assert isinstance(filter_keys, Sequence)
+        if not isinstance(filter_keys, Sequence):
+            raise TypeError(
+                f"Expects `filter_keys` to be a Sequence, actual type: {type(filter_keys)}"
+            )
         gym.utils.RecordConstructorArgs.__init__(self, filter_keys=filter_keys)
 
         # Filters for dictionary space
         if isinstance(env.observation_space, spaces.Dict):
             assert all(isinstance(key, str) for key in filter_keys)
 
             if any(
@@ -137,18 +155,18 @@
                 )
 
             new_observation_space = spaces.Dict(
                 {key: env.observation_space[key] for key in filter_keys}
             )
             if len(new_observation_space) == 0:
                 raise ValueError(
-                    "The observation space is empty due to filtering all keys."
+                    "The observation space is empty due to filtering all of the keys."
                 )
 
-            LambdaObservationV0.__init__(
+            TransformObservation.__init__(
                 self,
                 env=env,
                 func=lambda obs: {key: obs[key] for key in filter_keys},
                 observation_space=new_observation_space,
             )
             # Filter for tuple observation
         elif isinstance(env.observation_space, spaces.Tuple):
@@ -175,83 +193,94 @@
                 env.observation_space[key] for key in filter_keys
             )
             if len(new_observation_spaces) == 0:
                 raise ValueError(
                     "The observation space is empty due to filtering all keys."
                 )
 
-            LambdaObservationV0.__init__(
+            TransformObservation.__init__(
                 self,
                 env=env,
                 func=lambda obs: tuple(obs[key] for key in filter_keys),
                 observation_space=new_observation_spaces,
             )
         else:
             raise ValueError(
                 f"FilterObservation wrapper is only usable with `Dict` and `Tuple` observations, actual type: {type(env.observation_space)}"
             )
 
         self.filter_keys: Final[Sequence[str | int]] = filter_keys
 
 
-class FlattenObservationV0(
-    LambdaObservationV0[WrapperObsType, ActType, ObsType],
+class FlattenObservation(
+    TransformObservation[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Observation wrapper that flattens the observation.
+    """Flattens the environment's observation space and each observation from ``reset`` and ``step`` functions.
+
+    A vector version of the wrapper exists :class:`gymnasium.wrappers.vector.FlattenObservation`.
 
     Example:
         >>> import gymnasium as gym
-        >>> from gymnasium.experimental.wrappers import FlattenObservationV0
+        >>> from gymnasium.wrappers import FlattenObservation
         >>> env = gym.make("CarRacing-v2")
         >>> env.observation_space.shape
         (96, 96, 3)
-        >>> env = FlattenObservationV0(env)
+        >>> env = FlattenObservation(env)
         >>> env.observation_space.shape
         (27648,)
         >>> obs, _ = env.reset()
         >>> obs.shape
         (27648,)
+
+    Change logs:
+     * v0.15.0 - Initially added
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType]):
         """Constructor for any environment's observation space that implements ``spaces.utils.flatten_space`` and ``spaces.utils.flatten``.
 
         Args:
             env:  The environment to wrap
         """
         gym.utils.RecordConstructorArgs.__init__(self)
-        LambdaObservationV0.__init__(
+        TransformObservation.__init__(
             self,
             env=env,
             func=lambda obs: spaces.utils.flatten(env.observation_space, obs),
             observation_space=spaces.utils.flatten_space(env.observation_space),
         )
 
 
-class GrayscaleObservationV0(
-    LambdaObservationV0[WrapperObsType, ActType, ObsType],
+class GrayscaleObservation(
+    TransformObservation[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Observation wrapper that converts an RGB image to grayscale.
+    """Converts an image observation computed by ``reset`` and ``step`` from RGB to Grayscale.
 
-    The :attr:`keep_dim` will keep the channel dimension
+    The :attr:`keep_dim` will keep the channel dimension.
+
+    A vector version of the wrapper exists :class:`gymnasium.wrappers.vector.GrayscaleObservation`.
 
     Example:
         >>> import gymnasium as gym
-        >>> from gymnasium.experimental.wrappers import GrayscaleObservationV0
+        >>> from gymnasium.wrappers import GrayscaleObservation
         >>> env = gym.make("CarRacing-v2")
         >>> env.observation_space.shape
         (96, 96, 3)
-        >>> grayscale_env = GrayscaleObservationV0(env)
+        >>> grayscale_env = GrayscaleObservation(env)
         >>> grayscale_env.observation_space.shape
         (96, 96)
-        >>> grayscale_env = GrayscaleObservationV0(env, keep_dim=True)
+        >>> grayscale_env = GrayscaleObservation(env, keep_dim=True)
         >>> grayscale_env.observation_space.shape
         (96, 96, 1)
+
+    Change logs:
+     * v0.15.0 - Initially added, originally called ``GrayScaleObservation``
+     * v1.0.0 - Renamed to ``GrayscaleObservation``
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType], keep_dim: bool = False):
         """Constructor for an RGB image based environments to make the image grayscale.
 
         Args:
             env: The environment to wrap
@@ -273,162 +302,183 @@
         if keep_dim:
             new_observation_space = spaces.Box(
                 low=0,
                 high=255,
                 shape=env.observation_space.shape[:2] + (1,),
                 dtype=np.uint8,
             )
-            LambdaObservationV0.__init__(
+            TransformObservation.__init__(
                 self,
                 env=env,
                 func=lambda obs: np.expand_dims(
                     np.sum(
                         np.multiply(obs, np.array([0.2125, 0.7154, 0.0721])), axis=-1
                     ).astype(np.uint8),
                     axis=-1,
                 ),
                 observation_space=new_observation_space,
             )
         else:
             new_observation_space = spaces.Box(
                 low=0, high=255, shape=env.observation_space.shape[:2], dtype=np.uint8
             )
-            LambdaObservationV0.__init__(
+            TransformObservation.__init__(
                 self,
                 env=env,
                 func=lambda obs: np.sum(
                     np.multiply(obs, np.array([0.2125, 0.7154, 0.0721])), axis=-1
                 ).astype(np.uint8),
                 observation_space=new_observation_space,
             )
 
 
-class ResizeObservationV0(
-    LambdaObservationV0[WrapperObsType, ActType, ObsType],
+class ResizeObservation(
+    TransformObservation[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Resizes image observations using OpenCV to shape.
+    """Resizes image observations using OpenCV to a specified shape.
+
+    A vector version of the wrapper exists :class:`gymnasium.wrappers.vector.ResizeObservation`.
 
     Example:
         >>> import gymnasium as gym
-        >>> from gymnasium.experimental.wrappers import ResizeObservationV0
+        >>> from gymnasium.wrappers import ResizeObservation
         >>> env = gym.make("CarRacing-v2")
         >>> env.observation_space.shape
         (96, 96, 3)
-        >>> resized_env = ResizeObservationV0(env, (32, 32))
+        >>> resized_env = ResizeObservation(env, (32, 32))
         >>> resized_env.observation_space.shape
         (32, 32, 3)
+
+    Change logs:
+     * v0.12.6 - Initially added
+     * v1.0.0 - Requires ``shape`` with a tuple of two integers
     """
 
-    def __init__(self, env: gym.Env[ObsType, ActType], shape: tuple[int, ...]):
+    def __init__(self, env: gym.Env[ObsType, ActType], shape: tuple[int, int]):
         """Constructor that requires an image environment observation space with a shape.
 
         Args:
             env: The environment to wrap
             shape: The resized observation shape
         """
         assert isinstance(env.observation_space, spaces.Box)
-        assert len(env.observation_space.shape) in [2, 3]
+        assert len(env.observation_space.shape) in {2, 3}
         assert np.all(env.observation_space.low == 0) and np.all(
             env.observation_space.high == 255
         )
         assert env.observation_space.dtype == np.uint8
 
         assert isinstance(shape, tuple)
+        assert len(shape) == 2
         assert all(np.issubdtype(type(elem), np.integer) for elem in shape)
         assert all(x > 0 for x in shape)
 
         try:
             import cv2
         except ImportError as e:
             raise DependencyNotInstalled(
                 "opencv (cv2) is not installed, run `pip install gymnasium[other]`"
             ) from e
 
-        self.shape: Final[tuple[int, ...]] = tuple(shape)
+        self.shape: Final[tuple[int, int]] = tuple(shape)
+        # for some reason, cv2.resize will return the shape in reverse, todo confirm implementation
+        self.cv2_shape: Final[tuple[int, int]] = (shape[1], shape[0])
 
         new_observation_space = spaces.Box(
             low=0,
             high=255,
             shape=self.shape + env.observation_space.shape[2:],
             dtype=np.uint8,
         )
 
         gym.utils.RecordConstructorArgs.__init__(self, shape=shape)
-        LambdaObservationV0.__init__(
+        TransformObservation.__init__(
             self,
             env=env,
-            func=lambda obs: cv2.resize(obs, self.shape, interpolation=cv2.INTER_AREA),
+            func=lambda obs: cv2.resize(
+                obs, self.cv2_shape, interpolation=cv2.INTER_AREA
+            ),
             observation_space=new_observation_space,
         )
 
 
-class ReshapeObservationV0(
-    LambdaObservationV0[WrapperObsType, ActType, ObsType],
+class ReshapeObservation(
+    TransformObservation[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Reshapes array based observations to shapes.
+    """Reshapes Array based observations to a specified shape.
+
+    A vector version of the wrapper exists :class:`gymnasium.wrappers.vector.RescaleObservation`.
 
     Example:
         >>> import gymnasium as gym
-        >>> from gymnasium.experimental.wrappers import ReshapeObservationV0
+        >>> from gymnasium.wrappers import ReshapeObservation
         >>> env = gym.make("CarRacing-v2")
         >>> env.observation_space.shape
         (96, 96, 3)
-        >>> reshape_env = ReshapeObservationV0(env, (24, 4, 96, 1, 3))
+        >>> reshape_env = ReshapeObservation(env, (24, 4, 96, 1, 3))
         >>> reshape_env.observation_space.shape
         (24, 4, 96, 1, 3)
+
+    Change logs:
+     * v1.0.0 - Initially added
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType], shape: int | tuple[int, ...]):
         """Constructor for env with ``Box`` observation space that has a shape product equal to the new shape product.
 
         Args:
             env: The environment to wrap
             shape: The reshaped observation space
         """
         assert isinstance(env.observation_space, spaces.Box)
-        assert np.product(shape) == np.product(env.observation_space.shape)
+        assert np.prod(shape) == np.prod(env.observation_space.shape)
 
         assert isinstance(shape, tuple)
         assert all(np.issubdtype(type(elem), np.integer) for elem in shape)
         assert all(x > 0 or x == -1 for x in shape)
 
         new_observation_space = spaces.Box(
             low=np.reshape(np.ravel(env.observation_space.low), shape),
             high=np.reshape(np.ravel(env.observation_space.high), shape),
             shape=shape,
             dtype=env.observation_space.dtype,
         )
         self.shape = shape
 
         gym.utils.RecordConstructorArgs.__init__(self, shape=shape)
-        LambdaObservationV0.__init__(
+        TransformObservation.__init__(
             self,
             env=env,
             func=lambda obs: np.reshape(obs, shape),
             observation_space=new_observation_space,
         )
 
 
-class RescaleObservationV0(
-    LambdaObservationV0[WrapperObsType, ActType, ObsType],
+class RescaleObservation(
+    TransformObservation[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Linearly rescales observation to between a minimum and maximum value.
+    """Affinely (linearly) rescales a ``Box`` observation space of the environment to within the range of ``[min_obs, max_obs]``.
+
+    A vector version of the wrapper exists :class:`gymnasium.wrappers.vector.RescaleObservation`.
 
     Example:
         >>> import gymnasium as gym
-        >>> from gymnasium.experimental.wrappers import RescaleObservationV0
+        >>> from gymnasium.wrappers import RescaleObservation
         >>> env = gym.make("Pendulum-v1")
         >>> env.observation_space
         Box([-1. -1. -8.], [1. 1. 8.], (3,), float32)
-        >>> env = RescaleObservationV0(env, np.array([-2, -1, -10], dtype=np.float32), np.array([1, 0, 1], dtype=np.float32))
+        >>> env = RescaleObservation(env, np.array([-2, -1, -10], dtype=np.float32), np.array([1, 0, 1], dtype=np.float32))
         >>> env.observation_space
         Box([ -2.  -1. -10.], [1. 0. 1.], (3,), float32)
+
+    Change logs:
+     * v1.0.0 - Initially added
     """
 
     def __init__(
         self,
         env: gym.Env[ObsType, ActType],
         min_obs: np.floating | np.integer | np.ndarray,
         max_obs: np.floating | np.integer | np.ndarray,
@@ -463,41 +513,50 @@
         assert max_obs.shape == env.observation_space.shape
         assert not np.any(max_obs == np.inf)
 
         self.min_obs = min_obs
         self.max_obs = max_obs
 
         # Imagine the x-axis between the old Box and the y-axis being the new Box
-        gradient = (max_obs - min_obs) / (
-            env.observation_space.high - env.observation_space.low
+        high_low_diff = np.array(
+            env.observation_space.high, dtype=np.float128
+        ) - np.array(env.observation_space.low, dtype=np.float128)
+        gradient = np.array(
+            (max_obs - min_obs) / high_low_diff, dtype=env.observation_space.dtype
         )
+
         intercept = gradient * -env.observation_space.low + min_obs
 
         gym.utils.RecordConstructorArgs.__init__(self, min_obs=min_obs, max_obs=max_obs)
-        LambdaObservationV0.__init__(
+        TransformObservation.__init__(
             self,
             env=env,
             func=lambda obs: gradient * obs + intercept,
             observation_space=spaces.Box(
                 low=min_obs,
                 high=max_obs,
                 shape=env.observation_space.shape,
                 dtype=env.observation_space.dtype,
             ),
         )
 
 
-class DtypeObservationV0(
-    LambdaObservationV0[WrapperObsType, ActType, ObsType],
+class DtypeObservation(
+    TransformObservation[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Observation wrapper for transforming the dtype of an observation.
+    """Modifies the dtype of an observation array to a specified dtype.
 
     Note:
         This is only compatible with :class:`Box`, :class:`Discrete`, :class:`MultiDiscrete` and :class:`MultiBinary` observation spaces
+
+    A vector version of the wrapper exists :class:`gymnasium.wrappers.vector.DtypeObservation`.
+
+    Change logs:
+     * v1.0.0 - Initially added
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType], dtype: Any):
         """Constructor for Dtype observation wrapper.
 
         Args:
             env: The environment to wrap
@@ -536,85 +595,121 @@
             )
         else:
             raise TypeError(
                 "DtypeObservation is only compatible with value / array-based observations."
             )
 
         gym.utils.RecordConstructorArgs.__init__(self, dtype=dtype)
-        LambdaObservationV0.__init__(
+        TransformObservation.__init__(
             self,
             env=env,
             func=lambda obs: dtype(obs),
             observation_space=new_observation_space,
         )
 
 
-class PixelObservationV0(
-    LambdaObservationV0[WrapperObsType, ActType, ObsType],
+class AddRenderObservation(
+    TransformObservation[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Includes the rendered observations to the environment's observations.
+    """Includes the rendered observations in the environment's observations.
+
+    Notes:
+       This was previously called ``PixelObservationWrapper``.
+
+    No vector version of the wrapper exists.
 
-    Observations of this wrapper will be dictionaries of images.
-    You can also choose to add the observation of the base environment to this dictionary.
-    In that case, if the base environment has an observation space of type :class:`Dict`, the dictionary
-    of rendered images will be updated with the base environment's observation. If, however, the observation
-    space is of type :class:`Box`, the base environment's observation (which will be an element of the :class:`Box`
-    space) will be added to the dictionary under the key "state".
+    Example - Replace the observation with the rendered image:
+        >>> env = gym.make("CartPole-v1", render_mode="rgb_array")
+        >>> env = AddRenderObservation(env, render_only=True)
+        >>> env.observation_space
+        Box(0, 255, (400, 600, 3), uint8)
+        >>> obs, _ = env.reset(seed=123)
+        >>> image = env.render()
+        >>> np.all(obs == image)
+        True
+        >>> obs, *_ = env.step(env.action_space.sample())
+        >>> image = env.render()
+        >>> np.all(obs == image)
+        True
+
+    Example - Add the rendered image to the original observation as a dictionary item:
+        >>> env = gym.make("CartPole-v1", render_mode="rgb_array")
+        >>> env = AddRenderObservation(env, render_only=False)
+        >>> env.observation_space
+        Dict('pixels': Box(0, 255, (400, 600, 3), uint8), 'state': Box([-4.8000002e+00 -3.4028235e+38 -4.1887903e-01 -3.4028235e+38], [4.8000002e+00 3.4028235e+38 4.1887903e-01 3.4028235e+38], (4,), float32))
+        >>> obs, info = env.reset(seed=123)
+        >>> obs.keys()
+        dict_keys(['state', 'pixels'])
+        >>> obs["state"]
+        array([ 0.01823519, -0.0446179 , -0.02796401, -0.03156282], dtype=float32)
+        >>> np.all(obs["pixels"] == env.render())
+        True
+        >>> obs, reward, terminates, truncates, info = env.step(env.action_space.sample())
+        >>> image = env.render()
+        >>> np.all(obs["pixels"] == image)
+        True
+
+    Change logs:
+     * v0.15.0 - Initially added as ``PixelObservationWrapper``
+     * v1.0.0 - Renamed to ``AddRenderObservation``
     """
 
     def __init__(
         self,
         env: gym.Env[ObsType, ActType],
-        pixels_only: bool = True,
-        pixels_key: str = "pixels",
+        render_only: bool = True,
+        render_key: str = "pixels",
         obs_key: str = "state",
     ):
-        """Constructor of the pixel observation wrapper.
+        """Constructor of the add render observation wrapper.
 
         Args:
             env: The environment to wrap.
-            pixels_only (bool): If ``True`` (default), the original observation returned
+            render_only (bool): If ``True`` (default), the original observation returned
                 by the wrapped environment will be discarded, and a dictionary
                 observation will only include pixels. If ``False``, the
                 observation dictionary will contain both the original
                 observations and the pixel observations.
-            pixels_key: Optional custom string specifying the pixel key. Defaults to "pixels"
+            render_key: Optional custom string specifying the pixel key. Defaults to "pixels"
             obs_key: Optional custom string specifying the obs key. Defaults to "state"
         """
         gym.utils.RecordConstructorArgs.__init__(
-            self, pixels_only=pixels_only, pixels_key=pixels_key, obs_key=obs_key
+            self,
+            pixels_only=render_only,
+            pixels_key=render_key,
+            obs_key=obs_key,
         )
 
         assert env.render_mode is not None and env.render_mode != "human"
         env.reset()
         pixels = env.render()
         assert pixels is not None and isinstance(pixels, np.ndarray)
         pixel_space = spaces.Box(low=0, high=255, shape=pixels.shape, dtype=np.uint8)
 
-        if pixels_only:
+        if render_only:
             obs_space = pixel_space
-            LambdaObservationV0.__init__(
+            TransformObservation.__init__(
                 self, env=env, func=lambda _: self.render(), observation_space=obs_space
             )
         elif isinstance(env.observation_space, spaces.Dict):
-            assert pixels_key not in env.observation_space.spaces.keys()
+            assert render_key not in env.observation_space.spaces.keys()
 
             obs_space = spaces.Dict(
-                {pixels_key: pixel_space, **env.observation_space.spaces}
+                {render_key: pixel_space, **env.observation_space.spaces}
             )
-            LambdaObservationV0.__init__(
+            TransformObservation.__init__(
                 self,
                 env=env,
-                func=lambda obs: {pixels_key: self.render(), **obs_space},
+                func=lambda obs: {render_key: self.render(), **obs},
                 observation_space=obs_space,
             )
         else:
             obs_space = spaces.Dict(
-                {obs_key: env.observation_space, pixels_key: pixel_space}
+                {obs_key: env.observation_space, render_key: pixel_space}
             )
-            LambdaObservationV0.__init__(
+            TransformObservation.__init__(
                 self,
                 env=env,
-                func=lambda obs: {obs_key: obs, pixels_key: self.render()},
+                func=lambda obs: {obs_key: obs, render_key: self.render()},
                 observation_space=obs_space,
             )
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/lambda_reward.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/vector/vectorize_reward.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,127 @@
-"""A collection of wrappers for modifying the reward.
-
-* ``LambdaRewardV0`` - Transforms the reward by a function
-* ``ClipRewardV0`` - Clips the reward between a minimum and maximum value
-"""
+"""Vectorizes reward function to work with `VectorEnv`."""
 from __future__ import annotations
 
-from typing import Callable, SupportsFloat
+from typing import Any, Callable
 
 import numpy as np
 
-import gymnasium as gym
-from gymnasium.core import ActType, ObsType
-from gymnasium.error import InvalidBound
-
-
-__all__ = ["LambdaRewardV0", "ClipRewardV0"]
+from gymnasium import Env
+from gymnasium.vector import VectorEnv, VectorRewardWrapper
+from gymnasium.vector.vector_env import ArrayType
+from gymnasium.wrappers import transform_reward
 
 
-class LambdaRewardV0(
-    gym.RewardWrapper[ObsType, ActType], gym.utils.RecordConstructorArgs
-):
+class TransformReward(VectorRewardWrapper):
     """A reward wrapper that allows a custom function to modify the step reward.
 
-    Example:
+    Example with reward transformation:
         >>> import gymnasium as gym
-        >>> from gymnasium.experimental.wrappers import LambdaRewardV0
-        >>> env = gym.make("CartPole-v1")
-        >>> env = LambdaRewardV0(env, lambda r: 2 * r + 1)
-        >>> _ = env.reset()
-        >>> _, rew, _, _, _ = env.step(0)
-        >>> rew
-        3.0
+        >>> from gymnasium.spaces import Box
+        >>> def scale_and_shift(rew):
+        ...     return (rew - 1.0) * 2.0
+        ...
+        >>> envs = gym.make_vec("MountainCarContinuous-v0", num_envs=3)
+        >>> envs = TransformReward(env=envs, func=scale_and_shift)
+        >>> _ = envs.action_space.seed(123)
+        >>> obs, info = envs.reset(seed=123)
+        >>> obs, rew, term, trunc, info = envs.step(envs.action_space.sample())
+        >>> envs.close()
+        >>> obs
+        array([[-4.6343064e-01,  9.8971417e-05],
+               [-4.4488689e-01, -1.9375233e-03],
+               [-4.3118435e-01, -1.5342437e-03]], dtype=float32)
     """
 
-    def __init__(
-        self,
-        env: gym.Env[ObsType, ActType],
-        func: Callable[[SupportsFloat], SupportsFloat],
-    ):
-        """Initialize LambdaRewardV0 wrapper.
+    def __init__(self, env: VectorEnv, func: Callable[[ArrayType], ArrayType]):
+        """Initialize LambdaReward wrapper.
 
         Args:
-            env (Env): The environment to wrap
+            env (Env): The vector environment to wrap
             func: (Callable): The function to apply to reward
         """
-        gym.utils.RecordConstructorArgs.__init__(self, func=func)
-        gym.RewardWrapper.__init__(self, env)
+        super().__init__(env)
 
         self.func = func
 
-    def reward(self, reward: SupportsFloat) -> SupportsFloat:
-        """Apply function to reward.
+    def rewards(self, reward: ArrayType) -> ArrayType:
+        """Apply function to reward."""
+        return self.func(reward)
+
+
+class VectorizeTransformReward(VectorRewardWrapper):
+    """Vectorizes a single-agent transform reward wrapper for vector environments.
+
+    An example such that applies a ReLU to the reward:
+        >>> import gymnasium as gym
+        >>> from gymnasium.wrappers import TransformReward
+        >>> envs = gym.make_vec("MountainCarContinuous-v0", num_envs=3)
+        >>> envs = VectorizeTransformReward(envs, wrapper=TransformReward, func=lambda x: (x > 0.0) * x)
+        >>> _ = envs.action_space.seed(123)
+        >>> obs, info = envs.reset(seed=123)
+        >>> obs, rew, term, trunc, info = envs.step(envs.action_space.sample())
+        >>> envs.close()
+        >>> rew
+        array([-0., -0., -0.])
+    """
+
+    def __init__(
+        self,
+        env: VectorEnv,
+        wrapper: type[transform_reward.TransformReward],
+        **kwargs: Any,
+    ):
+        """Constructor for the vectorized lambda reward wrapper.
 
         Args:
-            reward (Union[float, int, np.ndarray]): environment's reward
+            env: The vector environment to wrap.
+            wrapper: The wrapper to vectorize
+            **kwargs: Keyword argument for the wrapper
         """
-        return self.func(reward)
+        super().__init__(env)
+
+        self.wrapper = wrapper(Env(), **kwargs)
+
+    def rewards(self, reward: ArrayType) -> ArrayType:
+        """Iterates over the reward updating each with the wrapper func."""
+        for i, r in enumerate(reward):
+            reward[i] = self.wrapper.func(r)
+        return reward
 
 
-class ClipRewardV0(LambdaRewardV0[ObsType, ActType], gym.utils.RecordConstructorArgs):
+class ClipReward(VectorizeTransformReward):
     """A wrapper that clips the rewards for an environment between an upper and lower bound.
 
-    Example:
+    Example with clipped rewards:
+        >>> import numpy as np
         >>> import gymnasium as gym
-        >>> from gymnasium.experimental.wrappers import ClipRewardV0
-        >>> env = gym.make("CartPole-v1")
-        >>> env = ClipRewardV0(env, 0, 0.5)
-        >>> _ = env.reset()
-        >>> _, rew, _, _, _ = env.step(1)
+        >>> envs = gym.make_vec("MountainCarContinuous-v0", num_envs=3)
+        >>> envs = ClipReward(envs, 0.0, 2.0)
+        >>> _ = envs.action_space.seed(123)
+        >>> obs, info = envs.reset(seed=123)
+        >>> for _ in range(10):
+        ...     obs, rew, term, trunc, info = envs.step(0.5 * np.ones((3, 1)))
+        ...
+        >>> envs.close()
         >>> rew
-        0.5
+        array([0., 0., 0.])
     """
 
     def __init__(
         self,
-        env: gym.Env[ObsType, ActType],
+        env: VectorEnv,
         min_reward: float | np.ndarray | None = None,
         max_reward: float | np.ndarray | None = None,
     ):
-        """Initialize ClipRewardsV0 wrapper.
+        """Constructor for ClipReward wrapper.
 
         Args:
-            env (Env): The environment to wrap
-            min_reward (Union[float, np.ndarray]): lower bound to apply
-            max_reward (Union[float, np.ndarray]): higher bound to apply
+            env: The vector environment to wrap
+            min_reward: The min reward for each step
+            max_reward: the max reward for each step
         """
-        if min_reward is None and max_reward is None:
-            raise InvalidBound("Both `min_reward` and `max_reward` cannot be None")
-
-        elif max_reward is not None and min_reward is not None:
-            if np.any(max_reward - min_reward < 0):
-                raise InvalidBound(
-                    f"Min reward ({min_reward}) must be smaller than max reward ({max_reward})"
-                )
-
-        gym.utils.RecordConstructorArgs.__init__(
-            self, min_reward=min_reward, max_reward=max_reward
-        )
-        LambdaRewardV0.__init__(
-            self, env=env, func=lambda x: np.clip(x, a_min=min_reward, a_max=max_reward)
+        super().__init__(
+            env,
+            transform_reward.ClipReward,
+            min_reward=min_reward,
+            max_reward=max_reward,
         )
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/rendering.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/rendering.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A collections of rendering-based wrappers.
 
-* ``RenderCollectionV0`` - Collects rendered frames into a list
-* ``RecordVideoV0`` - Records a video of the environments
-* ``HumanRenderingV0`` - Provides human rendering of environments with ``"rgb_array"``
+* ``RenderCollection`` - Collects rendered frames into a list
+* ``RecordVideo`` - Records a video of the environments
+* ``HumanRendering`` - Provides human rendering of environments with ``"rgb_array"``
 """
 from __future__ import annotations
 
 import os
 from copy import deepcopy
 from typing import Any, Callable, List, SupportsFloat
 
@@ -14,21 +14,84 @@
 
 import gymnasium as gym
 from gymnasium import error, logger
 from gymnasium.core import ActType, ObsType, RenderFrame
 from gymnasium.error import DependencyNotInstalled
 
 
-__all__ = ["RenderCollectionV0", "RecordVideoV0", "HumanRenderingV0"]
+__all__ = [
+    "RenderCollection",
+    "RecordVideo",
+    "HumanRendering",
+]
 
 
-class RenderCollectionV0(
+class RenderCollection(
     gym.Wrapper[ObsType, ActType, ObsType, ActType], gym.utils.RecordConstructorArgs
 ):
-    """Collect rendered frames of an environment such ``render`` returns a ``list[RenderedFrame]``."""
+    """Collect rendered frames of an environment such ``render`` returns a ``list[RenderedFrame]``.
+
+    No vector version of the wrapper exists.
+
+    Example:
+        Return the list of frames for the number of steps ``render`` wasn't called.
+        >>> import gymnasium as gym
+        >>> env = gym.make("LunarLander-v2", render_mode="rgb_array")
+        >>> env = RenderCollection(env)
+        >>> _ = env.reset(seed=123)
+        >>> for _ in range(5):
+        ...     _ = env.step(env.action_space.sample())
+        ...
+        >>> frames = env.render()
+        >>> len(frames)
+        6
+
+        >>> frames = env.render()
+        >>> len(frames)
+        0
+
+        Return the list of frames for the number of steps the episode was running.
+        >>> import gymnasium as gym
+        >>> env = gym.make("LunarLander-v2", render_mode="rgb_array")
+        >>> env = RenderCollection(env, pop_frames=False)
+        >>> _ = env.reset(seed=123)
+        >>> for _ in range(5):
+        ...     _ = env.step(env.action_space.sample())
+        ...
+        >>> frames = env.render()
+        >>> len(frames)
+        6
+
+        >>> frames = env.render()
+        >>> len(frames)
+        6
+
+        Collect all frames for all episodes, without clearing them when render is called
+        >>> import gymnasium as gym
+        >>> env = gym.make("LunarLander-v2", render_mode="rgb_array")
+        >>> env = RenderCollection(env, pop_frames=False, reset_clean=False)
+        >>> _ = env.reset(seed=123)
+        >>> for _ in range(5):
+        ...     _ = env.step(env.action_space.sample())
+        ...
+        >>> _ = env.reset(seed=123)
+        >>> for _ in range(5):
+        ...     _ = env.step(env.action_space.sample())
+        ...
+        >>> frames = env.render()
+        >>> len(frames)
+        12
+
+        >>> frames = env.render()
+        >>> len(frames)
+        12
+
+    Change logs:
+     * v0.26.2 - Initially added
+    """
 
     def __init__(
         self,
         env: gym.Env[ObsType, ActType],
         pop_frames: bool = True,
         reset_clean: bool = True,
     ):
@@ -85,54 +148,112 @@
         frames = self.frame_list
         if self.pop_frames:
             self.frame_list = []
 
         return frames
 
 
-class RecordVideoV0(
+class RecordVideo(
     gym.Wrapper[ObsType, ActType, ObsType, ActType], gym.utils.RecordConstructorArgs
 ):
-    """This wrapper records videos of rollouts.
+    """Records videos of environment episodes using the environment's render function.
 
-    Usually, you only want to record episodes intermittently, say every hundredth episode.
+    .. py:currentmodule:: gymnasium.utils.save_video
+
+    Usually, you only want to record episodes intermittently, say every hundredth episode or at every thousandth environment step.
     To do this, you can specify ``episode_trigger`` or ``step_trigger``.
     They should be functions returning a boolean that indicates whether a recording should be started at the
     current episode or step, respectively.
-    If neither :attr:`episode_trigger` nor ``step_trigger`` is passed, a default ``episode_trigger`` will be employed,
-    i.e. capped_cubic_video_schedule. This function starts a video at every episode that is a power of 3 until 1000 and
-    then every 1000 episodes.
-    By default, the recording will be stopped once reset is called. However, you can also create recordings of fixed
-    length (possibly spanning several episodes) by passing a strictly positive value for ``video_length``.
+
+    The ``episode_trigger`` should return ``True`` on the episode when recording should start.
+    The ``step_trigger`` should return ``True`` on the n-th environment step that the recording should be started, where n sums over all previous episodes.
+    If neither :attr:`episode_trigger` nor ``step_trigger`` is passed, a default ``episode_trigger`` will be employed, i.e. :func:`capped_cubic_video_schedule`.
+    This function starts a video at every episode that is a power of 3 until 1000 and then every 1000 episodes.
+    By default, the recording will be stopped once reset is called.
+    However, you can also create recordings of fixed length (possibly spanning several episodes)
+    by passing a strictly positive value for ``video_length``.
+
+    No vector version of the wrapper exists.
+
+    Examples - Run the environment for 50 episodes, and save the video every 10 episodes starting from the 0th:
+        >>> import os
+        >>> import gymnasium as gym
+        >>> env = gym.make("LunarLander-v2", render_mode="rgb_array")
+        >>> trigger = lambda t: t % 10 == 0
+        >>> env = RecordVideo(env, video_folder="./save_videos1", episode_trigger=trigger, disable_logger=True)
+        >>> for i in range(50):
+        ...     termination, truncation = False, False
+        ...     _ = env.reset(seed=123)
+        ...     while not (termination or truncation):
+        ...         obs, rew, termination, truncation, info = env.step(env.action_space.sample())
+        ...
+        >>> env.close()
+        >>> len(os.listdir("./save_videos1"))
+        5
+
+    Examples - Run the environment for 5 episodes, start a recording every 200th step, making sure each video is 100 frames long:
+        >>> import os
+        >>> import gymnasium as gym
+        >>> env = gym.make("LunarLander-v2", render_mode="rgb_array")
+        >>> trigger = lambda t: t % 200 == 0
+        >>> env = RecordVideo(env, video_folder="./save_videos2", step_trigger=trigger, video_length=100, disable_logger=True)
+        >>> for i in range(5):
+        ...     termination, truncation = False, False
+        ...     _ = env.reset(seed=123)
+        ...     _ = env.action_space.seed(123)
+        ...     while not (termination or truncation):
+        ...         obs, rew, termination, truncation, info = env.step(env.action_space.sample())
+        ...
+        >>> env.close()
+        >>> len(os.listdir("./save_videos2"))
+        2
+
+    Examples - Run 3 episodes, record everything, but in chunks of 1000 frames:
+        >>> import os
+        >>> import gymnasium as gym
+        >>> env = gym.make("LunarLander-v2", render_mode="rgb_array")
+        >>> env = RecordVideo(env, video_folder="./save_videos3", video_length=1000, disable_logger=True)
+        >>> for i in range(3):
+        ...     termination, truncation = False, False
+        ...     _ = env.reset(seed=123)
+        ...     while not (termination or truncation):
+        ...         obs, rew, termination, truncation, info = env.step(env.action_space.sample())
+        ...
+        >>> env.close()
+        >>> len(os.listdir("./save_videos3"))
+        2
+
+    Change logs:
+     * v0.25.0 - Initially added to replace ``wrappers.monitoring.VideoRecorder``
     """
 
     def __init__(
         self,
         env: gym.Env[ObsType, ActType],
         video_folder: str,
         episode_trigger: Callable[[int], bool] | None = None,
         step_trigger: Callable[[int], bool] | None = None,
         video_length: int = 0,
         name_prefix: str = "rl-video",
         fps: int | None = None,
-        disable_logger: bool = False,
+        disable_logger: bool = True,
     ):
         """Wrapper records videos of rollouts.
 
         Args:
             env: The environment that will be wrapped
             video_folder (str): The folder where the recordings will be stored
             episode_trigger: Function that accepts an integer and returns ``True`` iff a recording should be started at this episode
             step_trigger: Function that accepts an integer and returns ``True`` iff a recording should be started at this step
             video_length (int): The length of recorded episodes. If 0, entire episodes are recorded.
                 Otherwise, snippets of the specified length are captured
             name_prefix (str): Will be prepended to the filename of the recordings
-            fps (int): The frame per second in the video. The default value is the one specified in the environment metadata.
-                If the environment metadata doesn't specify `render_fps`, the value 30 is used.
-            disable_logger (bool): Whether to disable moviepy logger or not
+            fps (int): The frame per second in the video. Provides a custom video fps for environment, if ``None`` then
+                the environment metadata ``render_fps`` key is used if it exists, otherwise a default value of 30 is used.
+            disable_logger (bool): Whether to disable moviepy logger or not, default it is disabled
         """
         gym.utils.RecordConstructorArgs.__init__(
             self,
             video_folder=video_folder,
             episode_trigger=episode_trigger,
             step_trigger=step_trigger,
             video_length=video_length,
@@ -144,20 +265,15 @@
         if env.render_mode in {None, "human", "ansi"}:
             raise ValueError(
                 f"Render mode is {env.render_mode}, which is incompatible with RecordVideo.",
                 "Initialize your environment with a render_mode that returns an image, such as rgb_array.",
             )
 
         if episode_trigger is None and step_trigger is None:
-
-            def capped_cubic_video_schedule(episode_id: int) -> bool:
-                if episode_id < 1000:
-                    return int(round(episode_id ** (1.0 / 3))) ** 3 == episode_id
-                else:
-                    return episode_id % 1000 == 0
+            from gymnasium.utils.save_video import capped_cubic_video_schedule
 
             episode_trigger = capped_cubic_video_schedule
 
         self.episode_trigger = episode_trigger
         self.step_trigger = step_trigger
         self.disable_logger = disable_logger
 
@@ -200,16 +316,15 @@
             frame = frame[-1]
 
         if isinstance(frame, np.ndarray):
             self.recorded_frames.append(frame)
         else:
             self.stop_recording()
             logger.warn(
-                "Recording stopped: expected type of frame returned by render ",
-                f"to be a numpy array, got instead {type(frame)}.",
+                f"Recording stopped: expected type of frame returned by render to be a numpy array, got instead {type(frame)}."
             )
 
     def reset(
         self, *, seed: int | None = None, options: dict[str, Any] | None = None
     ) -> tuple[ObsType, dict[str, Any]]:
         """Reset the environment and eventually starts a new recording."""
         obs, info = super().reset(seed=seed, options=options)
@@ -240,14 +355,33 @@
             self._capture_frame()
 
             if len(self.recorded_frames) > self.video_length:
                 self.stop_recording()
 
         return obs, rew, terminated, truncated, info
 
+    def render(self) -> RenderFrame | list[RenderFrame]:
+        """Compute the render frames as specified by render_mode attribute during initialization of the environment."""
+        render_out = super().render()
+        if self.recording and isinstance(render_out, List):
+            self.recorded_frames += render_out
+
+        if len(self.render_history) > 0:
+            tmp_history = self.render_history
+            self.render_history = []
+            return tmp_history + render_out
+        else:
+            return render_out
+
+    def close(self):
+        """Closes the wrapper then the video recorder."""
+        super().close()
+        if self.recording:
+            self.stop_recording()
+
     def start_recording(self, video_name: str):
         """Start a new recording. If it is already recording, stops the current recording before starting the new one."""
         if self.recording:
             self.stop_recording()
 
         self.recording = True
         self._video_name = video_name
@@ -271,73 +405,59 @@
             path = os.path.join(self.video_folder, f"{self._video_name}.mp4")
             clip.write_videofile(path, logger=moviepy_logger)
 
         self.recorded_frames = []
         self.recording = False
         self._video_name = None
 
-    def render(self) -> RenderFrame | list[RenderFrame]:
-        """Compute the render frames as specified by render_mode attribute during initialization of the environment."""
-        render_out = super().render()
-        if self.recording and isinstance(render_out, List):
-            self.recorded_frames += render_out
-
-        if len(self.render_history) > 0:
-            tmp_history = self.render_history
-            self.render_history = []
-            return tmp_history + render_out
-        else:
-            return render_out
-
-    def close(self):
-        """Closes the wrapper then the video recorder."""
-        super().close()
-        if self.recording:
-            self.stop_recording()
-
     def __del__(self):
         """Warn the user in case last video wasn't saved."""
         if len(self.recorded_frames) > 0:
             logger.warn("Unable to save last video! Did you call close()?")
 
 
-class HumanRenderingV0(
+class HumanRendering(
     gym.Wrapper[ObsType, ActType, ObsType, ActType], gym.utils.RecordConstructorArgs
 ):
-    """Performs human rendering for an environment that only supports "rgb_array"rendering.
+    """Allows human like rendering for environments that support "rgb_array" rendering.
 
     This wrapper is particularly useful when you have implemented an environment that can produce
     RGB images but haven't implemented any code to render the images to the screen.
     If you want to use this wrapper with your environments, remember to specify ``"render_fps"``
     in the metadata of your environment.
 
     The ``render_mode`` of the wrapped environment must be either ``'rgb_array'`` or ``'rgb_array_list'``.
 
+    No vector version of the wrapper exists.
+
     Example:
         >>> import gymnasium as gym
-        >>> from gymnasium.experimental.wrappers import HumanRenderingV0
+        >>> from gymnasium.wrappers import HumanRendering
         >>> env = gym.make("LunarLander-v2", render_mode="rgb_array")
-        >>> wrapped = HumanRenderingV0(env)
+        >>> wrapped = HumanRendering(env)
         >>> obs, _ = wrapped.reset()     # This will start rendering to the screen
 
         The wrapper can also be applied directly when the environment is instantiated, simply by passing
         ``render_mode="human"`` to ``make``. The wrapper will only be applied if the environment does not
         implement human-rendering natively (i.e. ``render_mode`` does not contain ``"human"``).
 
         >>> env = gym.make("phys2d/CartPole-v1", render_mode="human")      # CartPoleJax-v1 doesn't implement human-rendering natively
         >>> obs, _ = env.reset()     # This will start rendering to the screen
 
         Warning: If the base environment uses ``render_mode="rgb_array_list"``, its (i.e. the *base environment's*) render method
         will always return an empty list:
 
         >>> env = gym.make("LunarLander-v2", render_mode="rgb_array_list")
-        >>> wrapped = HumanRenderingV0(env)
+        >>> wrapped = HumanRendering(env)
         >>> obs, _ = wrapped.reset()
         >>> env.render() # env.render() will always return an empty list!
         []
+
+    Change logs:
+     * v0.25.0 - Initially added
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType]):
         """Initialize a :class:`HumanRendering` instance.
 
         Args:
             env: The environment that is being wrapped
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/stateful_observation.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/stateful_observation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 """A collection of stateful observation wrappers.
 
-* ``DelayObservationV0`` - A wrapper for delaying the returned observation
-* ``TimeAwareObservationV0`` - A wrapper for adding time aware observations to environment observation
-* ``FrameStackObservationV0`` - Frame stack the observations
-* ``NormalizeObservationV0`` - Normalized the observations to a mean and
-* ``MaxAndSkipObservationV0`` - Return only every ``skip``-th frame (frameskipping) and return the max between the two last frames.
+* ``DelayObservation`` - A wrapper for delaying the returned observation
+* ``TimeAwareObservation`` - A wrapper for adding time aware observations to environment observation
+* ``FrameStackObservation`` - Frame stack the observations
+* ``NormalizeObservation`` - Normalized the observations to have unit variance with a moving mean
+* ``MaxAndSkipObservation`` - Return only every ``skip``-th frame (frameskipping) and return the max between the two last frames.
 """
 from __future__ import annotations
 
 from collections import deque
 from copy import deepcopy
 from typing import Any, Final, SupportsFloat
 
 import numpy as np
 
 import gymnasium as gym
 import gymnasium.spaces as spaces
 from gymnasium.core import ActType, ObsType, WrapperActType, WrapperObsType
-from gymnasium.experimental.vector.utils import (
-    batch_space,
-    concatenate,
-    create_empty_array,
-)
-from gymnasium.experimental.wrappers.utils import RunningMeanStd, create_zero_array
 from gymnasium.spaces import Box, Dict, Tuple
+from gymnasium.vector.utils import batch_space, concatenate, create_empty_array
+from gymnasium.wrappers.utils import RunningMeanStd, create_zero_array
 
 
 __all__ = [
-    "DelayObservationV0",
-    "TimeAwareObservationV0",
-    "FrameStackObservationV0",
-    "NormalizeObservationV0",
+    "DelayObservation",
+    "TimeAwareObservation",
+    "FrameStackObservation",
+    "NormalizeObservation",
+    "MaxAndSkipObservation",
 ]
 
 
-class DelayObservationV0(
+class DelayObservation(
     gym.ObservationWrapper[ObsType, ActType, ObsType], gym.utils.RecordConstructorArgs
 ):
-    """Wrapper which adds a delay to the returned observation.
+    """Adds a delay to the returned observation from the environment.
 
     Before reaching the :attr:`delay` number of timesteps, returned observations is an array of zeros with
     the same shape as the observation space.
 
+    No vector version of the wrapper exists.
+
+    Note:
+        This does not support random delay values, if users are interested, please raise an issue or pull request to add this feature.
+
     Example:
         >>> import gymnasium as gym
         >>> env = gym.make("CartPole-v1")
         >>> env.reset(seed=123)
         (array([ 0.01823519, -0.0446179 , -0.02796401, -0.03156282], dtype=float32), {})
 
-        >>> env = DelayObservationV0(env, delay=2)
+        >>> env = DelayObservation(env, delay=2)
         >>> env.reset(seed=123)
         (array([0., 0., 0., 0.], dtype=float32), {})
         >>> env.step(env.action_space.sample())
         (array([0., 0., 0., 0.], dtype=float32), 1.0, False, False, {})
         >>> env.step(env.action_space.sample())
         (array([ 0.01823519, -0.0446179 , -0.02796401, -0.03156282], dtype=float32), 1.0, False, False, {})
 
-    Note:
-        This does not support random delay values, if users are interested, please raise an issue or pull request to add this feature.
+    Change logs:
+     * v1.0.0 - Initially added
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType], delay: int):
         """Initialises the DelayObservation wrapper with an integer.
 
         Args:
             env: The environment to wrap
@@ -96,80 +98,88 @@
 
         if len(self.observation_queue) > self.delay:
             return self.observation_queue.popleft()
         else:
             return create_zero_array(self.observation_space)
 
 
-class TimeAwareObservationV0(
+class TimeAwareObservation(
     gym.ObservationWrapper[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Augment the observation with time information of the episode.
+    """Augment the observation with the number of time steps taken within an episode.
 
     The :attr:`normalize_time` if ``True`` represents time as a normalized value between [0,1]
-    otherwise if ``False``, the number of timesteps remaining before truncation occurs is an integer.
+    otherwise if ``False``, the current timestep is an integer.
 
     For environments with ``Dict`` observation spaces, the time information is automatically
     added in the key `"time"` (can be changed through :attr:`dict_time_key`) and for environments with ``Tuple``
     observation space, the time information is added as the final element in the tuple.
     Otherwise, the observation space is transformed into a ``Dict`` observation space with two keys,
     `"obs"` for the base environment's observation and `"time"` for the time information.
 
     To flatten the observation, use the :attr:`flatten` parameter which will use the
     :func:`gymnasium.spaces.utils.flatten` function.
 
+    No vector version of the wrapper exists.
+
     Example:
         >>> import gymnasium as gym
-        >>> from gymnasium.experimental.wrappers import TimeAwareObservationV0
+        >>> from gymnasium.wrappers import TimeAwareObservation
         >>> env = gym.make("CartPole-v1")
-        >>> env = TimeAwareObservationV0(env)
+        >>> env = TimeAwareObservation(env)
         >>> env.observation_space
-        Dict('obs': Box([-4.8000002e+00 -3.4028235e+38 -4.1887903e-01 -3.4028235e+38], [4.8000002e+00 3.4028235e+38 4.1887903e-01 3.4028235e+38], (4,), float32), 'time': Box(0.0, 1.0, (1,), float32))
+        Box([-4.80000019e+00 -3.40282347e+38 -4.18879032e-01 -3.40282347e+38
+          0.00000000e+00], [4.80000019e+00 3.40282347e+38 4.18879032e-01 3.40282347e+38
+         5.00000000e+02], (5,), float64)
         >>> env.reset(seed=42)[0]
-        {'obs': array([ 0.0273956 , -0.00611216,  0.03585979,  0.0197368 ], dtype=float32), 'time': array([0.], dtype=float32)}
+        array([ 0.0273956 , -0.00611216,  0.03585979,  0.0197368 ,  0.        ])
         >>> _ = env.action_space.seed(42)
         >>> env.step(env.action_space.sample())[0]
-        {'obs': array([ 0.02727336, -0.20172954,  0.03625453,  0.32351476], dtype=float32), 'time': array([0.002], dtype=float32)}
+        array([ 0.02727336, -0.20172954,  0.03625453,  0.32351476,  1.        ])
 
-    Unnormalize time observation space example:
+    Normalize time observation space example:
         >>> env = gym.make('CartPole-v1')
-        >>> env = TimeAwareObservationV0(env, normalize_time=False)
-        >>> env.observation_space
-        Dict('obs': Box([-4.8000002e+00 -3.4028235e+38 -4.1887903e-01 -3.4028235e+38], [4.8000002e+00 3.4028235e+38 4.1887903e-01 3.4028235e+38], (4,), float32), 'time': Box(0, 500, (1,), int32))
-        >>> env.reset(seed=42)[0]
-        {'obs': array([ 0.0273956 , -0.00611216,  0.03585979,  0.0197368 ], dtype=float32), 'time': array([500], dtype=int32)}
-        >>> _ = env.action_space.seed(42)[0]
-        >>> env.step(env.action_space.sample())[0]
-        {'obs': array([ 0.02727336, -0.20172954,  0.03625453,  0.32351476], dtype=float32), 'time': array([499], dtype=int32)}
-
-    Flatten observation space example:
-        >>> env = gym.make("CartPole-v1")
-        >>> env = TimeAwareObservationV0(env, flatten=True)
+        >>> env = TimeAwareObservation(env, normalize_time=True)
         >>> env.observation_space
         Box([-4.8000002e+00 -3.4028235e+38 -4.1887903e-01 -3.4028235e+38
           0.0000000e+00], [4.8000002e+00 3.4028235e+38 4.1887903e-01 3.4028235e+38 1.0000000e+00], (5,), float32)
         >>> env.reset(seed=42)[0]
         array([ 0.0273956 , -0.00611216,  0.03585979,  0.0197368 ,  0.        ],
               dtype=float32)
         >>> _ = env.action_space.seed(42)
         >>> env.step(env.action_space.sample())[0]
         array([ 0.02727336, -0.20172954,  0.03625453,  0.32351476,  0.002     ],
               dtype=float32)
+
+    Flatten observation space example:
+        >>> env = gym.make("CartPole-v1")
+        >>> env = TimeAwareObservation(env, flatten=False)
+        >>> env.observation_space
+        Dict('obs': Box([-4.8000002e+00 -3.4028235e+38 -4.1887903e-01 -3.4028235e+38], [4.8000002e+00 3.4028235e+38 4.1887903e-01 3.4028235e+38], (4,), float32), 'time': Box(0, 500, (1,), int32))
+        >>> env.reset(seed=42)[0]
+        {'obs': array([ 0.0273956 , -0.00611216,  0.03585979,  0.0197368 ], dtype=float32), 'time': array([0], dtype=int32)}
+        >>> _ = env.action_space.seed(42)
+        >>> env.step(env.action_space.sample())[0]
+        {'obs': array([ 0.02727336, -0.20172954,  0.03625453,  0.32351476], dtype=float32), 'time': array([1], dtype=int32)}
+
+    Change logs:
+     * v0.18.0 - Initially added
+     * v1.0.0 - Remove vector environment support, add ``flatten`` and ``normalize_time`` parameters
     """
 
     def __init__(
         self,
         env: gym.Env[ObsType, ActType],
-        flatten: bool = False,
-        normalize_time: bool = True,
+        flatten: bool = True,
+        normalize_time: bool = False,
         *,
         dict_time_key: str = "time",
     ):
-        """Initialize :class:`TimeAwareObservationV0`.
+        """Initialize :class:`TimeAwareObservation`.
 
         Args:
             env: The environment to apply the wrapper
             flatten: Flatten the observation to a `Box` of a single dimension
             normalize_time: if `True` return time in the range [0,1]
                 otherwise return time as remaining timesteps before truncation
             dict_time_key: For environment with a ``Dict`` observation space, the key for the time space. By default, `"time"`.
@@ -189,26 +199,24 @@
         if env.spec is not None and env.spec.max_episode_steps is not None:
             self.max_timesteps = env.spec.max_episode_steps
         else:
             raise ValueError(
                 "The environment must be wrapped by a TimeLimit wrapper or the spec specify a `max_episode_steps`."
             )
 
-        self._timesteps: int = 0
+        self.timesteps: int = 0
 
         # Find the normalized time space
         if self.normalize_time:
             self._time_preprocess_func = lambda time: np.array(
                 [time / self.max_timesteps], dtype=np.float32
             )
             time_space = Box(0.0, 1.0)
         else:
-            self._time_preprocess_func = lambda time: np.array(
-                [self.max_timesteps - time], dtype=np.int32
-            )
+            self._time_preprocess_func = lambda time: np.array([time], dtype=np.int32)
             time_space = Box(0, self.max_timesteps, dtype=np.int32)
 
         # Find the observation space
         if isinstance(env.observation_space, Dict):
             assert dict_time_key not in env.observation_space.keys()
             observation_space = Dict(
                 {dict_time_key: time_space, **env.observation_space.spaces}
@@ -240,30 +248,30 @@
             observation: The observation to add the time step to
 
         Returns:
             The observation with the time information appended to it
         """
         return self._obs_postprocess_func(
             self._append_data_func(
-                observation, self._time_preprocess_func(self._timesteps)
+                observation, self._time_preprocess_func(self.timesteps)
             )
         )
 
     def step(
         self, action: ActType
     ) -> tuple[WrapperObsType, SupportsFloat, bool, bool, dict[str, Any]]:
         """Steps through the environment, incrementing the time step.
 
         Args:
             action: The action to take
 
         Returns:
             The environment's step using the action with the next observation containing the timestep info
         """
-        self._timesteps += 1
+        self.timesteps += 1
 
         return super().step(action)
 
     def reset(
         self, *, seed: int | None = None, options: dict[str, Any] | None = None
     ) -> tuple[WrapperObsType, dict[str, Any]]:
         """Reset the environment setting the time to zero.
@@ -271,103 +279,150 @@
         Args:
             seed: The seed to reset the environment
             options: The options used to reset the environment
 
         Returns:
             Resets the environment with the initial timestep info added the observation
         """
-        self._timesteps = 0
+        self.timesteps = 0
 
         return super().reset(seed=seed, options=options)
 
 
-class FrameStackObservationV0(
+class FrameStackObservation(
     gym.Wrapper[WrapperObsType, ActType, ObsType, ActType],
     gym.utils.RecordConstructorArgs,
 ):
-    """Observation wrapper that stacks the observations in a rolling manner.
+    """Stacks the observations from the last ``N`` time steps in a rolling manner.
 
     For example, if the number of stacks is 4, then the returned observation contains
     the most recent 4 observations. For environment 'Pendulum-v1', the original observation
     is an array with shape [3], so if we stack 4 observations, the processed observation
     has shape [4, 3].
 
-    Note:
-        - After :meth:`reset` is called, the frame buffer will be filled with the initial observation.
-          I.e. the observation returned by :meth:`reset` will consist of `num_stack` many identical frames.
+    Users have options for the padded observation used:
+
+     * "reset" (default) - The reset value is repeated
+     * "zero" - A "zero"-like instance of the observation space
+     * custom - An instance of the observation space
+
+    No vector version of the wrapper exists.
 
     Example:
         >>> import gymnasium as gym
-        >>> from gymnasium.experimental.wrappers import FrameStackObservationV0
+        >>> from gymnasium.wrappers import FrameStackObservation
         >>> env = gym.make("CarRacing-v2")
-        >>> env = FrameStackObservationV0(env, 4)
+        >>> env = FrameStackObservation(env, stack_size=4)
         >>> env.observation_space
         Box(0, 255, (4, 96, 96, 3), uint8)
         >>> obs, _ = env.reset()
         >>> obs.shape
         (4, 96, 96, 3)
+
+    Example with different padding observations:
+        >>> env = gym.make("CartPole-v1")
+        >>> env.reset(seed=123)
+        (array([ 0.01823519, -0.0446179 , -0.02796401, -0.03156282], dtype=float32), {})
+        >>> stacked_env = FrameStackObservation(env, 3)   # the default is padding_type="reset"
+        >>> stacked_env.reset(seed=123)
+        (array([[ 0.01823519, -0.0446179 , -0.02796401, -0.03156282],
+               [ 0.01823519, -0.0446179 , -0.02796401, -0.03156282],
+               [ 0.01823519, -0.0446179 , -0.02796401, -0.03156282]],
+              dtype=float32), {})
+
+
+        >>> stacked_env = FrameStackObservation(env, 3, padding_type="zero")
+        >>> stacked_env.reset(seed=123)
+        (array([[ 0.        ,  0.        ,  0.        ,  0.        ],
+               [ 0.        ,  0.        ,  0.        ,  0.        ],
+               [ 0.01823519, -0.0446179 , -0.02796401, -0.03156282]],
+              dtype=float32), {})
+        >>> stacked_env = FrameStackObservation(env, 3, padding_type=np.array([1, -1, 0, 2], dtype=np.float32))
+        >>> stacked_env.reset(seed=123)
+        (array([[ 1.        , -1.        ,  0.        ,  2.        ],
+               [ 1.        , -1.        ,  0.        ,  2.        ],
+               [ 0.01823519, -0.0446179 , -0.02796401, -0.03156282]],
+              dtype=float32), {})
+
+    Change logs:
+     * v0.15.0 - Initially add as ``FrameStack`` with support for lz4
+     * v1.0.0 - Rename to ``FrameStackObservation`` and remove lz4 and ``LazyFrame`` support
+                along with adding the ``padding_type`` parameter
+
     """
 
     def __init__(
         self,
         env: gym.Env[ObsType, ActType],
         stack_size: int,
         *,
-        zeros_obs: ObsType | None = None,
+        padding_type: str | ObsType = "reset",
     ):
         """Observation wrapper that stacks the observations in a rolling manner.
 
         Args:
             env: The environment to apply the wrapper
-            stack_size: The number of frames to stack with zero_obs being used originally.
-            zeros_obs: Keyword only parameter that allows a custom padding observation at :meth:`reset`
+            stack_size: The number of frames to stack.
+            padding_type: The padding type to use when stacking the observations, options: "reset", "zero", custom obs
         """
+        gym.utils.RecordConstructorArgs.__init__(
+            self, stack_size=stack_size, padding_type=padding_type
+        )
+        gym.Wrapper.__init__(self, env)
+
         if not np.issubdtype(type(stack_size), np.integer):
             raise TypeError(
                 f"The stack_size is expected to be an integer, actual type: {type(stack_size)}"
             )
         if not 1 < stack_size:
             raise ValueError(
                 f"The stack_size needs to be greater than one, actual value: {stack_size}"
             )
-
-        gym.utils.RecordConstructorArgs.__init__(self, stack_size=stack_size)
-        gym.Wrapper.__init__(self, env)
+        if isinstance(padding_type, str) and (
+            padding_type == "reset" or padding_type == "zero"
+        ):
+            self.padding_value: ObsType = create_zero_array(env.observation_space)
+        elif padding_type in env.observation_space:
+            self.padding_value = padding_type
+            padding_type = "_custom"
+        else:
+            if isinstance(padding_type, str):
+                raise ValueError(  # we are guessing that the user just entered the "reset" or "zero" wrong
+                    f"Unexpected `padding_type`, expected 'reset', 'zero' or a custom observation space, actual value: {padding_type!r}"
+                )
+            else:
+                raise ValueError(
+                    f"Unexpected `padding_type`, expected 'reset', 'zero' or a custom observation space, actual value: {padding_type!r} not an instance of env observation ({env.observation_space})"
+                )
 
         self.observation_space = batch_space(env.observation_space, n=stack_size)
         self.stack_size: Final[int] = stack_size
+        self.padding_type: Final[str] = padding_type
 
-        self.zero_obs: Final[ObsType] = (
-            zeros_obs if zeros_obs else create_zero_array(env.observation_space)
-        )
-        self._stacked_obs = deque(
-            [self.zero_obs for _ in range(self.stack_size)], maxlen=self.stack_size
-        )
-        self._stacked_array = create_empty_array(
-            env.observation_space, n=self.stack_size
+        self.obs_queue = deque(
+            [self.padding_value for _ in range(self.stack_size)], maxlen=self.stack_size
         )
+        self.stacked_obs = create_empty_array(env.observation_space, n=self.stack_size)
 
     def step(
         self, action: WrapperActType
     ) -> tuple[WrapperObsType, SupportsFloat, bool, bool, dict[str, Any]]:
         """Steps through the environment, appending the observation to the frame buffer.
 
         Args:
             action: The action to step through the environment with
 
         Returns:
             Stacked observations, reward, terminated, truncated, and info from the environment
         """
-        obs, reward, terminated, truncated, info = super().step(action)
-        self._stacked_obs.append(obs)
+        obs, reward, terminated, truncated, info = self.env.step(action)
+        self.obs_queue.append(obs)
 
         updated_obs = deepcopy(
-            concatenate(
-                self.env.observation_space, self._stacked_obs, self._stacked_array
-            )
+            concatenate(self.env.observation_space, self.obs_queue, self.stacked_obs)
         )
         return updated_obs, reward, terminated, truncated, info
 
     def reset(
         self, *, seed: int | None = None, options: dict[str, Any] | None = None
     ) -> tuple[WrapperObsType, dict[str, Any]]:
         """Reset the environment, returning the stacked observation and info.
@@ -375,53 +430,82 @@
         Args:
             seed: The environment seed
             options: The reset options
 
         Returns:
             The stacked observations and info
         """
-        obs, info = super().reset(seed=seed, options=options)
+        obs, info = self.env.reset(seed=seed, options=options)
+
+        if self.padding_type == "reset":
+            self.padding_value = obs
         for _ in range(self.stack_size - 1):
-            self._stacked_obs.append(self.zero_obs)
-        self._stacked_obs.append(obs)
+            self.obs_queue.append(self.padding_value)
+        self.obs_queue.append(obs)
 
         updated_obs = deepcopy(
-            concatenate(
-                self.env.observation_space, self._stacked_obs, self._stacked_array
-            )
+            concatenate(self.env.observation_space, self.obs_queue, self.stacked_obs)
         )
         return updated_obs, info
 
 
-class NormalizeObservationV0(
+class NormalizeObservation(
     gym.ObservationWrapper[WrapperObsType, ActType, ObsType],
     gym.utils.RecordConstructorArgs,
 ):
-    """This wrapper will normalize observations s.t. each coordinate is centered with unit variance.
+    """Normalizes observations to be centered at the mean with unit variance.
 
-    The property `_update_running_mean` allows to freeze/continue the running mean calculation of the observation
-    statistics. If `True` (default), the `RunningMeanStd` will get updated every time `self.observation()` is called.
-    If `False`, the calculated statistics are used but not updated anymore; this may be used during evaluation.
+    The property :attr:`update_running_mean` allows to freeze/continue the running mean calculation of the observation
+    statistics. If ``True`` (default), the ``RunningMeanStd`` will get updated every time ``step`` or ``reset`` is called.
+    If ``False``, the calculated statistics are used but not updated anymore; this may be used during evaluation.
+
+    A vector version of the wrapper exists :class:`gymnasium.wrappers.vector.NormalizeObservation`.
 
     Note:
         The normalization depends on past trajectories and observations will not be normalized correctly if the wrapper was
         newly instantiated or the policy was changed recently.
+
+    Example:
+        >>> import numpy as np
+        >>> import gymnasium as gym
+        >>> env = gym.make("CartPole-v1")
+        >>> obs, info = env.reset(seed=123)
+        >>> term, trunc = False, False
+        >>> while not (term or trunc):
+        ...     obs, _, term, trunc, _ = env.step(1)
+        ...
+        >>> obs
+        array([ 0.1511158 ,  1.7183299 , -0.25533703, -2.8914354 ], dtype=float32)
+        >>> env = gym.make("CartPole-v1")
+        >>> env = NormalizeObservation(env)
+        >>> obs, info = env.reset(seed=123)
+        >>> term, trunc = False, False
+        >>> while not (term or trunc):
+        ...     obs, _, term, trunc, _ = env.step(1)
+        >>> obs
+        array([ 2.0059888,  1.5676788, -1.9944268, -1.6120394], dtype=float32)
+
+    Change logs:
+     * v0.21.0 - Initially add
+     * v1.0.0 - Add `update_running_mean` attribute to allow disabling of updating the running mean / standard, particularly useful for evaluation time.
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType], epsilon: float = 1e-8):
-        """This wrapper will normalize observations s.t. each coordinate is centered with unit variance.
+        """This wrapper will normalize observations such that each observation is centered with unit variance.
 
         Args:
             env (Env): The environment to apply the wrapper
             epsilon: A stability parameter that is used when scaling the observations.
         """
         gym.utils.RecordConstructorArgs.__init__(self, epsilon=epsilon)
         gym.ObservationWrapper.__init__(self, env)
 
-        self.obs_rms = RunningMeanStd(shape=self.observation_space.shape)
+        self.obs_rms = RunningMeanStd(
+            shape=self.observation_space.shape, dtype=self.observation_space.dtype
+        )
         self.epsilon = epsilon
         self._update_running_mean = True
 
     @property
     def update_running_mean(self) -> bool:
         """Property to freeze/continue the running mean calculation of the observation statistics."""
         return self._update_running_mean
@@ -430,27 +514,51 @@
     def update_running_mean(self, setting: bool):
         """Sets the property to freeze/continue the running mean calculation of the observation statistics."""
         self._update_running_mean = setting
 
     def observation(self, observation: ObsType) -> WrapperObsType:
         """Normalises the observation using the running mean and variance of the observations."""
         if self._update_running_mean:
-            self.obs_rms.update(observation)
+            self.obs_rms.update(np.array([observation]))
         return (observation - self.obs_rms.mean) / np.sqrt(
             self.obs_rms.var + self.epsilon
         )
 
 
-class MaxAndSkipObservationV0(
+class MaxAndSkipObservation(
     gym.Wrapper[WrapperObsType, ActType, ObsType, ActType],
     gym.utils.RecordConstructorArgs,
 ):
-    """This wrapper will return only every ``skip``-th frame (frameskipping) and return the max between the two last observations.
+    """Skips the N-th frame (observation) and return the max values between the two last observations.
+
+    No vector version of the wrapper exists.
+
+    Note:
+        This wrapper is based on the wrapper from [stable-baselines3](https://stable-baselines3.readthedocs.io/en/master/_modules/stable_baselines3/common/atari_wrappers.html#MaxAndSkipEnv)
+
+    Example:
+        >>> import gymnasium as gym
+        >>> env = gym.make("CartPole-v1")
+        >>> obs0, *_ = env.reset(seed=123)
+        >>> obs1, *_ = env.step(1)
+        >>> obs2, *_ = env.step(1)
+        >>> obs3, *_ = env.step(1)
+        >>> obs4, *_ = env.step(1)
+        >>> skip_and_max_obs = np.max(np.stack([obs3, obs4], axis=0), axis=0)
+        >>> env = gym.make("CartPole-v1")
+        >>> wrapped_env = MaxAndSkipObservation(env)
+        >>> wrapped_obs0, *_ = wrapped_env.reset(seed=123)
+        >>> wrapped_obs1, *_ = wrapped_env.step(1)
+        >>> np.all(obs0 == wrapped_obs0)
+        True
+        >>> np.all(wrapped_obs1 == skip_and_max_obs)
+        True
 
-    Note: This wrapper is based on the wrapper from stable-baselines3: https://stable-baselines3.readthedocs.io/en/master/_modules/stable_baselines3/common/atari_wrappers.html#MaxAndSkipEnv
+    Change logs:
+     * v1.0.0 - Initially add
     """
 
     def __init__(self, env: gym.Env[ObsType, ActType], skip: int = 4):
         """This wrapper will return only every ``skip``-th frame (frameskipping) and return the max between the two last frames.
 
         Args:
             env (Env): The environment to apply the wrapper
@@ -488,18 +596,17 @@
             Max of the last two observations, reward, terminated, truncated, and info from the environment
         """
         total_reward = 0.0
         terminated = truncated = False
         info = {}
         for i in range(self._skip):
             obs, reward, terminated, truncated, info = self.env.step(action)
-            done = terminated or truncated
             if i == self._skip - 2:
                 self._obs_buffer[0] = obs
             if i == self._skip - 1:
                 self._obs_buffer[1] = obs
             total_reward += float(reward)
-            if done:
+            if terminated or truncated:
                 break
-        max_frame = self._obs_buffer.max(axis=0)
+        max_frame = np.max(self._obs_buffer, axis=0)
 
         return max_frame, total_reward, terminated, truncated, info
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/stateful_reward.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/vector/stateful_reward.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,93 @@
 """A collection of wrappers for modifying the reward with an internal state.
 
-* ``NormalizeRewardV1`` - Normalizes the rewards to a mean and standard deviation
+* ``NormalizeReward`` - Normalizes the rewards to a mean and standard deviation
 """
 from __future__ import annotations
 
 from typing import Any, SupportsFloat
 
 import numpy as np
 
 import gymnasium as gym
 from gymnasium.core import ActType, ObsType
-from gymnasium.experimental.wrappers.utils import RunningMeanStd
+from gymnasium.vector.vector_env import ArrayType, VectorEnv, VectorWrapper
+from gymnasium.wrappers.utils import RunningMeanStd
 
 
-__all__ = ["NormalizeRewardV1"]
+__all__ = ["NormalizeReward"]
 
 
-class NormalizeRewardV1(
-    gym.Wrapper[ObsType, ActType, ObsType, ActType], gym.utils.RecordConstructorArgs
-):
+class NormalizeReward(VectorWrapper, gym.utils.RecordConstructorArgs):
     r"""This wrapper will normalize immediate rewards s.t. their exponential moving average has a fixed variance.
 
     The exponential moving average will have variance :math:`(1 - \gamma)^2`.
 
     The property `_update_running_mean` allows to freeze/continue the running mean calculation of the reward
     statistics. If `True` (default), the `RunningMeanStd` will get updated every time `self.normalize()` is called.
     If False, the calculated statistics are used but not updated anymore; this may be used during evaluation.
 
     Note:
-        In v0.27, NormalizeReward was updated as the forward discounted reward estimate was incorrect computed in Gym v0.25+.
-        For more detail, read [#3154](https://github.com/openai/gym/pull/3152).
-
-    Note:
         The scaling depends on past trajectories and rewards will not be scaled correctly if the wrapper was newly
         instantiated or the policy was changed recently.
+
+    Example without the normalize reward wrapper:
+        >>> import gymnasium as gym
+        >>> import numpy as np
+        >>> envs = gym.make_vec("MountainCarContinuous-v0", 3)
+        >>> _ = envs.reset(seed=123)
+        >>> _ = envs.action_space.seed(123)
+        >>> episode_rewards = []
+        >>> for _ in range(100):
+        ...     observation, reward, *_ = envs.step(envs.action_space.sample())
+        ...     episode_rewards.append(reward)
+        ...
+        >>> envs.close()
+        >>> np.mean(episode_rewards)
+        -0.03359492141887935
+        >>> np.std(episode_rewards)
+        0.029028230434438706
+
+    Example with the normalize reward wrapper:
+        >>> import gymnasium as gym
+        >>> import numpy as np
+        >>> envs = gym.make_vec("MountainCarContinuous-v0", 3)
+        >>> envs = NormalizeReward(envs)
+        >>> _ = envs.reset(seed=123)
+        >>> _ = envs.action_space.seed(123)
+        >>> episode_rewards = []
+        >>> for _ in range(100):
+        ...     observation, reward, *_ = envs.step(envs.action_space.sample())
+        ...     episode_rewards.append(reward)
+        ...
+        >>> envs.close()
+        >>> np.mean(episode_rewards)
+        -0.1598639586606745
+        >>> np.std(episode_rewards)
+        0.27800309628058434
     """
 
     def __init__(
         self,
-        env: gym.Env[ObsType, ActType],
+        env: VectorEnv,
         gamma: float = 0.99,
         epsilon: float = 1e-8,
     ):
         """This wrapper will normalize immediate rewards s.t. their exponential moving average has a fixed variance.
 
         Args:
             env (env): The environment to apply the wrapper
             epsilon (float): A stability parameter
             gamma (float): The discount factor that is used in the exponential moving average.
         """
         gym.utils.RecordConstructorArgs.__init__(self, gamma=gamma, epsilon=epsilon)
-        gym.Wrapper.__init__(self, env)
+        VectorWrapper.__init__(self, env)
 
-        self.rewards_running_means = RunningMeanStd(shape=())
-        self.discounted_reward: np.array = np.array([0.0])
+        self.return_rms = RunningMeanStd(shape=())
+        self.accumulated_reward: np.array = np.zeros((self.num_envs,), dtype=np.float32)
         self.gamma = gamma
         self.epsilon = epsilon
         self._update_running_mean = True
 
     @property
     def update_running_mean(self) -> bool:
         """Property to freeze/continue the running mean calculation of the reward statistics."""
@@ -65,21 +95,21 @@
 
     @update_running_mean.setter
     def update_running_mean(self, setting: bool):
         """Sets the property to freeze/continue the running mean calculation of the reward statistics."""
         self._update_running_mean = setting
 
     def step(
-        self, action: ActType
-    ) -> tuple[ObsType, SupportsFloat, bool, bool, dict[str, Any]]:
+        self, actions: ActType
+    ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict[str, Any]]:
         """Steps through the environment, normalizing the reward returned."""
-        obs, reward, terminated, truncated, info = super().step(action)
-        self.discounted_reward = self.discounted_reward * self.gamma * (
-            1 - terminated
-        ) + float(reward)
-        return obs, self.normalize(float(reward)), terminated, truncated, info
+        obs, reward, terminated, truncated, info = super().step(actions)
+        self.accumulated_reward = (
+            self.accumulated_reward * self.gamma * (1 - terminated) + reward
+        )
+        return obs, self.normalize(reward), terminated, truncated, info
 
     def normalize(self, reward: SupportsFloat):
         """Normalizes the rewards with the running mean rewards and their variance."""
         if self._update_running_mean:
-            self.rewards_running_means.update(self.discounted_reward)
-        return reward / np.sqrt(self.rewards_running_means.var + self.epsilon)
+            self.return_rms.update(self.accumulated_reward)
+        return reward / np.sqrt(self.return_rms.var + self.epsilon)
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/utils.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 __all__ = ["RunningMeanStd", "update_mean_var_count_from_moments", "create_zero_array"]
 
 
 class RunningMeanStd:
     """Tracks the mean, variance and count of values."""
 
     # https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance#Parallel_algorithm
-    def __init__(self, epsilon=1e-4, shape=()):
+    def __init__(self, epsilon=1e-4, shape=(), dtype=np.float64):
         """Tracks the mean, variance and count of values."""
-        self.mean = np.zeros(shape, "float64")
-        self.var = np.ones(shape, "float64")
+        self.mean = np.zeros(shape, dtype=dtype)
+        self.var = np.ones(shape, dtype=dtype)
         self.count = epsilon
 
     def update(self, x):
         """Updates the mean, var and count from a batch of samples."""
         batch_mean = np.mean(x, axis=0)
         batch_var = np.var(x, axis=0)
         batch_count = x.shape[0]
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/jax_to_numpy.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/vector/jax_to_numpy.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,29 +3,34 @@
 
 from typing import Any
 
 import jax.numpy as jnp
 
 from gymnasium.core import ActType, ObsType
 from gymnasium.error import DependencyNotInstalled
-from gymnasium.experimental.vector import VectorEnv, VectorWrapper
-from gymnasium.experimental.vector.vector_env import ArrayType
-from gymnasium.experimental.wrappers.jax_to_numpy import jax_to_numpy, numpy_to_jax
+from gymnasium.vector import VectorEnv, VectorWrapper
+from gymnasium.vector.vector_env import ArrayType
+from gymnasium.wrappers.jax_to_numpy import jax_to_numpy, numpy_to_jax
 
 
-__all__ = ["JaxToNumpyV0"]
+__all__ = ["JaxToNumpy"]
 
 
-class JaxToNumpyV0(VectorWrapper):
+class JaxToNumpy(VectorWrapper):
     """Wraps a jax vector environment so that it can be interacted with through numpy arrays.
 
     Notes:
-        A vectorized version of ``gymnasium.experimental.wrappers.JaxToNumpyV0``
+        A vectorized version of ``gymnasium.wrappers.JaxToNumpy``
 
     Actions must be provided as numpy arrays and observations, rewards, terminations and truncations will be returned as numpy arrays.
+
+    Example:
+        >>> import gymnasium as gym                                         # doctest: +SKIP
+        >>> envs = gym.make_vec("JaxEnv-vx", 3)                             # doctest: +SKIP
+        >>> envs = JaxToNumpy(envs)                                         # doctest: +SKIP
     """
 
     def __init__(self, env: VectorEnv):
         """Wraps an environment such that the input and outputs are numpy arrays.
 
         Args:
             env: the vector jax environment to wrap
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/jax_to_torch.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/vector/jax_to_torch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Vector wrapper class for converting between PyTorch and Jax."""
 from __future__ import annotations
 
 from typing import Any
 
 from gymnasium.core import ActType, ObsType
-from gymnasium.experimental.vector import VectorEnv, VectorWrapper
-from gymnasium.experimental.vector.vector_env import ArrayType
-from gymnasium.experimental.wrappers.jax_to_torch import (
-    Device,
-    jax_to_torch,
-    torch_to_jax,
-)
+from gymnasium.vector import VectorEnv, VectorWrapper
+from gymnasium.vector.vector_env import ArrayType
+from gymnasium.wrappers.jax_to_torch import Device, jax_to_torch, torch_to_jax
 
 
-__all__ = ["JaxToTorchV0"]
+__all__ = ["JaxToTorch"]
 
 
-class JaxToTorchV0(VectorWrapper):
+class JaxToTorch(VectorWrapper):
     """Wraps a Jax-based vector environment so that it can be interacted with through PyTorch Tensors.
 
     Actions must be provided as PyTorch Tensors and observations, rewards, terminations and truncations will be returned as PyTorch Tensors.
+
+    Example:
+        >>> import gymnasium as gym                                         # doctest: +SKIP
+        >>> envs = gym.make_vec("JaxEnv-vx", 3)                             # doctest: +SKIP
+        >>> envs = JaxToTorch(envs)                                         # doctest: +SKIP
     """
 
     def __init__(self, env: VectorEnv, device: Device | None = None):
         """Vector wrapper to change inputs and outputs to PyTorch tensors.
 
         Args:
             env: The Jax-based vector environment to wrap
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/numpy_to_torch.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/vector/numpy_to_torch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,46 @@
 """Wrapper for converting NumPy environments to PyTorch."""
 from __future__ import annotations
 
 from typing import Any
 
 from gymnasium.core import ActType, ObsType
-from gymnasium.experimental.vector import VectorEnv, VectorWrapper
-from gymnasium.experimental.vector.vector_env import ArrayType
-from gymnasium.experimental.wrappers.jax_to_torch import Device
-from gymnasium.experimental.wrappers.numpy_to_torch import (
-    numpy_to_torch,
-    torch_to_numpy,
-)
-
-
-__all__ = ["NumpyToTorchV0"]
-
-
-class NumpyToTorchV0(VectorWrapper):
-    """Wraps a numpy-based environment so that it can be interacted with through PyTorch Tensors."""
+from gymnasium.vector import VectorEnv, VectorWrapper
+from gymnasium.vector.vector_env import ArrayType
+from gymnasium.wrappers.jax_to_torch import Device
+from gymnasium.wrappers.numpy_to_torch import numpy_to_torch, torch_to_numpy
+
+
+__all__ = ["NumpyToTorch"]
+
+
+class NumpyToTorch(VectorWrapper):
+    """Wraps a numpy-based environment so that it can be interacted with through PyTorch Tensors.
+
+    Example:
+        >>> import torch
+        >>> import gymnasium as gym
+        >>> from gymnasium.wrappers.vector import NumpyToTorch
+        >>> envs = gym.make_vec("CartPole-v1", 3)
+        >>> envs = NumpyToTorch(envs)
+        >>> obs, _ = envs.reset(seed=123)
+        >>> type(obs)
+        <class 'torch.Tensor'>
+        >>> action = torch.tensor(envs.action_space.sample())
+        >>> obs, reward, terminated, truncated, info = envs.step(action)
+        >>> envs.close()
+        >>> type(obs)
+        <class 'torch.Tensor'>
+        >>> type(reward)
+        <class 'torch.Tensor'>
+        >>> type(terminated)
+        <class 'torch.Tensor'>
+        >>> type(truncated)
+        <class 'torch.Tensor'>
+    """
 
     def __init__(self, env: VectorEnv, device: Device | None = None):
         """Wrapper class to change inputs and outputs of environment to PyTorch tensors.
 
         Args:
             env: The Jax-based vector environment to wrap
             device: The device the torch Tensors should be moved to
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/record_episode_statistics.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/vector/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,40 +3,26 @@
 
 import time
 from collections import deque
 
 import numpy as np
 
 from gymnasium.core import ActType, ObsType
-from gymnasium.experimental.vector.vector_env import ArrayType, VectorEnv, VectorWrapper
+from gymnasium.vector.vector_env import ArrayType, VectorEnv, VectorWrapper
 
 
-__all__ = ["RecordEpisodeStatisticsV0"]
+__all__ = ["RecordEpisodeStatistics"]
 
 
-class RecordEpisodeStatisticsV0(VectorWrapper):
+class RecordEpisodeStatistics(VectorWrapper):
     """This wrapper will keep track of cumulative rewards and episode lengths.
 
-    At the end of an episode, the statistics of the episode will be added to ``info``
-    using the key ``episode``. If using a vectorized environment also the key
-    ``_episode`` is used which indicates whether the env at the respective index has
-    the episode statistics.
-
-    After the completion of an episode, ``info`` will look like this::
-
-        >>> info = {  # doctest: +SKIP
-        ...     ...
-        ...     "episode": {
-        ...         "r": "<cumulative reward>",
-        ...         "l": "<episode length>",
-        ...         "t": "<elapsed time since beginning of episode>"
-        ...     },
-        ... }
-
-    For a vectorized environments the output will be in the form of::
+    At the end of any episode within the vectorized env, the statistics of the episode
+    will be added to ``info`` using the key ``episode``, and the ``_episode`` key
+    is used to indicate the environment index which has a terminated or truncated episode.
 
         >>> infos = {  # doctest: +SKIP
         ...     ...
         ...     "episode": {
         ...         "r": "<array of cumulative reward for each done sub-environment>",
         ...         "l": "<array of episode length for each done sub-environment>",
         ...         "t": "<array of elapsed time since beginning of episode for each done sub-environment>"
@@ -46,47 +32,77 @@
 
     Moreover, the most recent rewards and episode lengths are stored in buffers that can be accessed via
     :attr:`wrapped_env.return_queue` and :attr:`wrapped_env.length_queue` respectively.
 
     Attributes:
         return_queue: The cumulative rewards of the last ``deque_size``-many episodes
         length_queue: The lengths of the last ``deque_size``-many episodes
+
+    Example:
+        >>> from pprint import pprint
+        >>> import gymnasium as gym
+        >>> envs = gym.make_vec("CartPole-v1", num_envs=3)
+        >>> envs = RecordEpisodeStatistics(envs)
+        >>> obs, info = envs.reset(123)
+        >>> _ = envs.action_space.seed(123)
+        >>> end = False
+        >>> while not end:
+        ...     obs, rew, term, trunc, info = envs.step(envs.action_space.sample())
+        ...     end = term.any() or trunc.any()
+        ...
+        >>> envs.close()
+        >>> pprint(info) # doctest: +SKIP
+        {'_episode': array([ True, False, False]),
+         '_final_info': array([ True, False, False]),
+         '_final_observation': array([ True, False, False]),
+         'episode': {'l': array([11,  0,  0], dtype=int32),
+                     'r': array([11.,  0.,  0.], dtype=float32),
+                     't': array([0.007812, 0.      , 0.      ], dtype=float32)},
+         'final_info': array([{}, None, None], dtype=object),
+         'final_observation': array([array([ 0.11448676,  0.9416149 , -0.20946532, -1.7619033 ], dtype=float32),
+               None, None], dtype=object)}
     """
 
-    def __init__(self, env: VectorEnv, deque_size: int = 100):
+    def __init__(
+        self,
+        env: VectorEnv,
+        buffer_length: int = 100,
+        stats_key: str = "episode",
+    ):
         """This wrapper will keep track of cumulative rewards and episode lengths.
 
         Args:
             env (Env): The environment to apply the wrapper
-            deque_size: The size of the buffers :attr:`return_queue` and :attr:`length_queue`
+            buffer_length: The size of the buffers :attr:`return_queue`, :attr:`length_queue` and :attr:`time_queue`
+            stats_key: The info key to save the data
         """
         super().__init__(env)
+        self._stats_key = stats_key
 
         self.episode_count = 0
 
         self.episode_start_times: np.ndarray = np.zeros(())
         self.episode_returns: np.ndarray = np.zeros(())
         self.episode_lengths: np.ndarray = np.zeros(())
 
-        self.return_queue = deque(maxlen=deque_size)
-        self.length_queue = deque(maxlen=deque_size)
+        self.time_queue = deque(maxlen=buffer_length)
+        self.return_queue = deque(maxlen=buffer_length)
+        self.length_queue = deque(maxlen=buffer_length)
 
     def reset(
         self,
         seed: int | list[int] | None = None,
         options: dict | None = None,
     ):
         """Resets the environment using kwargs and resets the episode returns and lengths."""
         obs, info = super().reset(seed=seed, options=options)
 
-        self.episode_start_times = np.full(
-            self.num_envs, time.perf_counter(), dtype=np.float32
-        )
-        self.episode_returns = np.zeros(self.num_envs, dtype=np.float32)
-        self.episode_lengths = np.zeros(self.num_envs, dtype=np.int32)
+        self.episode_start_times = np.full(self.num_envs, time.perf_counter())
+        self.episode_returns = np.zeros(self.num_envs)
+        self.episode_lengths = np.zeros(self.num_envs)
 
         return obs, info
 
     def step(
         self, actions: ActType
     ) -> tuple[ObsType, ArrayType, ArrayType, ArrayType, dict]:
         """Steps through the environment, recording the episode statistics."""
@@ -96,42 +112,42 @@
             terminations,
             truncations,
             infos,
         ) = self.env.step(actions)
 
         assert isinstance(
             infos, dict
-        ), f"`info` dtype is {type(infos)} while supported dtype is `dict`. This may be due to usage of other wrappers in the wrong order."
+        ), f"`vector.RecordEpisodeStatistics` requires `info` type to be `dict`, its actual type is {type(infos)}. This may be due to usage of other wrappers in the wrong order."
 
         self.episode_returns += rewards
         self.episode_lengths += 1
 
         dones = np.logical_or(terminations, truncations)
         num_dones = np.sum(dones)
 
         if num_dones:
-            if "episode" in infos or "_episode" in infos:
+            if self._stats_key in infos or f"_{self._stats_key}" in infos:
                 raise ValueError(
-                    "Attempted to add episode stats when they already exist"
+                    f"Attempted to add episode stats when they already exist, info keys: {list(infos.keys())}"
                 )
             else:
-                infos["episode"] = {
+                episode_time_length = np.round(
+                    time.perf_counter() - self.episode_start_times, 6
+                )
+                infos[self._stats_key] = {
                     "r": np.where(dones, self.episode_returns, 0.0),
                     "l": np.where(dones, self.episode_lengths, 0),
-                    "t": np.where(
-                        dones,
-                        np.round(time.perf_counter() - self.episode_start_times, 6),
-                        0.0,
-                    ),
+                    "t": np.where(dones, episode_time_length, 0.0),
                 }
-                infos["_episode"] = dones
+                infos[f"_{self._stats_key}"] = dones
 
             self.episode_count += num_dones
 
             for i in np.where(dones):
+                self.time_queue.extend(episode_time_length[i])
                 self.return_queue.extend(self.episode_returns[i])
                 self.length_queue.extend(self.episode_lengths[i])
 
             self.episode_lengths[dones] = 0
             self.episode_returns[dones] = 0
             self.episode_start_times[dones] = time.perf_counter()
```

### Comparing `gymnasium-0.29.1/gymnasium/experimental/wrappers/vector/vectorize_observation.py` & `gymnasium-1.0.0a1/gymnasium/wrappers/vector/vectorize_action.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,222 +1,253 @@
-"""Vectorizes observation wrappers to works for `VectorEnv`."""
+"""Vectorizes action wrappers to work for `VectorEnv`."""
 from __future__ import annotations
 
 from copy import deepcopy
-from typing import Any, Callable, Sequence
+from typing import Any, Callable
 
 import numpy as np
 
 from gymnasium import Space
-from gymnasium.core import Env, ObsType
-from gymnasium.experimental.vector import VectorEnv, VectorObservationWrapper
-from gymnasium.experimental.vector.utils import batch_space, concatenate, iterate
-from gymnasium.experimental.wrappers import lambda_observation
-from gymnasium.vector.utils import create_empty_array
-
-
-class LambdaObservationV0(VectorObservationWrapper):
-    """Transforms an observation via a function provided to the wrapper.
-
-    The function :attr:`func` will be applied to all vector observations.
-    If the observations from :attr:`func` are outside the bounds of the ``env``'s observation space, provide an :attr:`observation_space`.
+from gymnasium.core import ActType, Env
+from gymnasium.vector import VectorActionWrapper, VectorEnv
+from gymnasium.vector.utils import batch_space, concatenate, create_empty_array, iterate
+from gymnasium.wrappers import transform_action
+
+
+class TransformAction(VectorActionWrapper):
+    """Transforms an action via a function provided to the wrapper.
+
+    The function :attr:`func` will be applied to all vector actions.
+    If the observations from :attr:`func` are outside the bounds of the ``env``'s action space,
+    provide an :attr:`action_space` which specifies the action space for the vectorized environment.
+
+    Example - Without action transformation:
+        >>> import gymnasium as gym
+        >>> envs = gym.make_vec("MountainCarContinuous-v0", num_envs=3)
+        >>> _ = envs.action_space.seed(123)
+        >>> obs, info = envs.reset(seed=123)
+        >>> for _ in range(10):
+        ...     obs, rew, term, trunc, info = envs.step(envs.action_space.sample())
+        ...
+        >>> envs.close()
+        >>> obs
+        array([[-0.46553135, -0.00142543],
+               [-0.498371  , -0.00715587],
+               [-0.4651575 , -0.00624371]], dtype=float32)
+
+    Example - With action transformation:
+        >>> import gymnasium as gym
+        >>> from gymnasium.spaces import Box
+        >>> def shrink_action(act):
+        ...     return act * 0.3
+        ...
+        >>> envs = gym.make_vec("MountainCarContinuous-v0", num_envs=3)
+        >>> new_action_space = Box(low=shrink_action(envs.action_space.low), high=shrink_action(envs.action_space.high))
+        >>> envs = TransformAction(env=envs, func=shrink_action, action_space=new_action_space)
+        >>> _ = envs.action_space.seed(123)
+        >>> obs, info = envs.reset(seed=123)
+        >>> for _ in range(10):
+        ...     obs, rew, term, trunc, info = envs.step(envs.action_space.sample())
+        ...
+        >>> envs.close()
+        >>> obs
+        array([[-0.48468155, -0.00372536],
+               [-0.47599354, -0.00545912],
+               [-0.46543318, -0.00615723]], dtype=float32)
     """
 
     def __init__(
         self,
         env: VectorEnv,
-        vector_func: Callable[[ObsType], Any],
-        single_func: Callable[[ObsType], Any],
-        observation_space: Space | None = None,
+        func: Callable[[ActType], Any],
+        action_space: Space | None = None,
     ):
-        """Constructor for the lambda observation wrapper.
+        """Constructor for the lambda action wrapper.
 
         Args:
             env: The vector environment to wrap
-            vector_func: A function that will transform the vector observation. If this transformed observation is outside the observation space of ``env.observation_space`` then provide an ``observation_space``.
-            single_func: A function that will transform an individual observation.
-            observation_space: The observation spaces of the wrapper, if None, then it is assumed the same as ``env.observation_space``.
+            func: A function that will transform an action. If this transformed action is outside the action space of ``env.action_space`` then provide an ``action_space``.
+            action_space: The action spaces of the wrapper, if None, then it is assumed the same as ``env.action_space``.
         """
         super().__init__(env)
 
-        if observation_space is not None:
-            self.observation_space = observation_space
-
-        self.vector_func = vector_func
-        self.single_func = single_func
+        if action_space is not None:
+            self.action_space = action_space
 
-    def vector_observation(self, observation: ObsType) -> ObsType:
-        """Apply function to the vector observation."""
-        return self.vector_func(observation)
+        self.func = func
 
-    def single_observation(self, observation: ObsType) -> ObsType:
-        """Apply function to the single observation."""
-        return self.single_func(observation)
-
-
-class VectorizeLambdaObservationV0(VectorObservationWrapper):
-    """Vectori`es a single-agent lambda observation wrapper for vector environments."""
+    def actions(self, actions: ActType) -> ActType:
+        """Applies the :attr:`func` to the actions."""
+        return self.func(actions)
+
+
+class VectorizeTransformAction(VectorActionWrapper):
+    """Vectorizes a single-agent transform action wrapper for vector environments.
+
+    Example - Without action transformation:
+        >>> import gymnasium as gym
+        >>> envs = gym.make_vec("MountainCarContinuous-v0", num_envs=3)
+        >>> _ = envs.action_space.seed(123)
+        >>> obs, info = envs.reset(seed=123)
+        >>> obs, rew, term, trunc, info = envs.step(envs.action_space.sample())
+        >>> envs.close()
+        >>> obs
+        array([[-4.6343064e-01,  9.8971417e-05],
+               [-4.4488689e-01, -1.9375233e-03],
+               [-4.3118435e-01, -1.5342437e-03]], dtype=float32)
+
+    Example - Adding a transform that applies a ReLU to the action:
+        >>> import gymnasium as gym
+        >>> from gymnasium.wrappers import TransformAction
+        >>> envs = gym.make_vec("MountainCarContinuous-v0", num_envs=3)
+        >>> envs = VectorizeTransformAction(envs, wrapper=TransformAction, func=lambda x: (x > 0.0) * x, action_space=envs.single_action_space)
+        >>> _ = envs.action_space.seed(123)
+        >>> obs, info = envs.reset(seed=123)
+        >>> obs, rew, term, trunc, info = envs.step(envs.action_space.sample())
+        >>> envs.close()
+        >>> obs
+        array([[-4.6343064e-01,  9.8971417e-05],
+               [-4.4354835e-01, -5.9898634e-04],
+               [-4.3034542e-01, -6.9532328e-04]], dtype=float32)
+    """
 
-    class VectorizedEnv(Env):
-        """Fake single-agent environment uses for the single-agent wrapper."""
+    class _SingleEnv(Env):
+        """Fake single-agent environment used for the single-agent wrapper."""
 
-        def __init__(self, observation_space: Space):
+        def __init__(self, action_space: Space):
             """Constructor for the fake environment."""
-            self.observation_space = observation_space
+            self.action_space = action_space
 
     def __init__(
         self,
         env: VectorEnv,
-        wrapper: type[lambda_observation.LambdaObservationV0],
+        wrapper: type[transform_action.TransformAction],
         **kwargs: Any,
     ):
-        """Constructor for the vectorized lambda observation wrapper.
+        """Constructor for the vectorized lambda action wrapper.
 
         Args:
-            env: The vector environment to wrap.
+            env: The vector environment to wrap
             wrapper: The wrapper to vectorize
-            **kwargs: Keyword argument for the wrapper
+            **kwargs: Arguments for the LambdaAction wrapper
         """
         super().__init__(env)
 
-        self.wrapper = wrapper(
-            self.VectorizedEnv(self.env.single_observation_space), **kwargs
-        )
-        self.single_observation_space = self.wrapper.observation_space
-        self.observation_space = batch_space(
-            self.single_observation_space, self.num_envs
-        )
+        self.wrapper = wrapper(self._SingleEnv(self.env.single_action_space), **kwargs)
+        self.single_action_space = self.wrapper.action_space
+        self.action_space = batch_space(self.single_action_space, self.num_envs)
+
+        self.same_out = self.action_space == self.env.action_space
+        self.out = create_empty_array(self.single_action_space, self.num_envs)
 
-        self.same_out = self.observation_space == self.env.observation_space
-        self.out = create_empty_array(self.single_observation_space, self.num_envs)
+    def actions(self, actions: ActType) -> ActType:
+        """Applies the wrapper to each of the action.
 
-    def vector_observation(self, observation: ObsType) -> ObsType:
-        """Iterates over the vector observations applying the single-agent wrapper ``observation`` then concatenates the observations together again."""
+        Args:
+            actions: The actions to apply the function to
+
+        Returns:
+            The updated actions using the wrapper func
+        """
         if self.same_out:
             return concatenate(
-                self.single_observation_space,
+                self.single_action_space,
                 tuple(
-                    self.wrapper.func(obs)
-                    for obs in iterate(self.observation_space, observation)
+                    self.wrapper.func(action)
+                    for action in iterate(self.action_space, actions)
                 ),
-                observation,
+                actions,
             )
         else:
             return deepcopy(
                 concatenate(
-                    self.single_observation_space,
+                    self.single_action_space,
                     tuple(
-                        self.wrapper.func(obs)
-                        for obs in iterate(self.observation_space, observation)
+                        self.wrapper.func(action)
+                        for action in iterate(self.env.action_space, actions)
                     ),
                     self.out,
                 )
             )
 
-    def single_observation(self, observation: ObsType) -> ObsType:
-        """Transforms a single observation using the wrapper transformation function."""
-        return self.wrapper.func(observation)
 
+class ClipAction(VectorizeTransformAction):
+    """Clip the continuous action within the valid :class:`Box` observation space bound.
 
-class FilterObservationV0(VectorizeLambdaObservationV0):
-    """Vector wrapper for filtering dict or tuple observation spaces."""
-
-    def __init__(self, env: VectorEnv, filter_keys: Sequence[str | int]):
-        """Constructor for the filter observation wrapper.
-
-        Args:
-            env: The vector environment to wrap
-            filter_keys: The subspaces to be included, use a list of strings or integers for ``Dict`` and ``Tuple`` spaces respectivesly
-        """
-        super().__init__(
-            env, lambda_observation.FilterObservationV0, filter_keys=filter_keys
-        )
-
-
-class FlattenObservationV0(VectorizeLambdaObservationV0):
-    """Observation wrapper that flattens the observation."""
+    Example - Passing an out-of-bounds action to the environment to be clipped.
+        >>> import numpy as np
+        >>> import gymnasium as gym
+        >>> envs = gym.make_vec("MountainCarContinuous-v0", num_envs=3)
+        >>> envs = ClipAction(envs)
+        >>> _ = envs.action_space.seed(123)
+        >>> obs, info = envs.reset(seed=123)
+        >>> obs, rew, term, trunc, info = envs.step(np.array([5.0, -5.0, 2.0]))
+        >>> envs.close()
+        >>> obs
+        array([[-0.4624777 ,  0.00105192],
+               [-0.44504836, -0.00209899],
+               [-0.42884544,  0.00080468]], dtype=float32)
+    """
 
     def __init__(self, env: VectorEnv):
-        """Constructor for any environment's observation space that implements ``spaces.utils.flatten_space`` and ``spaces.utils.flatten``.
-
-        Args:
-            env:  The vector environment to wrap
-        """
-        super().__init__(env, lambda_observation.FlattenObservationV0)
-
-
-class GrayscaleObservationV0(VectorizeLambdaObservationV0):
-    """Observation wrapper that converts an RGB image to grayscale."""
-
-    def __init__(self, env: VectorEnv, keep_dim: bool = False):
-        """Constructor for an RGB image based environments to make the image grayscale.
-
-        Args:
-            env: The vector environment to wrap
-            keep_dim: If to keep the channel in the observation, if ``True``, ``obs.shape == 3`` else ``obs.shape == 2``
-        """
-        super().__init__(
-            env, lambda_observation.GrayscaleObservationV0, keep_dim=keep_dim
-        )
-
-
-class ResizeObservationV0(VectorizeLambdaObservationV0):
-    """Resizes image observations using OpenCV to shape."""
-
-    def __init__(self, env: VectorEnv, shape: tuple[int, ...]):
-        """Constructor that requires an image environment observation space with a shape.
+        """Constructor for the Clip Action wrapper.
 
         Args:
             env: The vector environment to wrap
-            shape: The resized observation shape
         """
-        super().__init__(env, lambda_observation.ResizeObservationV0, shape=shape)
+        super().__init__(env, transform_action.ClipAction)
 
 
-class ReshapeObservationV0(VectorizeLambdaObservationV0):
-    """Reshapes array based observations to shapes."""
-
-    def __init__(self, env: VectorEnv, shape: int | tuple[int, ...]):
-        """Constructor for env with Box observation space that has a shape product equal to the new shape product.
-
-        Args:
-            env: The vector environment to wrap
-            shape: The reshaped observation space
-        """
-        super().__init__(env, lambda_observation.ReshapeObservationV0, shape=shape)
-
-
-class RescaleObservationV0(VectorizeLambdaObservationV0):
-    """Linearly rescales observation to between a minimum and maximum value."""
+class RescaleAction(VectorizeTransformAction):
+    """Affinely rescales the continuous action space of the environment to the range [min_action, max_action].
+
+    Example - Without action scaling:
+        >>> import numpy as np
+        >>> import gymnasium as gym
+        >>> envs = gym.make_vec("MountainCarContinuous-v0", num_envs=3)
+        >>> _ = envs.action_space.seed(123)
+        >>> obs, info = envs.reset(seed=123)
+        >>> for _ in range(10):
+        ...     obs, rew, term, trunc, info = envs.step(0.5 * np.ones((3, 1)))
+        ...
+        >>> envs.close()
+        >>> obs
+        array([[-0.44799727,  0.00266526],
+               [-0.4351738 ,  0.00133522],
+               [-0.42683297,  0.00048403]], dtype=float32)
+
+    Example - With action scaling:
+        >>> import numpy as np
+        >>> import gymnasium as gym
+        >>> envs = gym.make_vec("MountainCarContinuous-v0", num_envs=3)
+        >>> envs = RescaleAction(envs, 0.0, 1.0)
+        >>> _ = envs.action_space.seed(123)
+        >>> obs, info = envs.reset(seed=123)
+        >>> for _ in range(10):
+        ...     obs, rew, term, trunc, info = envs.step(0.5 * np.ones((3, 1)))
+        ...
+        >>> envs.close()
+        >>> obs
+        array([[-0.48657528, -0.00395268],
+               [-0.47377947, -0.00529102],
+               [-0.46546045, -0.00614867]], dtype=float32)
+    """
 
     def __init__(
         self,
         env: VectorEnv,
-        min_obs: np.floating | np.integer | np.ndarray,
-        max_obs: np.floating | np.integer | np.ndarray,
+        min_action: float | int | np.ndarray,
+        max_action: float | int | np.ndarray,
     ):
-        """Constructor that requires the env observation spaces to be a :class:`Box`.
+        """Initializes the :class:`RescaleAction` wrapper.
 
         Args:
-            env: The vector environment to wrap
-            min_obs: The new minimum observation bound
-            max_obs: The new maximum observation bound
+            env (Env): The vector environment to wrap
+            min_action (float, int or np.ndarray): The min values for each action. This may be a numpy array or a scalar.
+            max_action (float, int or np.ndarray): The max values for each action. This may be a numpy array or a scalar.
         """
         super().__init__(
             env,
-            lambda_observation.RescaleObservationV0,
-            min_obs=min_obs,
-            max_obs=max_obs,
+            transform_action.RescaleAction,
+            min_action=min_action,
+            max_action=max_action,
         )
-
-
-class DtypeObservationV0(VectorizeLambdaObservationV0):
-    """Observation wrapper for transforming the dtype of an observation."""
-
-    def __init__(self, env: VectorEnv, dtype: Any):
-        """Constructor for Dtype observation wrapper.
-
-        Args:
-            env: The vector environment to wrap
-            dtype: The new dtype of the observation
-        """
-        super().__init__(env, lambda_observation.DtypeObservationV0, dtype=dtype)
```

### Comparing `gymnasium-0.29.1/gymnasium/logger.py` & `gymnasium-1.0.0a1/gymnasium/logger.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/spaces/__init__.py` & `gymnasium-1.0.0a1/gymnasium/spaces/__init__.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/spaces/box.py` & `gymnasium-1.0.0a1/gymnasium/spaces/box.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         return f"Box({self.low_repr}, {self.high_repr}, {self.shape}, {self.dtype})"
 
     def __eq__(self, other: Any) -> bool:
         """Check whether `other` is equivalent to this instance. Doesn't check dtype equivalence."""
         return (
             isinstance(other, Box)
             and (self.shape == other.shape)
-            # and (self.dtype == other.dtype)
+            and (self.dtype == other.dtype)
             and np.allclose(self.low, other.low)
             and np.allclose(self.high, other.high)
         )
 
     def __setstate__(self, state: Iterable[tuple[str, Any]] | Mapping[str, Any]):
         """Sets the state of the box for unpickling a box with legacy support."""
         super().__setstate__(state)
```

### Comparing `gymnasium-0.29.1/gymnasium/spaces/dict.py` & `gymnasium-1.0.0a1/gymnasium/spaces/dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         ...             }
         ...         ),
         ...     }
         ... )
 
     It can be convenient to use :class:`Dict` spaces if you want to make complex observations or actions more human-readable.
     Usually, it will not be possible to use elements of this space directly in learning code. However, you can easily
-    convert `Dict` observations to flat arrays by using a :class:`gymnasium.wrappers.FlattenObservation` wrapper.
+    convert :class:`Dict` observations to flat arrays by using a :class:`gymnasium.wrappers.FlattenObservation` wrapper.
     Similar wrappers can be implemented to deal with :class:`Dict` actions.
     """
 
     def __init__(
         self,
         spaces: None | dict[str, Space] | Sequence[tuple[str, Space]] = None,
         seed: dict | int | np.random.Generator | None = None,
```

### Comparing `gymnasium-0.29.1/gymnasium/spaces/discrete.py` & `gymnasium-1.0.0a1/gymnasium/spaces/discrete.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,16 @@
     def sample(self, mask: MaskNDArray | None = None) -> np.int64:
         """Generates a single random sample from this space.
 
         A sample will be chosen uniformly at random with the mask if provided
 
         Args:
             mask: An optional mask for if an action can be selected.
-                Expected `np.ndarray` of shape `(n,)` and dtype `np.int8` where `1` represents valid actions and `0` invalid / infeasible actions.
-                If there are no possible actions (i.e. `np.all(mask == 0)`) then `space.start` will be returned.
+                Expected `np.ndarray` of shape ``(n,)`` and dtype ``np.int8`` where ``1`` represents valid actions and ``0`` invalid / infeasible actions.
+                If there are no possible actions (i.e. ``np.all(mask == 0)``) then ``space.start`` will be returned.
 
         Returns:
             A sampled integer from the space
         """
         if mask is not None:
             assert isinstance(
                 mask, np.ndarray
```

### Comparing `gymnasium-0.29.1/gymnasium/spaces/graph.py` & `gymnasium-1.0.0a1/gymnasium/spaces/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     nodes: NDArray[Any]
     edges: NDArray[Any] | None
     edge_links: NDArray[Any] | None
 
 
 class Graph(Space[GraphInstance]):
-    r"""A space representing graph information as a series of `nodes` connected with `edges` according to an adjacency matrix represented as a series of `edge_links`.
+    r"""A space representing graph information as a series of ``nodes`` connected with ``edges`` according to an adjacency matrix represented as a series of ``edge_links``.
 
     Example:
         >>> from gymnasium.spaces import Graph, Box, Discrete
         >>> observation_space = Graph(node_space=Box(low=-100, high=100, shape=(3,)), edge_space=Discrete(3), seed=42)
         >>> observation_space.sample()
         GraphInstance(nodes=array([[-12.224312 ,  71.71958  ,  39.473606 ],
                [-81.16453  ,  95.12447  ,  52.22794  ],
@@ -118,22 +118,22 @@
                 NDArray[Any] | tuple[Any, ...] | None,
                 NDArray[Any] | tuple[Any, ...] | None,
             ]
         ) = None,
         num_nodes: int = 10,
         num_edges: int | None = None,
     ) -> GraphInstance:
-        """Generates a single sample graph with num_nodes between 1 and 10 sampled from the Graph.
+        """Generates a single sample graph with num_nodes between ``1`` and ``10`` sampled from the Graph.
 
         Args:
             mask: An optional tuple of optional node and edge mask that is only possible with Discrete spaces
                 (Box spaces don't support sample masks).
-                If no `num_edges` is provided then the `edge_mask` is multiplied by the number of edges
-            num_nodes: The number of nodes that will be sampled, the default is 10 nodes
-            num_edges: An optional number of edges, otherwise, a random number between 0 and `num_nodes` ^ 2
+                If no ``num_edges`` is provided then the ``edge_mask`` is multiplied by the number of edges
+            num_nodes: The number of nodes that will be sampled, the default is `10` nodes
+            num_edges: An optional number of edges, otherwise, a random number between `0` and :math:`num_nodes^2`
 
         Returns:
             A :class:`GraphInstance` with attributes `.nodes`, `.edges`, and `.edge_links`.
         """
         assert (
             num_nodes > 0
         ), f"The number of nodes is expected to be greater than 0, actual value: {num_nodes}"
@@ -208,15 +208,15 @@
                     else:
                         return x.edges is None and x.edge_links is None
         return False
 
     def __repr__(self) -> str:
         """A string representation of this space.
 
-        The representation will include node_space and edge_space
+        The representation will include ``node_space`` and ``edge_space``
 
         Returns:
             A representation of the space
         """
         return f"Graph({self.node_space}, {self.edge_space})"
 
     def __eq__(self, other: Any) -> bool:
```

### Comparing `gymnasium-0.29.1/gymnasium/spaces/multi_binary.py` & `gymnasium-1.0.0a1/gymnasium/spaces/multi_binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,16 @@
     def sample(self, mask: MaskNDArray | None = None) -> NDArray[np.int8]:
         """Generates a single random sample from this space.
 
         A sample is drawn by independent, fair coin tosses (one toss per binary variable of the space).
 
         Args:
             mask: An optional np.ndarray to mask samples with expected shape of ``space.shape``.
-                For mask == 0 then the samples will be 0 and mask == 1 then random samples will be generated.
-                The expected mask shape is the space shape and mask dtype is `np.int8`.
+                For ``mask == 0`` then the samples will be ``0`` and ``mask == 1` then random samples will be generated.
+                The expected mask shape is the space shape and mask dtype is ``np.int8``.
 
         Returns:
             Sampled values from space
         """
         if mask is not None:
             assert isinstance(
                 mask, np.ndarray
```

### Comparing `gymnasium-0.29.1/gymnasium/spaces/multi_discrete.py` & `gymnasium-1.0.0a1/gymnasium/spaces/multi_discrete.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,20 +83,20 @@
 
     def sample(
         self, mask: tuple[MaskNDArray, ...] | None = None
     ) -> NDArray[np.integer[Any]]:
         """Generates a single random sample this space.
 
         Args:
-            mask: An optional mask for multi-discrete, expects tuples with a `np.ndarray` mask in the position of each
-                action with shape `(n,)` where `n` is the number of actions and `dtype=np.int8`.
-                Only mask values == 1 are possible to sample unless all mask values for an action are 0 then the default action `self.start` (the smallest element) is sampled.
+            mask: An optional mask for multi-discrete, expects tuples with a ``np.ndarray`` mask in the position of each
+                action with shape ``(n,)`` where ``n`` is the number of actions and ``dtype=np.int8``.
+                Only ``mask values == 1`` are possible to sample unless all mask values for an action are ``0`` then the default action ``self.start`` (the smallest element) is sampled.
 
         Returns:
-            An `np.ndarray` of shape `space.shape`
+            An ``np.ndarray`` of :meth:`Space.shape`
         """
         if mask is not None:
 
             def _apply_mask(
                 sub_mask: MaskNDArray | tuple[MaskNDArray, ...],
                 sub_nvec: MaskNDArray | np.integer[Any],
                 sub_start: MaskNDArray | np.integer[Any],
@@ -202,14 +202,15 @@
             )
         return len(self.nvec)
 
     def __eq__(self, other: Any) -> bool:
         """Check whether ``other`` is equivalent to this instance."""
         return bool(
             isinstance(other, MultiDiscrete)
+            and self.dtype == other.dtype
             and np.all(self.nvec == other.nvec)
             and np.all(self.start == other.start)
         )
 
     def __setstate__(self, state: Iterable[tuple[str, Any]] | Mapping[str, Any]):
         """Used when loading a pickled space.
```

### Comparing `gymnasium-0.29.1/gymnasium/spaces/sequence.py` & `gymnasium-1.0.0a1/gymnasium/spaces/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         stack: bool = False,
     ):
         """Constructor of the :class:`Sequence` space.
 
         Args:
             space: Elements in the sequences this space represent must belong to this space.
             seed: Optionally, you can use this argument to seed the RNG that is used to sample from the space.
-            stack: If `True` then the resulting samples would be stacked.
+            stack: If ``True`` then the resulting samples would be stacked.
         """
         assert isinstance(
             space, Space
         ), f"Expects the feature space to be instance of a gym Space, actual type: {type(space)}"
         self.feature_space = space
         self.stack = stack
         if self.stack:
@@ -74,22 +74,21 @@
             ]
         ) = None,
     ) -> tuple[Any] | Any:
         """Generates a single random sample from this space.
 
         Args:
             mask: An optional mask for (optionally) the length of the sequence and (optionally) the values in the sequence.
-                If you specify `mask`, it is expected to be a tuple of the form `(length_mask, sample_mask)` where `length_mask`
-                is
+                If you specify ``mask``, it is expected to be a tuple of the form ``(length_mask, sample_mask)`` where ``length_mask`` is
 
                 * ``None`` The length will be randomly drawn from a geometric distribution
                 * ``np.ndarray`` of integers, in which case the length of the sampled sequence is randomly drawn from this array.
                 * ``int`` for a fixed length sample
 
-                The second element of the mask tuple `sample` mask specifies a mask that is applied when
+                The second element of the mask tuple ``sample`` mask specifies a mask that is applied when
                 sampling elements from the base space. The mask is applied for each feature space sample.
 
         Returns:
             A tuple of random length with random samples of elements from the :attr:`feature_space`.
         """
         if mask is not None:
             length_mask, feature_mask = mask
```

### Comparing `gymnasium-0.29.1/gymnasium/spaces/space.py` & `gymnasium-1.0.0a1/gymnasium/spaces/space.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     Different spaces can be combined hierarchically via container spaces (:class:`Tuple` and :class:`Dict`) to build a
     more expressive space
 
     Warning:
         Custom observation & action spaces can inherit from the ``Space``
         class. However, most use-cases should be covered by the existing space
-        classes (e.g. :class:`Box`, :class:`Discrete`, etc...), and container classes (:class`Tuple` &
+        classes (e.g. :class:`Box`, :class:`Discrete`, etc...), and container classes (:class:`Tuple` &
         :class:`Dict`). Note that parametrized probability distributions (through the
         :meth:`Space.sample()` method), and batching functions (in :class:`gym.vector.VectorEnv`), are
         only well-defined for instances of spaces provided in gym by default.
         Moreover, some implementations of Reinforcement Learning algorithms might
         not handle custom spaces properly. Use custom spaces with care.
     """
```

### Comparing `gymnasium-0.29.1/gymnasium/spaces/text.py` & `gymnasium-1.0.0a1/gymnasium/spaces/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,21 +74,21 @@
         # As the shape is dynamic (between min_length and max_length) then None
         super().__init__(dtype=str, seed=seed)
 
     def sample(
         self,
         mask: None | (tuple[int | None, NDArray[np.int8] | None]) = None,
     ) -> str:
-        """Generates a single random sample from this space with by default a random length between `min_length` and `max_length` and sampled from the `charset`.
+        """Generates a single random sample from this space with by default a random length between ``min_length`` and ``max_length`` and sampled from the ``charset``.
 
         Args:
             mask: An optional tuples of length and mask for the text.
-                The length is expected to be between the `min_length` and `max_length` otherwise a random integer between `min_length` and `max_length` is selected.
-                For the mask, we expect a numpy array of length of the charset passed with `dtype == np.int8`.
-                If the charlist mask is all zero then an empty string is returned no matter the `min_length`
+                The length is expected to be between the ``min_length`` and ``max_length`` otherwise a random integer between ``min_length`` and ``max_length`` is selected.
+                For the mask, we expect a numpy array of length of the charset passed with ``dtype == np.int8``.
+                If the charlist mask is all zero then an empty string is returned no matter the ``min_length``
 
         Returns:
             A sampled string from the space
         """
         if mask is not None:
             assert isinstance(
                 mask, tuple
```

### Comparing `gymnasium-0.29.1/gymnasium/spaces/tuple.py` & `gymnasium-1.0.0a1/gymnasium/spaces/tuple.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 
     def seed(self, seed: int | typing.Sequence[int] | None = None) -> list[int]:
         """Seed the PRNG of this space and all subspaces.
 
         Depending on the type of seed, the subspaces will be seeded differently
 
         * ``None`` - All the subspaces will use a random initial seed
-        * ``Int`` - The integer is used to seed the `Tuple` space that is used to generate seed values for each of the subspaces. Warning, this does not guarantee unique seeds for all of the subspaces.
-        * ``List`` - Values used to seed the subspaces. This allows the seeding of multiple composite subspaces (``List(42, 54, ...``).
+        * ``Int`` - The integer is used to seed the :class:`Tuple` space that is used to generate seed values for each of the subspaces. Warning, this does not guarantee unique seeds for all the subspaces.
+        * ``List`` - Values used to seed the subspaces. This allows the seeding of multiple composite subspaces ``[42, 54, ...]``.
 
         Args:
             seed: An optional list of ints or int to seed the (sub-)spaces.
         """
         seeds: list[int] = []
 
         if isinstance(seed, collections.abc.Sequence):
```

### Comparing `gymnasium-0.29.1/gymnasium/spaces/utils.py` & `gymnasium-1.0.0a1/gymnasium/spaces/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,42 +424,41 @@
 
     Returns:
         A flattened Box
 
     Raises:
         NotImplementedError: if the space is not defined in :mod:`gymnasium.spaces`.
 
-    Example:
-        Flatten spaces.Box:
+    Example - Flatten spaces.Box:
         >>> from gymnasium.spaces import Box
         >>> box = Box(0.0, 1.0, shape=(3, 4, 5))
         >>> box
         Box(0.0, 1.0, (3, 4, 5), float32)
         >>> flatten_space(box)
         Box(0.0, 1.0, (60,), float32)
         >>> flatten(box, box.sample()) in flatten_space(box)
         True
 
-        Flatten spaces.Discrete:
+    Example - Flatten spaces.Discrete:
         >>> from gymnasium.spaces import Discrete
         >>> discrete = Discrete(5)
         >>> flatten_space(discrete)
         Box(0, 1, (5,), int64)
         >>> flatten(discrete, discrete.sample()) in flatten_space(discrete)
         True
 
-        Flatten spaces.Dict:
+    Example - Flatten spaces.Dict:
         >>> from gymnasium.spaces import Dict, Discrete, Box
         >>> space = Dict({"position": Discrete(2), "velocity": Box(0, 1, shape=(2, 2))})
         >>> flatten_space(space)
         Box(0.0, 1.0, (6,), float64)
         >>> flatten(space, space.sample()) in flatten_space(space)
         True
 
-        Flatten spaces.Graph:
+    Example - Flatten spaces.Graph:
         >>> from gymnasium.spaces import Graph, Discrete, Box
         >>> space = Graph(node_space=Box(low=-100, high=100, shape=(3, 4)), edge_space=Discrete(5))
         >>> flatten_space(space)
         Graph(Box(-100.0, 100.0, (12,), float32), Box(0, 1, (5,), int64))
         >>> flatten(space, space.sample()) in flatten_space(space)
         True
     """
```

### Comparing `gymnasium-0.29.1/gymnasium/utils/__init__.py` & `gymnasium-1.0.0a1/gymnasium/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/utils/colorize.py` & `gymnasium-1.0.0a1/gymnasium/utils/colorize.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/utils/env_checker.py` & `gymnasium-1.0.0a1/gymnasium/utils/env_checker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""A set of functions for checking an environment details.
+"""A set of functions for checking an environment implementation.
 
 This file is originally from the Stable Baselines3 repository hosted on GitHub
 (https://github.com/DLR-RM/stable-baselines3/)
 Original Author: Antonin Raffin
 
 It also uses some warnings/assertions from the PettingZoo repository hosted on GitHub
 (https://github.com/PettingZoo-Team/PettingZoo)
@@ -36,15 +36,15 @@
     Args:
         data_1: data structure 1
         data_2: data structure 2
 
     Returns:
         If observation 1 and 2 are equivalent
     """
-    if type(data_1) == type(data_2):
+    if type(data_1) is type(data_2):
         if isinstance(data_1, dict):
             return data_1.keys() == data_2.keys() and all(
                 data_equivalence(data_1[k], data_2[k]) for k in data_1.keys()
             )
         elif isinstance(data_1, (tuple, list)):
             return len(data_1) == len(data_2) and all(
                 data_equivalence(o_1, o_2) for o_1, o_2 in zip(data_1, data_2)
@@ -223,15 +223,15 @@
     if isinstance(space, spaces.Box):
         if np.any(np.equal(space.low, -np.inf)):
             logger.warn(
                 f"A Box {space_type} space minimum value is -infinity. This is probably too low."
             )
         if np.any(np.equal(space.high, np.inf)):
             logger.warn(
-                f"A Box {space_type} space maximum value is -infinity. This is probably too high."
+                f"A Box {space_type} space maximum value is infinity. This is probably too high."
             )
 
         # Check that the Box space is normalized
         if space_type == "action":
             if len(space.shape) == 1:  # for vector boxes
                 if (
                     np.any(
@@ -252,27 +252,34 @@
         for subspace in space.spaces:
             check_space_limit(subspace, space_type)
     elif isinstance(space, spaces.Dict):
         for subspace in space.values():
             check_space_limit(subspace, space_type)
 
 
-def check_env(env: gym.Env, warn: bool = None, skip_render_check: bool = False):
-    """Check that an environment follows Gym API.
+def check_env(
+    env: gym.Env,
+    warn: bool = None,
+    skip_render_check: bool = False,
+    skip_close_check: bool = False,
+):
+    """Check that an environment follows Gymnasium's API.
 
-    This is an invasive function that calls the environment's reset and step.
+    .. py:currentmodule:: gymnasium.Env
 
-    This is particularly useful when using a custom environment.
-    Please take a look at https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/
-    for more information about the API.
+    To ensure that an environment is implemented "correctly", ``check_env`` checks that the :attr:`observation_space` and :attr:`action_space` are correct.
+    Furthermore, the function will call the :meth:`reset`, :meth:`step` and :meth:`render` functions with a variety of values.
+
+    We highly recommend users calling this function after an environment is constructed and within a projects continuous integration to keep an environment update with Gymnasium's API.
 
     Args:
         env: The Gym environment that will be checked
-        warn: Ignored
-        skip_render_check: Whether to skip the checks for the render method. True by default (useful for the CI)
+        warn: Ignored, previously silenced particular warnings
+        skip_render_check: Whether to skip the checks for the render method. False by default (useful for the CI)
+        skip_close_check: Whether to skip the checks for the close method. False by default
     """
     if warn is not None:
         logger.warn("`check_env(warn=...)` parameter is now ignored.")
 
     assert isinstance(
         env, gym.Env
     ), "The environment must inherit from the gymnasium.Env class. See https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/ for more info."
@@ -318,15 +325,15 @@
                 env_render_passive_checker(new_env)
                 new_env.close()
         else:
             logger.warn(
                 "Not able to test alternative render modes due to the environment not having a spec. Try instantialising the environment through gymnasium.make"
             )
 
-    if env.spec is not None:
+    if not skip_close_check and env.spec is not None:
         new_env = env.spec.make()
         new_env.close()
         try:
             new_env.close()
         except Exception as e:
             logger.warn(
                 f"Calling `env.close()` on the closed environment should be allowed, but it raised an exception: {e}"
```

### Comparing `gymnasium-0.29.1/gymnasium/utils/env_match.py` & `gymnasium-1.0.0a1/gymnasium/utils/env_match.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,35 +9,43 @@
     env_b: gym.Env,
     num_steps: int,
     seed: int = 0,
     skip_obs: bool = False,
     skip_rew: bool = False,
     skip_terminal: bool = False,
     skip_truncated: bool = False,
+    skip_render: bool = False,
     info_comparison: str = "equivalence",
 ):
     """Checks if the environments `env_a` & `env_b` are identical.
 
     Args:
         env_a: First environment to check.
         env_b: Second environment to check.
         num_steps: number of timesteps to test for, setting to 0 tests only resetting.
         seed: used the seed the reset & actions.
         skip_obs: If `True` it does not check for equivalence of the observation.
         skip_rew: If `True` it does not check for equivalence of the observation.
         skip_terminal: If `True` it does not check for equivalence of the observation.
         skip_truncated: If `True` it does not check for equivalence of the observation.
         skip_info: If `True` it does not check for equivalence of the observation.
+        skip_render: If `True` it does not check for equivalent renders. note:the render checked are automatically skipped if `render_mode` is not set or is "human".
         info_comparison: The options are
             If "equivalence" then checks if the `info`s are identical,
             If "superset" checks if `info_b` is a (non-strict) superset of `info_a`
             If "keys-equivalence" checks if the `info`s keys are identical (while ignoring the values).
             If "keys-superset" checks if the `info_b`s keys are a superset of `info_a`'s keys.
             If "skip" no checks are made at the `info`.
     """
+    skip_render = (
+        skip_render
+        or env_a.unwrapped.render_mode in [None, "human"]
+        or env_b.unwrapped.render in [None, "human"]
+    )
+
     assert info_comparison in [
         "equivalence",
         "superset",
         "skip",
         "keys-equivalence",
         "keys-superset",
     ]
@@ -47,75 +55,96 @@
 
     env_a.action_space.seed(seed)
     obs_a, info_a = env_a.reset(seed=seed)
     obs_b, info_b = env_b.reset(seed=seed)
 
     assert skip_obs or data_equivalence(
         obs_a, obs_b
-    ), "resetting observation is not equivalent"
+    ), f"resetting observation is not equivalent, observation_a = {obs_a}, observation_b = {obs_b}"
     if info_comparison == "equivalence":
-        assert data_equivalence(info_a, info_b), "resetting info is not equivalent"
+        assert data_equivalence(
+            info_a, info_b
+        ), f"resetting info is not equivalent, info_a = {info_a}, info_b = {info_b}"
     elif info_comparison == "superset":
         for key in info_a:
             assert data_equivalence(
                 info_a[key], info_b[key]
-            ), "resetting info is not a superset"
+            ), f"resetting info is not a superset, key {key} present in info_a with value = {info_a[key]}, in info_b with value = {info_b[key]}"
     elif info_comparison == "keys-equivalance":
-        assert info_a.keys() == info_b.keys(), "resetting info keys are not equivalent"
+        assert (
+            info_a.keys() == info_b.keys()
+        ), f"resetting info keys are not equivalent, info_a's keys are {info_a.keys()}, info_b's keys are {info_b.keys()}"
     elif info_comparison == "keys-superset":
-        assert info_b.keys() >= info_a.keys(), "resetting info keys are not a superset"
+        assert (
+            info_b.keys() >= info_a.keys()
+        ), f"resetting info keys are not a superset, keys not present in info_b are: {info_b.keys() - info_a.keys()}"
+
+    if not skip_render:
+        assert (
+            env_a.render() == env_b.render()
+        ).all(), "resetting render is not equivalent"
 
-    for _ in range(num_steps):
+    for step in range(num_steps):
         action = env_a.action_space.sample()
         obs_a, rew_a, terminal_a, truncated_a, info_a = env_a.step(action)
         obs_b, rew_b, terminal_b, truncated_b, info_b = env_b.step(action)
         assert skip_obs or data_equivalence(
             obs_a, obs_b
-        ), "stepping observation is not equivalent"
+        ), f"stepping observation is not equivalent in step = {step}, observation_a = {obs_a}, observation_b = {obs_b}"
         assert skip_rew or data_equivalence(
             rew_a, rew_b
-        ), "stepping reward is not equivalent"
+        ), f"stepping reward is not equivalent in step = {step}, reward_a = {rew_a}, reward_b = {rew_b}"
         assert (
             skip_terminal or terminal_a == terminal_b
-        ), "stepping terminal is not equivalent"
+        ), f"stepping terminal is not equivalent in step = {step}, terminal_a = {terminal_a}, terminal_b = {terminal_b}"
         assert (
             skip_truncated or truncated_a == truncated_b
-        ), "stepping truncated is not equivalent"
+        ), f"stepping truncated is not equivalent in step = {step}, truncated_a = {truncated_a}, truncated_b = {truncated_b}"
         if info_comparison == "equivalence":
-            assert data_equivalence(info_a, info_b), "stepping info is not equivalent"
+            assert data_equivalence(
+                info_a, info_b
+            ), f"stepping info is not equivalent in step = {step}, info_a = {info_a}, info_b = {info_b}"
         elif info_comparison == "superset":
             for key in info_a:
                 assert data_equivalence(
                     info_a[key], info_b[key]
-                ), "stepping info is not a superset"
+                ), f"stepping info is not a superset in step = {step}, key {key} present in info_a with value = {info_a[key]}, in info_b with value = {info_b[key]}"
         elif info_comparison == "keys-equivalance":
             assert (
                 info_a.keys() == info_b.keys()
-            ), "stepping info keys are not equivalent"
+            ), f"stepping info keys are not equivalent in step = {step}, info_a's keys are {info_a.keys()}, info_b's keys are {info_b.keys()}"
         elif info_comparison == "keys-superset":
             assert (
                 info_b.keys() >= info_a.keys()
-            ), "stepping info keys are not a superset"
+            ), f"stepping info keys are not a superset in step = {step}, keys not present in info_b are: {info_b.keys() - info_a.keys()}"
+        if not skip_render:
+            assert (
+                env_a.render() == env_b.render()
+            ).all(), "stepping render is not equivalent in step = {step}"
 
         if terminal_a or truncated_a or terminal_b or truncated_b:
             obs_a, info_a = env_a.reset(seed=seed)
             obs_b, info_b = env_b.reset(seed=seed)
             assert skip_obs or data_equivalence(
                 obs_a, obs_b
-            ), "resetting observation is not equivalent"
+            ), f"resetting observation is not equivalent in step = {step}, observation_a = {obs_a}, observation_b = {obs_b}"
             if info_comparison == "equivalence":
                 assert data_equivalence(
                     info_a, info_b
-                ), "resetting info is not equivalent"
+                ), f"resetting info is not equivalent in step = {step}, info_a = {info_a}, info_b = {info_b}"
             elif info_comparison == "superset":
                 for key in info_a:
                     assert data_equivalence(
                         info_a[key], info_b[key]
-                    ), "resetting info is not a superset"
+                    ), f"resetting info is not a superset in step = {step}, key {key} present in info_a with value = {info_a[key]}, in info_b with value = {info_b[key]}"
             elif info_comparison == "keys-equivalance":
                 assert (
                     info_a.keys() == info_b.keys()
-                ), "resetting info keys are not equivalent"
+                ), f"resetting info keys are not equivalent in step = {step}, info_a's keys are {info_a.keys()}, info_b's keys are {info_b.keys()}"
             elif info_comparison == "keys-superset":
                 assert (
                     info_b.keys() >= info_a.keys()
-                ), "resetting info keys are not a superset"
+                ), f"resetting info keys are not a superset in step = {step}, keys not present in info_b are: {info_b.keys() - info_a.keys()}"
+            if not skip_render:
+                assert (
+                    env_a.render() == env_b.render()
+                ).all(), "resetting render is not equivalent in step = {step}"
```

### Comparing `gymnasium-0.29.1/gymnasium/utils/ezpickle.py` & `gymnasium-1.0.0a1/gymnasium/utils/ezpickle.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/utils/passive_env_checker.py` & `gymnasium-1.0.0a1/gymnasium/utils/passive_env_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from gymnasium import Space, error, logger, spaces
 
 
 __all__ = [
     "env_render_passive_checker",
     "env_reset_passive_checker",
     "env_step_passive_checker",
+    "check_action_space",
+    "check_observation_space",
 ]
 
 
 def _check_box_observation_space(observation_space: spaces.Box):
     """Checks that a :class:`Box` observation space is defined in a sensible way.
 
     Args:
```

### Comparing `gymnasium-0.29.1/gymnasium/utils/performance.py` & `gymnasium-1.0.0a1/gymnasium/utils/performance.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/utils/play.py` & `gymnasium-1.0.0a1/gymnasium/utils/play.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Utilities of visualising an environment."""
+from __future__ import annotations
+
 from collections import deque
-from typing import Callable, Dict, List, Optional, Tuple, Union
+from typing import Callable, List
 
 import numpy as np
 
 import gymnasium as gym
 from gymnasium import Env, logger
 from gymnasium.core import ActType, ObsType
 from gymnasium.error import DependencyNotInstalled
-from gymnasium.logger import deprecation
 
 
 try:
     import pygame
     from pygame import Surface
     from pygame.event import Event
 except ImportError as e:
@@ -36,16 +37,16 @@
 
 class PlayableGame:
     """Wraps an environment allowing keyboard inputs to interact with the environment."""
 
     def __init__(
         self,
         env: Env,
-        keys_to_action: Optional[Dict[Tuple[int, ...], int]] = None,
-        zoom: Optional[float] = None,
+        keys_to_action: dict[tuple[int, ...], int] | None = None,
+        zoom: float | None = None,
     ):
         """Wraps an environment with a dictionary of keyboard buttons to action and if to zoom in on the environment.
 
         Args:
             env: The environment to play
             keys_to_action: The dictionary of keyboard tuples and action value
             zoom: If to zoom in on the environment render
@@ -62,15 +63,15 @@
         # The window size may be larger, in that case we will add black bars
         self.video_size = self._get_video_size(zoom)
         self.screen = pygame.display.set_mode(self.video_size, pygame.RESIZABLE)
         self.pressed_keys = []
         self.running = True
 
     def _get_relevant_keys(
-        self, keys_to_action: Optional[Dict[Tuple[int], int]] = None
+        self, keys_to_action: dict[tuple[int], int] | None = None
     ) -> set:
         if keys_to_action is None:
             if hasattr(self.env, "get_keys_to_action"):
                 keys_to_action = self.env.get_keys_to_action()
             elif hasattr(self.env.unwrapped, "get_keys_to_action"):
                 keys_to_action = self.env.unwrapped.get_keys_to_action()
             else:
@@ -79,15 +80,15 @@
                     f"{self.env.spec.id} does not have explicit key to action mapping, "
                     "please specify one manually"
                 )
         assert isinstance(keys_to_action, dict)
         relevant_keys = set(sum((list(k) for k in keys_to_action.keys()), []))
         return relevant_keys
 
-    def _get_video_size(self, zoom: Optional[float] = None) -> Tuple[int, int]:
+    def _get_video_size(self, zoom: float | None = None) -> tuple[int, int]:
         rendered = self.env.render()
         if isinstance(rendered, List):
             rendered = rendered[-1]
         assert rendered is not None and isinstance(rendered, np.ndarray)
         video_size = (rendered.shape[1], rendered.shape[0])
 
         if zoom is not None:
@@ -119,15 +120,15 @@
             scale_width = event.x / self.video_size[0]
             scale_height = event.y / self.video_size[1]
             scale = min(scale_height, scale_width)
             self.video_size = (scale * self.video_size[0], scale * self.video_size[1])
 
 
 def display_arr(
-    screen: Surface, arr: np.ndarray, video_size: Tuple[int, int], transpose: bool
+    screen: Surface, arr: np.ndarray, video_size: tuple[int, int], transpose: bool
 ):
     """Displays a numpy array on screen.
 
     Args:
         screen: The screen to show the array on
         arr: The array to show
         video_size: The video size of the screen
@@ -143,38 +144,39 @@
     height_offset = (surface_size[1] - video_size[1]) / 2
     screen.fill((0, 0, 0))
     screen.blit(pyg_img, (width_offset, height_offset))
 
 
 def play(
     env: Env,
-    transpose: Optional[bool] = True,
-    fps: Optional[int] = None,
-    zoom: Optional[float] = None,
-    callback: Optional[Callable] = None,
-    keys_to_action: Optional[Dict[Union[Tuple[Union[str, int]], str], ActType]] = None,
-    seed: Optional[int] = None,
+    transpose: bool | None = True,
+    fps: int | None = None,
+    zoom: float | None = None,
+    callback: Callable | None = None,
+    keys_to_action: dict[tuple[str | int] | str, ActType] | None = None,
+    seed: int | None = None,
     noop: ActType = 0,
 ):
-    """Allows one to play the game using keyboard.
+    """Allows the user to play the environment using a keyboard.
 
     Args:
         env: Environment to use for playing.
         transpose: If this is ``True``, the output of observation is transposed. Defaults to ``True``.
         fps: Maximum number of steps of the environment executed every second. If ``None`` (the default),
             ``env.metadata["render_fps""]`` (or 30, if the environment does not specify "render_fps") is used.
         zoom: Zoom the observation in, ``zoom`` amount, should be positive float
         callback: If a callback is provided, it will be executed after every step. It takes the following input:
-                obs_t: observation before performing action
-                obs_tp1: observation after performing action
-                action: action that was executed
-                rew: reward that was received
-                terminated: whether the environment is terminated or not
-                truncated: whether the environment is truncated or not
-                info: debug info
+
+            * obs_t: observation before performing action
+            * obs_tp1: observation after performing action
+            * action: action that was executed
+            * rew: reward that was received
+            * terminated: whether the environment is terminated or not
+            * truncated: whether the environment is truncated or not
+            * info: debug info
         keys_to_action:  Mapping from keys pressed to action performed.
             Different formats are supported: Key combinations can either be expressed as a tuple of unicode code
             points of the keys, as a tuple of characters, or as a string where each character of the string represents
             one key.
             For example if pressing 'w' and space at the same time is supposed
             to trigger action number 2 then ``key_to_action`` dict could look like this:
 
@@ -201,36 +203,37 @@
                 ... }
 
             If ``None``, default ``key_to_action`` mapping for that environment is used, if provided.
         seed: Random seed used when resetting the environment. If None, no seed is used.
         noop: The action used when no key input has been entered, or the entered key combination is unknown.
 
     Example:
-        >>> import gymnasium as gym
         >>> from gymnasium.utils.play import play
-        >>> play(gym.make("CarRacing-v2", render_mode="rgb_array"), keys_to_action={  # doctest: +SKIP
-        ...                                                "w": np.array([0, 0.7, 0]),
-        ...                                                "a": np.array([-1, 0, 0]),
-        ...                                                "s": np.array([0, 0, 1]),
-        ...                                                "d": np.array([1, 0, 0]),
-        ...                                                "wa": np.array([-1, 0.7, 0]),
-        ...                                                "dw": np.array([1, 0.7, 0]),
-        ...                                                "ds": np.array([1, 0, 1]),
-        ...                                                "as": np.array([-1, 0, 1]),
-        ...                                               }, noop=np.array([0,0,0]))
+        >>> play(gym.make("CarRacing-v2", render_mode="rgb_array"),  # doctest: +SKIP
+        ...     keys_to_action={
+        ...         "w": np.array([0, 0.7, 0]),
+        ...         "a": np.array([-1, 0, 0]),
+        ...         "s": np.array([0, 0, 1]),
+        ...         "d": np.array([1, 0, 0]),
+        ...         "wa": np.array([-1, 0.7, 0]),
+        ...         "dw": np.array([1, 0.7, 0]),
+        ...         "ds": np.array([1, 0, 1]),
+        ...         "as": np.array([-1, 0, 1]),
+        ...     },
+        ...     noop=np.array([0, 0, 0])
+        ... )
 
         Above code works also if the environment is wrapped, so it's particularly useful in
         verifying that the frame-level preprocessing does not render the game
         unplayable.
 
         If you wish to plot real time statistics as you play, you can use
-        :class:`gym.utils.play.PlayPlot`. Here's a sample code for plotting the reward
+        :class:`PlayPlot`. Here's a sample code for plotting the reward
         for last 150 steps.
 
-        >>> import gymnasium as gym
         >>> from gymnasium.utils.play import PlayPlot, play
         >>> def callback(obs_t, obs_tp1, action, rew, terminated, truncated, info):
         ...        return [rew,]
         >>> plotter = PlayPlot(callback, 150, ["reward"])             # doctest: +SKIP
         >>> play(gym.make("CartPole-v1"), callback=plotter.callback)  # doctest: +SKIP
     """
     env.reset(seed=seed)
@@ -317,32 +320,29 @@
 
         >>> plotter = PlayPlot(compute_metrics, horizon_timesteps=200,                               # doctest: +SKIP
         ...                    plot_names=["Immediate Rew.", "Cumulative Rew.", "Action Magnitude"])
         >>> play(your_env, callback=plotter.callback)                                                # doctest: +SKIP
     """
 
     def __init__(
-        self, callback: Callable, horizon_timesteps: int, plot_names: List[str]
+        self, callback: Callable, horizon_timesteps: int, plot_names: list[str]
     ):
         """Constructor of :class:`PlayPlot`.
 
         The function ``callback`` that is passed to this constructor should return
         a list of metrics that is of length ``len(plot_names)``.
 
         Args:
             callback: Function that computes metrics from environment transitions
             horizon_timesteps: The time horizon used for the live plots
             plot_names: List of plot titles
 
         Raises:
             DependencyNotInstalled: If matplotlib is not installed
         """
-        deprecation(
-            "`PlayPlot` is marked as deprecated and will be removed in the near future."
-        )
         self.data_callback = callback
         self.horizon_timesteps = horizon_timesteps
         self.plot_names = plot_names
 
         if plt is None:
             raise DependencyNotInstalled(
                 "matplotlib is not installed, run `pip install gymnasium[other]`"
@@ -351,15 +351,15 @@
         num_plots = len(self.plot_names)
         self.fig, self.ax = plt.subplots(num_plots)
         if num_plots == 1:
             self.ax = [self.ax]
         for axis, name in zip(self.ax, plot_names):
             axis.set_title(name)
         self.t = 0
-        self.cur_plot: List[Optional[plt.Axes]] = [None for _ in range(num_plots)]
+        self.cur_plot: list[plt.Axes | None] = [None for _ in range(num_plots)]
         self.data = [deque(maxlen=horizon_timesteps) for _ in range(num_plots)]
 
     def callback(
         self,
         obs_t: ObsType,
         obs_tp1: ObsType,
         action: ActType,
```

### Comparing `gymnasium-0.29.1/gymnasium/utils/record_constructor.py` & `gymnasium-1.0.0a1/gymnasium/utils/record_constructor.py`

 * *Files identical despite different names*

### Comparing `gymnasium-0.29.1/gymnasium/utils/save_video.py` & `gymnasium-1.0.0a1/gymnasium/utils/save_video.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Utility functions to save rendering videos."""
+from __future__ import annotations
+
 import os
-from typing import Callable, Optional
+from typing import Callable
 
 import gymnasium as gym
 from gymnasium import logger
 
 
 try:
     from moviepy.video.io.ImageSequenceClip import ImageSequenceClip
 except ImportError as e:
     raise gym.error.DependencyNotInstalled(
         "moviepy is not installed, run `pip install moviepy`"
     ) from e
 
 
 def capped_cubic_video_schedule(episode_id: int) -> bool:
-    """The default episode trigger.
+    r"""The default episode trigger.
 
-    This function will trigger recordings at the episode indices 0, 1, 4, 8, 27, ..., :math:`k^3`, ..., 729, 1000, 2000, 3000, ...
+    This function will trigger recordings at the episode indices :math:`\{0, 1, 4, 8, 27, ..., k^3, ..., 729, 1000, 2000, 3000, ...\}`
 
     Args:
         episode_id: The episode number
 
     Returns:
         If to apply a video schedule number
     """
@@ -32,18 +34,19 @@
 
 
 def save_video(
     frames: list,
     video_folder: str,
     episode_trigger: Callable[[int], bool] = None,
     step_trigger: Callable[[int], bool] = None,
-    video_length: Optional[int] = None,
+    video_length: int | None = None,
     name_prefix: str = "rl-video",
     episode_index: int = 0,
     step_starting_index: int = 0,
+    save_logger: str | None = None,
     **kwargs,
 ):
     """Save videos from rendering frames.
 
     This function extract video from a list of render frame episodes.
 
     Args:
@@ -52,14 +55,15 @@
         episode_trigger: Function that accepts an integer and returns ``True`` iff a recording should be started at this episode
         step_trigger: Function that accepts an integer and returns ``True`` iff a recording should be started at this step
         video_length (int): The length of recorded episodes. If it isn't specified, the entire episode is recorded.
             Otherwise, snippets of the specified length are captured.
         name_prefix (str): Will be prepended to the filename of the recordings.
         episode_index (int): The index of the current episode.
         step_starting_index (int): The step index of the first frame.
+        save_logger: If to log the video saving progress, helpful for long videos that take a while, use "bar" to enable.
         **kwargs: The kwargs that will be passed to moviepy's ImageSequenceClip.
             You need to specify either fps or duration.
 
     Example:
         >>> import gymnasium as gym
         >>> from gymnasium.utils.save_video import save_video
         >>> env = gym.make("FrozenLake-v1", render_mode="rgb_array_list")
@@ -68,16 +72,16 @@
         >>> episode_index = 0
         >>> for step_index in range(199): # doctest: +SKIP
         ...    action = env.action_space.sample()
         ...    _, _, terminated, truncated, _ = env.step(action)
         ...
         ...    if terminated or truncated:
         ...       save_video(
-        ...          env.render(),
-        ...          "videos",
+        ...          frames=env.render(),
+        ...          video_folder="videos",
         ...          fps=env.metadata["render_fps"],
         ...          step_starting_index=step_starting_index,
         ...          episode_index=episode_index
         ...       )
         ...       step_starting_index = step_index + 1
         ...       episode_index += 1
         ...       env.reset()
@@ -90,20 +94,24 @@
 
     video_folder = os.path.abspath(video_folder)
     os.makedirs(video_folder, exist_ok=True)
     path_prefix = f"{video_folder}/{name_prefix}"
 
     if episode_trigger is not None and episode_trigger(episode_index):
         clip = ImageSequenceClip(frames[:video_length], **kwargs)
-        clip.write_videofile(f"{path_prefix}-episode-{episode_index}.mp4")
+        clip.write_videofile(
+            f"{path_prefix}-episode-{episode_index}.mp4", logger=save_logger
+        )
 
     if step_trigger is not None:
         # skip the first frame since it comes from reset
         for step_index, frame_index in enumerate(
             range(1, len(frames)), start=step_starting_index
         ):
             if step_trigger(step_index):
                 end_index = (
                     frame_index + video_length if video_length is not None else None
                 )
                 clip = ImageSequenceClip(frames[frame_index:end_index], **kwargs)
-                clip.write_videofile(f"{path_prefix}-step-{step_index}.mp4")
+                clip.write_videofile(
+                    f"{path_prefix}-step-{step_index}.mp4", logger=save_logger
+                )
```

### Comparing `gymnasium-0.29.1/gymnasium/utils/step_api_compatibility.py` & `gymnasium-1.0.0a1/gymnasium/utils/step_api_compatibility.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Contains methods for step compatibility, from old-to-new and new-to-old API."""
+from __future__ import annotations
+
 from typing import SupportsFloat, Tuple, Union
 
 import numpy as np
 
 from gymnasium.core import ObsType
 
 
@@ -19,21 +21,23 @@
     Union[bool, np.ndarray],
     Union[bool, np.ndarray],
     Union[dict, list],
 ]
 
 
 def convert_to_terminated_truncated_step_api(
-    step_returns: Union[DoneStepType, TerminatedTruncatedStepType], is_vector_env=False
+    step_returns: DoneStepType | TerminatedTruncatedStepType, is_vector_env=False
 ) -> TerminatedTruncatedStepType:
     """Function to transform step returns to new step API irrespective of input API.
 
+    .. py:currentmodule:: gymnasium.Env
+
     Args:
-        step_returns (tuple): Items returned by step(). Can be (obs, rew, done, info) or (obs, rew, terminated, truncated, info)
-        is_vector_env (bool): Whether the step_returns are from a vector environment
+        step_returns (tuple): Items returned by :meth:`step`. Can be ``(obs, rew, done, info)`` or ``(obs, rew, terminated, truncated, info)``
+        is_vector_env (bool): Whether the ``step_returns`` are from a vector environment
     """
     if len(step_returns) == 5:
         return step_returns
     else:
         assert len(step_returns) == 4
         observations, rewards, dones, infos = step_returns
 
@@ -71,22 +75,24 @@
         else:
             raise TypeError(
                 f"Unexpected value of infos, as is_vector_envs=False, expects `info` to be a list or dict, actual type: {type(infos)}"
             )
 
 
 def convert_to_done_step_api(
-    step_returns: Union[TerminatedTruncatedStepType, DoneStepType],
+    step_returns: TerminatedTruncatedStepType | DoneStepType,
     is_vector_env: bool = False,
 ) -> DoneStepType:
     """Function to transform step returns to old step API irrespective of input API.
 
+    .. py:currentmodule:: gymnasium.Env
+
     Args:
-        step_returns (tuple): Items returned by step(). Can be (obs, rew, done, info) or (obs, rew, terminated, truncated, info)
-        is_vector_env (bool): Whether the step_returns are from a vector environment
+        step_returns (tuple): Items returned by :meth:`step`. Can be ``(obs, rew, done, info)`` or ``(obs, rew, terminated, truncated, info)``
+        is_vector_env (bool): Whether the ``step_returns`` are from a vector environment
     """
     if len(step_returns) == 4:
         return step_returns
     else:
         assert len(step_returns) == 5
         observations, rewards, terminated, truncated, infos = step_returns
 
@@ -126,44 +132,47 @@
         else:
             raise TypeError(
                 f"Unexpected value of infos, as is_vector_envs=False, expects `info` to be a list or dict, actual type: {type(infos)}"
             )
 
 
 def step_api_compatibility(
-    step_returns: Union[TerminatedTruncatedStepType, DoneStepType],
+    step_returns: TerminatedTruncatedStepType | DoneStepType,
     output_truncation_bool: bool = True,
     is_vector_env: bool = False,
-) -> Union[TerminatedTruncatedStepType, DoneStepType]:
-    """Function to transform step returns to the API specified by `output_truncation_bool` bool.
+) -> TerminatedTruncatedStepType | DoneStepType:
+    """Function to transform step returns to the API specified by ``output_truncation_bool``.
 
-    Done (old) step API refers to step() method returning (observation, reward, done, info)
-    Terminated Truncated (new) step API refers to step() method returning (observation, reward, terminated, truncated, info)
+    .. py:currentmodule:: gymnasium.Env
+
+    Done (old) step API refers to :meth:`step` method returning ``(observation, reward, done, info)``
+    Terminated Truncated (new) step API refers to :meth:`step` method returning ``(observation, reward, terminated, truncated, info)``
     (Refer to docs for details on the API change)
 
     Args:
-        step_returns (tuple): Items returned by step(). Can be (obs, rew, done, info) or (obs, rew, terminated, truncated, info)
-        output_truncation_bool (bool): Whether the output should return two booleans (new API) or one (old) (True by default)
-        is_vector_env (bool): Whether the step_returns are from a vector environment
+        step_returns (tuple): Items returned by :meth:`step`. Can be ``(obs, rew, done, info)`` or ``(obs, rew, terminated, truncated, info)``
+        output_truncation_bool (bool): Whether the output should return two booleans (new API) or one (old) (``True`` by default)
+        is_vector_env (bool): Whether the ``step_returns`` are from a vector environment
 
     Returns:
-        step_returns (tuple): Depending on `output_truncation_bool` bool, it can return `(obs, rew, done, info)` or `(obs, rew, terminated, truncated, info)`
+        step_returns (tuple): Depending on ``output_truncation_bool``, it can return ``(obs, rew, done, info)`` or ``(obs, rew, terminated, truncated, info)``
 
     Example:
-        This function can be used to ensure compatibility in step interfaces with conflicting API. Eg. if env is written in old API,
-         wrapper is written in new API, and the final step output is desired to be in old API.
+        This function can be used to ensure compatibility in step interfaces with conflicting API. E.g. if env is written in old API,
+        wrapper is written in new API, and the final step output is desired to be in old API.
 
         >>> import gymnasium as gym
         >>> env = gym.make("CartPole-v0")
-        >>> _ = env.reset()
-        >>> obs, rewards, done, info = step_api_compatibility(env.step(0), output_truncation_bool=False)
-        >>> obs, rewards, terminated, truncated, info = step_api_compatibility(env.step(0), output_truncation_bool=True)
+        >>> _, _ = env.reset()
+        >>> obs, reward, done, info = step_api_compatibility(env.step(0), output_truncation_bool=False)
+        >>> obs, reward, terminated, truncated, info = step_api_compatibility(env.step(0), output_truncation_bool=True)
 
-        >>> vec_env = gym.vector.make("CartPole-v0")
-        >>> _ = vec_env.reset()
+        >>> vec_env = gym.make_vec("CartPole-v0", vectorization_mode="sync")
+        >>> _, _ = vec_env.reset()
         >>> obs, rewards, dones, infos = step_api_compatibility(vec_env.step([0]), is_vector_env=True, output_truncation_bool=False)
-        >>> obs, rewards, terminated, truncated, info = step_api_compatibility(vec_env.step([0]), is_vector_env=True, output_truncation_bool=True)
+        >>> obs, rewards, terminations, truncations, infos = step_api_compatibility(vec_env.step([0]), is_vector_env=True, output_truncation_bool=True)
+
     """
     if output_truncation_bool:
         return convert_to_terminated_truncated_step_api(step_returns, is_vector_env)
     else:
         return convert_to_done_step_api(step_returns, is_vector_env)
```

### Comparing `gymnasium-0.29.1/gymnasium/wrappers/env_checker.py` & `gymnasium-1.0.0a1/tests/testing_env.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,108 @@
-"""A passive environment checker wrapper for an environment's observation and action space along with the reset, step and render functions."""
+"""Provides a generic testing environment for use in tests with custom reset, step and render functions."""
 from __future__ import annotations
 
-from copy import deepcopy
-from typing import TYPE_CHECKING
+import types
+from collections.abc import Callable
+from typing import Any
 
 import gymnasium as gym
-from gymnasium import logger
-from gymnasium.core import ActType
-from gymnasium.utils.passive_env_checker import (
-    check_action_space,
-    check_observation_space,
-    env_render_passive_checker,
-    env_reset_passive_checker,
-    env_step_passive_checker,
-)
-
-
-if TYPE_CHECKING:
-    from gymnasium.envs.registration import EnvSpec
-
-
-class PassiveEnvChecker(gym.Wrapper, gym.utils.RecordConstructorArgs):
-    """A passive environment checker wrapper that surrounds the step, reset and render functions to check they follow the gymnasium API."""
-
-    def __init__(self, env):
-        """Initialises the wrapper with the environments, run the observation and action space tests."""
-        gym.utils.RecordConstructorArgs.__init__(self)
-        gym.Wrapper.__init__(self, env)
-
-        assert hasattr(
-            env, "action_space"
-        ), "The environment must specify an action space. https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/"
-        check_action_space(env.action_space)
-        assert hasattr(
-            env, "observation_space"
-        ), "The environment must specify an observation space. https://gymnasium.farama.org/tutorials/gymnasium_basics/environment_creation/"
-        check_observation_space(env.observation_space)
-
-        self.checked_reset = False
-        self.checked_step = False
-        self.checked_render = False
-        self.close_called = False
-
-    def step(self, action: ActType):
-        """Steps through the environment that on the first call will run the `passive_env_step_check`."""
-        if not self.checked_step:
-            self.checked_step = True
-            return env_step_passive_checker(self.env, action)
-        else:
-            return self.env.step(action)
-
-    def reset(self, **kwargs):
-        """Resets the environment that on the first call will run the `passive_env_reset_check`."""
-        if not self.checked_reset:
-            self.checked_reset = True
-            return env_reset_passive_checker(self.env, **kwargs)
-        else:
-            return self.env.reset(**kwargs)
-
-    def render(self, *args, **kwargs):
-        """Renders the environment that on the first call will run the `passive_env_render_check`."""
-        if not self.checked_render:
-            self.checked_render = True
-            return env_render_passive_checker(self.env, *args, **kwargs)
-        else:
-            return self.env.render(*args, **kwargs)
-
-    @property
-    def spec(self) -> EnvSpec | None:
-        """Modifies the environment spec to such that `disable_env_checker=False`."""
-        if self._cached_spec is not None:
-            return self._cached_spec
-
-        env_spec = self.env.spec
-        if env_spec is not None:
-            env_spec = deepcopy(env_spec)
-            env_spec.disable_env_checker = False
-
-        self._cached_spec = env_spec
-        return env_spec
-
-    def close(self):
-        """Warns if calling close on a closed environment fails."""
-        if not self.close_called:
-            self.close_called = True
-            return self.env.close()
-        else:
-            try:
-                return self.env.close()
-            except Exception as e:
-                logger.warn(
-                    "Calling `env.close()` on the closed environment should be allowed, but it raised the following exception."
-                )
-                raise e
+from gymnasium import spaces
+from gymnasium.core import ActType, ObsType
+from gymnasium.envs.registration import EnvSpec
+
+
+def basic_reset_func(
+    self,
+    *,
+    seed: int | None = None,
+    options: dict | None = None,
+) -> tuple[ObsType, dict]:
+    """A basic reset function that will pass the environment check using random actions from the observation space."""
+    super(GenericTestEnv, self).reset(seed=seed)
+    self.observation_space.seed(seed)
+    return self.observation_space.sample(), {"options": options}
+
+
+def old_reset_func(self) -> ObsType:
+    """An old reset function that will pass the environment check using random actions from the observation space."""
+    super(GenericTestEnv, self).reset()
+    return self.observation_space.sample()
+
+
+def basic_step_func(self, action: ActType) -> tuple[ObsType, float, bool, bool, dict]:
+    """A step function that follows the basic step api that will pass the environment check using random actions from the observation space."""
+    return self.observation_space.sample(), 0, False, False, {}
+
+
+def old_step_func(self, action: ActType) -> tuple[ObsType, float, bool, dict]:
+    """A step function that follows the old step api that will pass the environment check using random actions from the observation space."""
+    return self.observation_space.sample(), 0, False, {}
+
+
+def basic_render_func(self):
+    """Basic render fn that does nothing."""
+    pass
+
+
+# todo: change all testing environment to this generic class
+class GenericTestEnv(gym.Env):
+    """A generic testing environment for use in testing with modified environments are required."""
+
+    def __init__(
+        self,
+        action_space: spaces.Space = spaces.Box(0, 1, (1,)),
+        observation_space: spaces.Space = spaces.Box(0, 1, (1,)),
+        reset_func: Callable = basic_reset_func,
+        step_func: Callable = basic_step_func,
+        render_func: Callable = basic_render_func,
+        metadata: dict[str, Any] = {"render_modes": []},
+        render_mode: str | None = None,
+        spec: EnvSpec = EnvSpec(
+            "TestingEnv-v0", "tests.testing_env:GenericTestEnv", max_episode_steps=100
+        ),
+    ):
+        """Generic testing environment constructor.
+
+        Args:
+            action_space: The environment action space
+            observation_space: The environment observation space
+            reset_func: The environment reset function
+            step_func: The environment step function
+            render_func: The environment render function
+            metadata: The environment metadata
+            render_mode: The render mode of the environment
+            spec: The environment spec
+        """
+        self.metadata = metadata
+        self.render_mode = render_mode
+        self.spec = spec
+
+        if observation_space is not None:
+            self.observation_space = observation_space
+        if action_space is not None:
+            self.action_space = action_space
+
+        if reset_func is not None:
+            self.reset = types.MethodType(reset_func, self)
+        if step_func is not None:
+            self.step = types.MethodType(step_func, self)
+        if render_func is not None:
+            self.render = types.MethodType(render_func, self)
+
+    def reset(
+        self,
+        *,
+        seed: int | None = None,
+        options: dict | None = None,
+    ) -> ObsType | tuple[ObsType, dict]:
+        """Resets the environment."""
+        # If you need a default working reset function, use `basic_reset_fn` above
+        raise NotImplementedError("TestingEnv reset_fn is not set.")
+
+    def step(self, action: ActType) -> tuple[ObsType, float, bool, dict[str, Any]]:
+        """Steps through the environment."""
+        raise NotImplementedError("TestingEnv step_fn is not set.")
+
+    def render(self):
+        """Renders the environment."""
+        raise NotImplementedError("testingEnv render_fn is not set.")
```

### Comparing `gymnasium-0.29.1/gymnasium.egg-info/SOURCES.txt` & `gymnasium-1.0.0a1/gymnasium.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 gymnasium/__init__.py
 gymnasium/core.py
 gymnasium/error.py
+gymnasium/functional.py
 gymnasium/logger.py
 gymnasium/py.typed
 gymnasium.egg-info/PKG-INFO
 gymnasium.egg-info/SOURCES.txt
 gymnasium.egg-info/dependency_links.txt
 gymnasium.egg-info/requires.txt
 gymnasium.egg-info/top_level.txt
 gymnasium/envs/__init__.py
+gymnasium/envs/functional_jax_env.py
 gymnasium/envs/registration.py
 gymnasium/envs/box2d/__init__.py
 gymnasium/envs/box2d/bipedal_walker.py
 gymnasium/envs/box2d/car_dynamics.py
 gymnasium/envs/box2d/car_racing.py
 gymnasium/envs/box2d/lunar_lander.py
 gymnasium/envs/classic_control/__init__.py
@@ -27,53 +29,65 @@
 gymnasium/envs/classic_control/pendulum.py
 gymnasium/envs/classic_control/utils.py
 gymnasium/envs/classic_control/assets/clockwise.png
 gymnasium/envs/mujoco/__init__.py
 gymnasium/envs/mujoco/ant.py
 gymnasium/envs/mujoco/ant_v3.py
 gymnasium/envs/mujoco/ant_v4.py
+gymnasium/envs/mujoco/ant_v5.py
 gymnasium/envs/mujoco/half_cheetah.py
 gymnasium/envs/mujoco/half_cheetah_v3.py
 gymnasium/envs/mujoco/half_cheetah_v4.py
+gymnasium/envs/mujoco/half_cheetah_v5.py
 gymnasium/envs/mujoco/hopper.py
 gymnasium/envs/mujoco/hopper_v3.py
 gymnasium/envs/mujoco/hopper_v4.py
+gymnasium/envs/mujoco/hopper_v5.py
 gymnasium/envs/mujoco/humanoid.py
 gymnasium/envs/mujoco/humanoid_v3.py
 gymnasium/envs/mujoco/humanoid_v4.py
+gymnasium/envs/mujoco/humanoid_v5.py
 gymnasium/envs/mujoco/humanoidstandup.py
 gymnasium/envs/mujoco/humanoidstandup_v4.py
+gymnasium/envs/mujoco/humanoidstandup_v5.py
 gymnasium/envs/mujoco/inverted_double_pendulum.py
 gymnasium/envs/mujoco/inverted_double_pendulum_v4.py
+gymnasium/envs/mujoco/inverted_double_pendulum_v5.py
 gymnasium/envs/mujoco/inverted_pendulum.py
 gymnasium/envs/mujoco/inverted_pendulum_v4.py
+gymnasium/envs/mujoco/inverted_pendulum_v5.py
 gymnasium/envs/mujoco/mujoco_env.py
 gymnasium/envs/mujoco/mujoco_rendering.py
 gymnasium/envs/mujoco/pusher.py
 gymnasium/envs/mujoco/pusher_v4.py
+gymnasium/envs/mujoco/pusher_v5.py
 gymnasium/envs/mujoco/reacher.py
 gymnasium/envs/mujoco/reacher_v4.py
+gymnasium/envs/mujoco/reacher_v5.py
 gymnasium/envs/mujoco/swimmer.py
 gymnasium/envs/mujoco/swimmer_v3.py
 gymnasium/envs/mujoco/swimmer_v4.py
+gymnasium/envs/mujoco/swimmer_v5.py
 gymnasium/envs/mujoco/walker2d.py
 gymnasium/envs/mujoco/walker2d_v3.py
 gymnasium/envs/mujoco/walker2d_v4.py
+gymnasium/envs/mujoco/walker2d_v5.py
 gymnasium/envs/mujoco/assets/ant.xml
 gymnasium/envs/mujoco/assets/half_cheetah.xml
 gymnasium/envs/mujoco/assets/hopper.xml
 gymnasium/envs/mujoco/assets/humanoid.xml
 gymnasium/envs/mujoco/assets/humanoidstandup.xml
 gymnasium/envs/mujoco/assets/inverted_double_pendulum.xml
 gymnasium/envs/mujoco/assets/inverted_pendulum.xml
 gymnasium/envs/mujoco/assets/point.xml
 gymnasium/envs/mujoco/assets/pusher.xml
 gymnasium/envs/mujoco/assets/reacher.xml
 gymnasium/envs/mujoco/assets/swimmer.xml
 gymnasium/envs/mujoco/assets/walker2d.xml
+gymnasium/envs/mujoco/assets/walker2d_v5.xml
 gymnasium/envs/phys2d/__init__.py
 gymnasium/envs/phys2d/cartpole.py
 gymnasium/envs/phys2d/pendulum.py
 gymnasium/envs/phys2d/assets/clockwise.png
 gymnasium/envs/tabular/__init__.py
 gymnasium/envs/tabular/blackjack.py
 gymnasium/envs/tabular/cliffwalking.py
@@ -161,48 +175,14 @@
 gymnasium/envs/toy_text/img/mountain_bg2.png
 gymnasium/envs/toy_text/img/mountain_cliff.png
 gymnasium/envs/toy_text/img/mountain_near-cliff1.png
 gymnasium/envs/toy_text/img/mountain_near-cliff2.png
 gymnasium/envs/toy_text/img/passenger.png
 gymnasium/envs/toy_text/img/stool.png
 gymnasium/envs/toy_text/img/taxi_background.png
-gymnasium/experimental/__init__.py
-gymnasium/experimental/functional.py
-gymnasium/experimental/functional_jax_env.py
-gymnasium/experimental/vector/__init__.py
-gymnasium/experimental/vector/async_vector_env.py
-gymnasium/experimental/vector/sync_vector_env.py
-gymnasium/experimental/vector/vector_env.py
-gymnasium/experimental/vector/utils/__init__.py
-gymnasium/experimental/vector/utils/misc.py
-gymnasium/experimental/vector/utils/shared_memory.py
-gymnasium/experimental/vector/utils/space_utils.py
-gymnasium/experimental/wrappers/__init__.py
-gymnasium/experimental/wrappers/atari_preprocessing.py
-gymnasium/experimental/wrappers/common.py
-gymnasium/experimental/wrappers/jax_to_numpy.py
-gymnasium/experimental/wrappers/jax_to_torch.py
-gymnasium/experimental/wrappers/lambda_action.py
-gymnasium/experimental/wrappers/lambda_observation.py
-gymnasium/experimental/wrappers/lambda_reward.py
-gymnasium/experimental/wrappers/numpy_to_torch.py
-gymnasium/experimental/wrappers/rendering.py
-gymnasium/experimental/wrappers/stateful_action.py
-gymnasium/experimental/wrappers/stateful_observation.py
-gymnasium/experimental/wrappers/stateful_reward.py
-gymnasium/experimental/wrappers/utils.py
-gymnasium/experimental/wrappers/vector/__init__.py
-gymnasium/experimental/wrappers/vector/dict_info_to_list.py
-gymnasium/experimental/wrappers/vector/jax_to_numpy.py
-gymnasium/experimental/wrappers/vector/jax_to_torch.py
-gymnasium/experimental/wrappers/vector/numpy_to_torch.py
-gymnasium/experimental/wrappers/vector/record_episode_statistics.py
-gymnasium/experimental/wrappers/vector/vectorize_action.py
-gymnasium/experimental/wrappers/vector/vectorize_observation.py
-gymnasium/experimental/wrappers/vector/vectorize_reward.py
 gymnasium/spaces/__init__.py
 gymnasium/spaces/box.py
 gymnasium/spaces/dict.py
 gymnasium/spaces/discrete.py
 gymnasium/spaces/graph.py
 gymnasium/spaces/multi_binary.py
 gymnasium/spaces/multi_discrete.py
@@ -225,39 +205,36 @@
 gymnasium/utils/step_api_compatibility.py
 gymnasium/vector/__init__.py
 gymnasium/vector/async_vector_env.py
 gymnasium/vector/sync_vector_env.py
 gymnasium/vector/vector_env.py
 gymnasium/vector/utils/__init__.py
 gymnasium/vector/utils/misc.py
-gymnasium/vector/utils/numpy_utils.py
 gymnasium/vector/utils/shared_memory.py
-gymnasium/vector/utils/spaces.py
+gymnasium/vector/utils/space_utils.py
 gymnasium/wrappers/__init__.py
 gymnasium/wrappers/atari_preprocessing.py
-gymnasium/wrappers/autoreset.py
-gymnasium/wrappers/clip_action.py
-gymnasium/wrappers/compatibility.py
-gymnasium/wrappers/env_checker.py
-gymnasium/wrappers/filter_observation.py
-gymnasium/wrappers/flatten_observation.py
-gymnasium/wrappers/frame_stack.py
-gymnasium/wrappers/gray_scale_observation.py
-gymnasium/wrappers/human_rendering.py
-gymnasium/wrappers/normalize.py
-gymnasium/wrappers/order_enforcing.py
-gymnasium/wrappers/pixel_observation.py
-gymnasium/wrappers/record_episode_statistics.py
-gymnasium/wrappers/record_video.py
-gymnasium/wrappers/render_collection.py
-gymnasium/wrappers/rescale_action.py
-gymnasium/wrappers/resize_observation.py
-gymnasium/wrappers/step_api_compatibility.py
-gymnasium/wrappers/time_aware_observation.py
-gymnasium/wrappers/time_limit.py
+gymnasium/wrappers/common.py
+gymnasium/wrappers/jax_to_numpy.py
+gymnasium/wrappers/jax_to_torch.py
+gymnasium/wrappers/numpy_to_torch.py
+gymnasium/wrappers/rendering.py
+gymnasium/wrappers/stateful_action.py
+gymnasium/wrappers/stateful_observation.py
+gymnasium/wrappers/stateful_reward.py
+gymnasium/wrappers/transform_action.py
 gymnasium/wrappers/transform_observation.py
 gymnasium/wrappers/transform_reward.py
-gymnasium/wrappers/vector_list_info.py
-gymnasium/wrappers/monitoring/__init__.py
-gymnasium/wrappers/monitoring/video_recorder.py
+gymnasium/wrappers/utils.py
+gymnasium/wrappers/vector/__init__.py
+gymnasium/wrappers/vector/common.py
+gymnasium/wrappers/vector/dict_info_to_list.py
+gymnasium/wrappers/vector/jax_to_numpy.py
+gymnasium/wrappers/vector/jax_to_torch.py
+gymnasium/wrappers/vector/numpy_to_torch.py
+gymnasium/wrappers/vector/stateful_observation.py
+gymnasium/wrappers/vector/stateful_reward.py
+gymnasium/wrappers/vector/vectorize_action.py
+gymnasium/wrappers/vector/vectorize_observation.py
+gymnasium/wrappers/vector/vectorize_reward.py
 tests/test_core.py
 tests/testing_env.py
```

### Comparing `gymnasium-0.29.1/gymnasium.egg-info/requires.txt` & `gymnasium-1.0.0a1/gymnasium.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 [all]
 shimmy[atari]<1.0,>=0.1.0
 box2d-py==2.3.5
 pygame>=2.1.3
 swig==4.*
 mujoco-py<2.2,>=2.1
 cython<3
-mujoco>=2.3.3
+mujoco<=3.1.1,>=2.1.5
 imageio>=2.14.1
 jax>=0.4.0
 jaxlib>=0.4.0
+flax>=0.5.0
 lz4>=3.1.0
 opencv-python>=3.0
 matplotlib>=3.0
 moviepy>=1.0.0
 torch>=1.0.0
 
 [atari]
@@ -39,17 +40,18 @@
 
 [classic_control]
 pygame>=2.1.3
 
 [jax]
 jax>=0.4.0
 jaxlib>=0.4.0
+flax>=0.5.0
 
 [mujoco]
-mujoco>=2.3.3
+mujoco<=3.1.1,>=2.1.5
 imageio>=2.14.1
 
 [mujoco-py]
 mujoco-py<2.2,>=2.1
 cython<3
 
 [mujoco_py]
@@ -62,13 +64,14 @@
 matplotlib>=3.0
 moviepy>=1.0.0
 torch>=1.0.0
 
 [testing]
 pytest==7.1.3
 scipy>=1.7.3
+dill>=0.3.7
 
 [toy-text]
 pygame>=2.1.3
 
 [toy_text]
 pygame>=2.1.3
```

### Comparing `gymnasium-0.29.1/pyproject.toml` & `gymnasium-1.0.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,18 @@
 atari = ["shimmy[atari] >=0.1.0,<1.0"]
 accept-rom-license = ["autorom[accept-rom-license] ~=0.4.2"]
 box2d = ["box2d-py ==2.3.5", "pygame >=2.1.3", "swig ==4.*"]
 classic-control = ["pygame >=2.1.3"]
 classic_control = ["pygame >=2.1.3"]  # kept for backward compatibility
 mujoco-py = ["mujoco-py >=2.1,<2.2", "cython<3"]
 mujoco_py = ["mujoco-py >=2.1,<2.2", "cython<3"]       # kept for backward compatibility
-mujoco = ["mujoco >=2.3.3", "imageio >=2.14.1"]
+mujoco = ["mujoco >=2.1.5, <= 3.1.1", "imageio >=2.14.1"]
 toy-text = ["pygame >=2.1.3"]
 toy_text = ["pygame >=2.1.3"]         # kept for backward compatibility
-jax = ["jax >=0.4.0", "jaxlib >=0.4.0"]
+jax = ["jax >=0.4.0", "jaxlib >=0.4.0", "flax >= 0.5.0"]
 other = [
     "lz4 >=3.1.0",
     "opencv-python >=3.0",
     "matplotlib >=3.0",
     "moviepy >=1.0.0",
     "torch >=1.0.0",
 ]
@@ -63,31 +63,33 @@
     "swig ==4.*",
     # classic-control
     "pygame >=2.1.3",
     # mujoco-py
     "mujoco-py >=2.1,<2.2",
     "cython<3",
     # mujoco
-    "mujoco >=2.3.3",
+    "mujoco >=2.1.5, <=3.1.1",
     "imageio >=2.14.1",
     # toy-text
     "pygame >=2.1.3",
     # jax
     "jax >=0.4.0",
     "jaxlib >=0.4.0",
+    "flax >= 0.5.0",
     # other
     "lz4 >=3.1.0",
     "opencv-python >=3.0",
     "matplotlib >=3.0",
     "moviepy >=1.0.0",
     "torch >=1.0.0",
 ]
 testing = [
     "pytest ==7.1.3",
     "scipy >= 1.7.3",
+    "dill>=0.3.7",
 ]
 
 [project.urls]
 Homepage = "https://farama.org"
 Repository = "https://github.com/Farama-Foundation/Gymnasium"
 Documentation = "https://gymnasium.farama.org"
 "Bug Report" = "https://github.com/Farama-Foundation/Gymnasium/issues"
@@ -147,9 +149,11 @@
 # reportUnknownArgumentType = "warning"  # -> raises 2104 warnings
 reportGeneralTypeIssues = "none"  # -> commented out raises 489 errors
 # reportUntypedFunctionDecorator = "none"  # -> pytest.mark.parameterize issues
 
 reportPrivateUsage = "warning"
 reportUnboundVariable = "warning"
 
+reportPrivateImportUsage = "none"  # -> commented out raises 144 errors
+
 [tool.pytest.ini_options]
 filterwarnings = ["ignore::DeprecationWarning:gymnasium.*:"]
```

### Comparing `gymnasium-0.29.1/setup.py` & `gymnasium-1.0.0a1/setup.py`

 * *Files identical despite different names*

