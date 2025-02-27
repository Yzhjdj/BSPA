这个代码用于解决二维条带装箱问题。

可直接运行jar文件，命令如下

单个问题的处理：

java -jar 'jar文件路径' 'problem_n.txt所在的文件夹路径' '结果输出文件夹的路径' '运行时间' '并行线程数' '1(默认值)' '参数b的值' 'minFillRate' 'n'

eg : java -jar C:\out\artifacts\BSGT_jar\BSPA.jar C:\dateset\C C:\outcome 30 16 1 0.1 1 21 

这个指令将会处理C:\dateset\C目录下problem21.txt这个问题同时将结果输出于C:\outcome,运行时间为30s，并行数量为16，b=0.1，minFillRate=1


处理整个数据集

java -jar 'jar文件路径' '数据集的文件夹路径' '结果输出文件夹的路径' '运行时间' '并行线程数' '1这个值(默认值)' '参数b的值' 'minFillRate'

eg : java -jar C:\out\artifacts\BSGT_jar\BSPA.jar C:\dateset\C C:\Coutcome 30 16 1 0.1 1

这个指令将会处理C:\dateset\C目录下的所有problem同时将结果输出于C:\Coutcome,运行时间为30s，并行数量为16，b=0.1，minFillRate=1


# 2D Strip Packing Problem Solver

This repository contains code for solving the **two-dimensional strip packing problem** using a beam search-based algorithm. The solution is packaged as a runnable JAR file that can be executed with Java.

## Usage

### Running the JAR File

You can directly run the JAR file using the following commands:

### Process a Single Problem

To solve a single problem instance, use the following command format:

`java -jar 'path_to_jar_file' 'problem_n.txt_folder_path' 'output_folder_path' 'runtime' 'num_threads' '1(default)' 'parameter_b_value' 'minFillRate' 'n'`

#### Example:
`java -jar C:\out\artifacts\BSGT_jar\BSPA.jar C:\dataset\C C:\outcome 30 16 1 0.1 1 21`

This will solve the problem defined in `problem21.txt` located in the `C:\dataset\C` directory. The results will be saved in the `C:\outcome` folder. The algorithm will run for 30 seconds, using 16 parallel threads, with `b=0.1`, `minFillRate=1`

### Process the Entire Dataset

To process an entire dataset, use the following command format:
`java -jar 'path_to_jar_file' 'dataset_folder_path' 'output_folder_path' 'runtime' 'num_threads' '1(default)' 'parameter_b_value' 'minFillRate'`

#### Example:

`java -jar C:\out\artifacts\BSGT_jar\BSPA.jar C:\dataset\C C:\Coutcome 30 16 1 0.1 1`

This will process all problems in the `C:\dataset\C` directory, saving the results in the `C:\Coutcome` folder. The algorithm will run for 30 seconds, using 16 parallel threads, with `b=0.1` and `minFillRate=1`.


