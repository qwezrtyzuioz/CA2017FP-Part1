# NCTU 2017 Computer Architecture Final Project - Part 1

Part-1：Implement convolution , relu , and maxpooling in convLayerGPU() with CUDA and store your result in the outGPU and use NVVP to analyze your code.

## Three sub-directory

### ./data
This directory contains the input data for the base program：
* . /data/filter.txt - Store the values of filters
* . /data/neuron.txt - Store the values of input neurons

### ./device
The program under this directory can show the device information.
#### usage
<pre>
cd ./device
make
make run
</pre>

### ./example
There are two examples(InnerProduct and Matrix Multiplication) under this directory.
#### usage
<pre>
cd ./example/InnerProduct/
make
make run

or

cd ./example/MatrixMultiplication/
make
make run
</pre>

## Usage of the base program
<pre>
make
make run
</pre>

## Evaluation
We will compare the execution time to get the speedup by
<pre>
Speedup = convLayerCPU_execTime / convLayerGPU_execTime
</pre>

## Grading Policy
*  (A) Completeness (35%)
  *  Your result(convLayerGPU) must be correct (Pass the check) (10%)
  *  Your design(convLayerGPU) is faster than convLayerCPU() (20%)
  *  Use NVIDIA Visual Profiler to help you improve performance(TA will check it in your report) (5%)
*  (B) Report (35%)
  *  Describe your implementation algorithm and explain your results (15%)
  *  Discuss what kind of optimization you did( it is better or worse?) (10%)
  *  Show how you use NVVP to help you find and solve perf. issues (5%)
  *  Feedback of this part (5%)
*  (C) Performance Rank (30%)
  *  We will rank your CUDA kernels’ performance(execution time) on GTX K20C
  *  The fastest one will get 30% and the last one will get 1%

