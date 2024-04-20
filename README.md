# Custom Convolution Circuit Implementation on Zedboard FPGA
## Improve performance compared to a microprocessor by exploiting parallelism.

This project implements a custom convolution circuit on the Zedboard FPGA platform to enhance digital signal processing performance compared to traditional microprocessor-based approaches. This project focuses on leveraging parallelism to accelerate convolution operations, utilizing an emulated DRAM interface, custom convolution pipeline, and efficient data buffering techniques.

* **Convolution Operation:** 
  - Digital signal processing operation essential for various applications. 
  - Pseudocode provided for reference. 
  - Instructions for handling boundary conditions and overflow in FPGA implementation.

* **DRAM DMA Interface:** 
  - Creation of a DMA entity for efficient data transfer between FPGA and emulated DRAM. 
  - Synchronization of control and data signals across different clock domains. 
  - Implementation of FIFOs for data transfer and handling 16-bit data width conversion.

* **Convolution Pipeline:** 
  - Development of a custom pipeline exploiting parallelism for improved performance. 
  - Detailed structure including multipliers, adder tree, and pipeline registers. 
  - Recommendations for implementation techniques to optimize resource usage.

* **Signal and Kernel Buffer:** 
  - Introduction of buffers for efficient data reuse and bandwidth enhancement. 
  - Utilization of shift registers and FIFO-like interfaces for signal and kernel data handling. 
* **Testing and Debugging:**
  - Importance of comprehensive testbench creation for validation and debugging. 
  - For further improvements such as padding optimization and support for arbitrary kernel sizes.



## Convolution pseduocode below:
![image](https://github.com/abhasingh12/Zedboard_custom_ip/assets/153552335/ee81a3fe-8b44-4a4d-a7e6-0b227c58d501)
