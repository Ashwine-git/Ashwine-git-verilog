<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

The Leaky Integrate-and-Fire (LIF) Neuron is a simple model of neuronal behavior. In this design, the neuron receives an input signal (spike) and integrates this input over time by increasing its internal membrane potential. If there is no input, the membrane potential "leaks" or decays gradually over time, simulating the natural loss of charge in biological neurons.

When the membrane potential reaches a defined threshold, the neuron fires a spike output, after which the membrane potential resets to zero. This process emulates the firing and reset cycle of biological neurons, providing a digital approximation of spiking behavior.

This project implements a single LIF neuron using digital logic. It showcases how a neuron model can be built in hardware to accumulate inputs, leak over time, and generate a firing signal when reaching a threshold.

## How to test

1. **Setup**: Upload the Verilog code to the Tiny Tapeout platform or a Verilog simulation environment.
2. **Provide Input Signals**: Apply input signals to the `spike_in` input to simulate incoming spikes or stimuli.
3. **Monitor Output**: Observe the `spike_out` output. The output will go high whenever the membrane potential of the neuron reaches the threshold, indicating that the neuron has "fired."
4. **Adjust Frequency**: Vary the frequency and intensity of the input spikes to test the neuron’s response under different conditions. Confirm that the neuron fires only when the integrated potential reaches the threshold and that it resets afterward.

This simple testing process will allow us to verify the neuron's behavior, including integration, leakage, and firing.

## External hardware

This project does not require external hardware. It operates entirely on the Tiny Tapeout platform. However, a logic analyzer or oscilloscope can be useful if we wish to visualize the output spikes and observe the neuron’s firing pattern.
