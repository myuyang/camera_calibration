# camera_calibration
单目标定流程：

1.使用相机拍摄不少于3张标定板的照片

2.修改calibration.cpp中25行的角点个数

3.在calibdata文件中声明照片的路径

4.编译calibration.cpp 需要opencv环境

使用命令：

g++ calibration.cpp -o calib `pkg-config --cflags --libs opencv`

5.执行 ./calib

6.得到标定结果calibration_result.txt
