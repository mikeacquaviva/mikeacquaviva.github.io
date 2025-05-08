---
layout: page
title: Pong on a Xilinx FPGA
permalink: /projects/pong/
---

In this project, I used a Xilinx FPGA on a Neyxs 4 DDR board to implement the classic game of pong in hardware.

<div style="max-width: 400px; text-align: center; margin: 2rem auto;">
  <img src="/assets/images/pong.png" alt="Pong" style="width: 100%; max-width: 600px; height: auto; border-radius: 12px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
</div>

The game logic and graphics were implemented in hardware, while sound effects used a Microblaze soft processor.

Check out the Verilog and Vivado project on GitHub [here](https://github.com/mikeacquaviva/fpga-pong).