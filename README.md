# Pose_graph_pnpl

You need to install `Ceres` and `Eigen` libraries.

### Compile Project:
```shell
mkdir build
cd build
cmake ..
make -j6
cd ..
```

### Pose Graph Demo:
The executable `pose_graph_3d` has one flag `--input` which is the path to the
problem definition. To run the executable,
```shell
cd build
./pose_graph --input ../data/sphere.g2o
cd ..
```


### Visualization:
```shell
python plot_results.py --initial_poses ./build/poses_original.txt --optimized_poses ./build/poses_optimized.txt
```
