# PCA-GPU-based-vector-summation.-Explore-the-differences.
i) Using the program sumArraysOnGPU-timer.cu, set the block.x = 1023. Recompile and run it. Compare the result with the execution confi guration of block.x = 1024. Try to explain the difference and the reason.

ii) Refer to sumArraysOnGPU-timer.cu, and let block.x = 256. Make a new kernel to let each thread handle two elements. Compare the results with other execution confi gurations.
Aim:
(i) To modify or set the execution configuration of block.x as 1023 & 1024 and compare the elapsed time obtained on Host and GPU.

(ii) To set the number of threads as 256 and obtain the elapsed time on Host and GPU.

Procedure:
Step 1 :
Include the required files and library.

Step 2 :
Declare a function sumMatrixOnHost , to perform vector summation on the host side .

Step 3 :
Declare a function with __ global __ , which is a CUDA C keyword , to execute the function to perform vector summation on GPU .

Step 4 :
Declare Main method/function .

Step 5 :
In the Main function Set up device and data size of vector ,Allocate Host Memory and device global memory,Initialize data at host side and then add vector at host side ,transfer data from host to device.

Step 6 :
Invoke kernel at host side(1023,1024,256), check for kernel error and copy kernel result back to host side.

Step 7 :
Finally Free device global memory,host memory and reset device.

Step 8 :
Save and Run the Program.

## Output:

## Result:
