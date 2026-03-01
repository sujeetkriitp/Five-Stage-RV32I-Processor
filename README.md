# Five-Stage-RV32I-Processor
The proposed processor is a five-stage pipelined RV32I RISC-V core that supports a subset of 36 base instructions, covering arithmetic, logical, memory access, and control operations. In pipelined RISC-V architectures, data hazards and control hazards have a direct impact on execution efficiency and the reliability of program flow
The proposed processor is a five-stage pipelined RV32I RISC-V core that supports a
subset of 36 base instructions, covering arithmetic, logical, memory access, and control
operations. In pipelined RISC-V architectures, data hazards and control hazards have
a direct impact on execution efficiency and the reliability of program flow. These is-
sues primarily arise from load-word (LW) instructions with operand dependency and
branch instructions whose outcomes are not immediately known during earlier pipeline
stages. To improve the execution performance of the energy-efficient core presented in
this work, dedicated hardware mechanisms have been incorporated for both data- and
control-hazard mitigation. Data hazards are managed through a hazard control and for-
warding unit that resolves operand dependencies without resorting to excessive pipeline
stalling. For control hazards, branch conditions are evaluated in the EX stage, and the
control-hazard unit intervenes only when a branch decision requires redirection of the
instruction sequence. By combining the forwarding-based data-hazard solution with a
lightweight control-hazard handling strategy, the pipeline aims to maintain stable in-
struction flow, reduce bubble generation, and improve overall energy efficiency while
preserving the simplicity of a low-end five-stage RISC-V design.
<img width="1344" height="761" alt="image" src="https://github.com/user-attachments/assets/3d1604d3-889f-4dd9-80f1-1761686125ad" />
Five-stage RV32I : Data hazard handling algorithm
<img width="1341" height="762" alt="image" src="https://github.com/user-attachments/assets/76723d8d-5c1e-4f75-bc74-dc3e05382b22" />
Five-stage RV32I processor micro-architecture with Data hazard unit
<img width="1338" height="747" alt="image" src="https://github.com/user-attachments/assets/51dc7eca-8b6b-4dd5-839d-22f081f7ff1e" />
Control hazard Handling Algorithm
<img width="1330" height="744" alt="image" src="https://github.com/user-attachments/assets/c7bc20ab-0608-4b8f-8cfb-2141e0b5b722" />
Five-stage RV32I processor micro-architecture with Data and Control hazard unit
<img width="1349" height="759" alt="image" src="https://github.com/user-attachments/assets/96073a6e-d193-49d9-b799-4cf68720c79b" />
Five-stage RV32I processor micro-architecture with Data and Control hazard unit: RTL Simulation
<img width="1345" height="751" alt="image" src="https://github.com/user-attachments/assets/7eaeb13a-5aed-44e7-ac47-9fd9fb95df3a" />
FPGA Prototype and Evaluation results
<img width="1321" height="755" alt="image" src="https://github.com/user-attachments/assets/8f2df6b1-cba5-4c42-acfb-2fd3adce8f9c" />
PUBLICtion: Under Review

