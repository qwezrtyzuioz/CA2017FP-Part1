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
**(A) Completeness (35%)**<br/>
&nbsp;    Your result(convLayerGPU) must be correct (Pass the check) (10%)<br/>
&nbsp;&nbsp;&nbsp;    Your design(convLayerGPU) is faster than convLayerCPU() (20%)<br/>
&nbsp;&nbsp;&nbsp;    Use NVIDIA Visual Profiler to help you improve performance(TA will check it in your report) (5%)<br/>
**(B) Report (35%)**<br/>
&nbsp;&nbsp;&nbsp;    Describe your implementation algorithm and explain your results (15%)<br/>
&nbsp;&nbsp;&nbsp;    Discuss what kind of optimization you did( it is better or worse?) (10%)<br/>
&nbsp;&nbsp;&nbsp;    Show how you use NVVP to help you find and solve perf. issues (5%)<br/>
&nbsp;&nbsp;&nbsp;    Feedback of this part (5%)<br/>
**(C) Performance Rank (30%)**<br/>
&nbsp;&nbsp;&nbsp;    We will rank your CUDA kernels’ performance(execution time) on GTX K20C<br/>
&nbsp;&nbsp;&nbsp;    The fastest one will get 30% and the last one will get 1%<br/>

