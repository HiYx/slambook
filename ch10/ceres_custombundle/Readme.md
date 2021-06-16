#To build the code : 
mkdir build

cd ./build

cmake ..

make

#How to run the code :

cd ./build

./ceres_customBundle -input ../data/problem-.....txt

#see more detail settings by :
./ceres_customBundle -help



0526 修改：

```
include_directories(${CERES_INCLUDE_DIRS} 
	    "/usr/include/eigen3/")
	    
//options->num_linear_solver_threads = params.num_threads;
options->num_threads = params.num_threads;
```

