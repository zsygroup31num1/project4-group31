# project4-group11
考虑以下一些优化措施：

使用位运算代替乘除法：在SM3算法中，一些乘法和除法运算可以通过位运算（左移、右移、异或等）来替代，从而提高计算效率。

批量处理数据块：目前的实现是逐个处理每个64字节的数据块，可以考虑对多个数据块进行批量处理，以减少循环次数，提高处理效率。

使用优化的循环结构：在循环中尽量避免不必要的内存访问，减少数据移动，以及尽量利用处理器的流水线执行特性。

并行计算：可以考虑使用并行计算的技术，如多线程或多进程，以充分利用多核处理器的能力。

内存对齐：对于一些平台，内存对齐对于提高访问效率非常重要。确保数据结构按照正确的字节对齐方式进行存储和访问。

使用硬件加速：对于一些特定平台，可以使用硬件加速技术，如AES指令集、SIMD指令集等，以加快哈希函数的计算速度。

最终我实现了sm3的加密过程时长为0.1s
运行结果：![image](https://github.com/zsygroup11num1/project4-group11/assets/129477117/9ae40510-1c07-46db-9c6e-c87a64e8050c)
