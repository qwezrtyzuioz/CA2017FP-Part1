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
cd example/InnerProduct/
make
make run

or

cd example/MatrixMultiplication/
make
make run
</pre >

