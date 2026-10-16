# CPU Load Overview

Open when you need guidance on CPU Load Overview in Ableton Live.

Context: [Computer Audio Resources and Strategies](computer-audio-resources-and-strategies.md#37-computer-audio-resources-and-strategies).

<a id="source-371-managing-the-cpu-load"></a>
### 37.1 Managing the CPU Load

Delivering an unbroken flow of audio out to the hardware forces Live to run an enormous quantity of math each second. Should the processor fall behind on that workload, you will end up with clicks or dropouts in the sound.

Several things shape how fast a machine can compute: the processor clock rates (e.g., speed in MHz or GHz), the chip architecture, the temperature (when it gets too warm, today's CPUs “thermal throttle” by dialing back their pace), the memory cache performance (a measure of how readily the chip pulls data out of memory), and the system bus bandwidth — the computer’s “pipeline“ that every byte has to travel along.

The good news is that Live works with multicore and multiprocessor systems, so the workload from instruments, effects, and I/O can be spread across the resources you have on hand. The usable processing power may exceed that of older machines by a wide margin, depending on your hardware and the Live Set in question.
