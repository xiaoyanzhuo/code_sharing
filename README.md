# Codes Sharing

Mainly for sharing codes sometime. 

## Openvx_sample

* openvx_sample/examples/vx\_tiling*
  * vx\_tiling\_ext.c : add two kernels: erode and dilate
  * vx\_tiling\_ext.h : add definition, declaration of the two kernels
  * vx\_tiling_[kernels].c 
      * 4 default [kernels]: add, alpha, box, gaussian, which can be found in original [openvx\_sample repo](https://github.com/xiaoyanzhuo/openvx_sample/tree/master/examples)
      * 2 new [kernels]: erode, dilate (vx\_tiling\_erode.c, vx\_tiling\_dilate.c)
  * tiling\_[kernels].c: Specifically, tiling\_erode.c, tiling\_dilate.c. They are similar to the 'vx\_tiling_main.c' which run 4 default kernels example together, while tiling\_erode.c only run erode kernel and tiling\_dilate.c only run dilate kernel.
  * CMakeLists.txt: add erode.c and dilate.c compilation in line 69.

