# Experiment--05-Implementation-of-flipflops-using-verilog
AIM: 

To implement all the flipflops using verilog and validating their functionality using their functional tables

HARDWARE REQUIRED:

– PC, Cyclone II , USB flasher

SOFTWARE REQUIRED: Quartus prime

THEORY

SR Flip-Flop SR flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, SR latch operates with enable signal. The circuit diagram of SR flip-flop is shown in the following figure.

![167910294-bb550548-b1dc-4cba-9044-31d9037d476b](https://user-images.githubusercontent.com/123359969/214301370-541f9e70-1ca9-469b-8b4a-542d5b44013a.png)


This circuit has two inputs S & R and two outputs Qtt & Qtt’. The operation of SR flipflop is similar to SR Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of SR flip-flop.


![167910648-ced88e69-869c-42e2-9718-a285a3902446](https://user-images.githubusercontent.com/123359969/214301491-a1c41f8a-8c3f-4e36-99f1-8e0d4f165e2d.png)

Here, Qtt & Qt+1t+1 are present state & next state respectively. So, SR flip-flop can be used for one of these three functions such as Hold, Reset & Set based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of SR flip-flop. Present Inputs Present State Next State

![167908180-5fc9d589-1cb5-41f5-b2c8-927e04f5f387](https://user-images.githubusercontent.com/123359969/214301570-d0bd0bfc-473a-4919-9db2-4556375f283f.png)

By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. The three variable K-Map for next state, Qt+1t+1 is shown in the following figure.

![167908214-25b30a54-db20-4bcb-9385-5f93a1982a09](https://user-images.githubusercontent.com/123359969/214301726-c964fe88-61d7-4a92-90af-3bf477a42999.png)


The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=S+R′Q(t)Q(t+1)=S+R′Q(t)

D Flip-Flop

D flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, D latch operates with enable signal. That means, the output of D flip-flop is insensitive to the changes in the input, D except for active transition of the clock signal. The circuit diagram of D flip-flop is shown in the following figure.

This circuit has single input D and two outputs Qtt & Qtt’. The operation of D flip-flop is similar to D Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state 

![167908342-e03f0cbb-5958-43bb-b74a-5e3ec2341675](https://user-images.githubusercontent.com/123359969/214302235-c966d0f8-fb93-4c78-8833-152fa1c5a7db.png)


table of D flip-flop.

![167910325-aeef0739-0a54-40e2-bebd-6f5fa0cad10e](https://user-images.githubusercontent.com/123359969/214302308-e781b8b6-1b79-4fa2-bf66-513419516942.png)

Therefore, D flip-flop always Hold the information, which is available on data input, D of earlier positive transition of clock signal. From the above state table, we can directly write the next state equation as Qt+1t+1 = D

![167908850-d39d07ba-7f9d-490a-b9f2-274e189fd047](https://user-images.githubusercontent.com/123359969/214302426-c8b05eba-eaa5-4cec-b4cf-004557a001c8.png)


Next state of D flip-flop is always equal to data input, D for every positive transition of the clock signal. Hence, D flip-flops can be used in registers, shift registers and some of the counters.

JK Flip-Flop

JK flip-flop is the modified version of SR flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of JK flip-flop is shown in the following figure.

![167910378-d2d984a7-2815-4d17-8c41-ee4bdf59ec24](https://user-images.githubusercontent.com/123359969/214302568-d475669c-c34f-41d9-a08d-7968a84ea9c7.png)

This circuit has two inputs J & K and two outputs Qtt & Qtt’. The operation of JK flip-flop is similar to SR flip-flop. Here, we considered the inputs of SR flip-flop as S = J Qtt’ and R = KQtt in order to utilize the modified SR flip-flop for 4 combinations of inputs. The following table shows the state table of JK flip-flop.


![167908575-59c35afb-50d3-46a2-888c-47478a3179d5](https://user-images.githubusercontent.com/123359969/214302661-61faefc5-267e-49f2-a5bd-5bb19412dce6.png)

Here, Qtt & Qt+1t+1 are present state & next state respectively. So, JK flip-flop can be used for one of these four functions such as Hold, Reset, Set & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of JK flip-flop. Present Inputs Present State Next State

![167908664-c854ffe9-0bd3-44c2-bfa6-e53928181c69](https://user-images.githubusercontent.com/123359969/214302746-22c0d22e-f500-4ef8-9f6c-db9b057546b8.png)


By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. Three variable K-Map for next state, Qt+1t+1 is shown in the following figure.

![167908688-fa93c3e9-8323-4864-947d-c11d163d5a90](https://user-images.githubusercontent.com/123359969/214302849-e255d298-1edc-4075-be64-1945d9b4e207.png)


The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=JQ(t)′+K′Q(t)Q(t+1)=JQ(t)′+K′Q(t)

T Flip-Flop
T flip-flop is the simplified version of JK flip-flop. It is obtained by connecting the same input ‘T’ to both inputs of JK flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of T flip-flop is shown in the following figure.

![167911534-5f3c445d-bc68-46e2-9a9c-7efce5febc60](https://user-images.githubusercontent.com/123359969/214302953-04c6195a-80c6-4b11-acf3-eabf0d6578a2.png)


This circuit has single input T and two outputs Qtt & Qtt’. The operation of T flip-flop is same as that of JK flip-flop. Here, we considered the inputs of JK flip-flop as J = T and K = T in order to utilize the modified JK flip-flop for 2 combinations of inputs. So, we eliminated the other two combinations of J & K, for which those two values are complement to each other in T flip-flop. The following table shows the state table of T flip-flop.

Here, Qtt & Qt+1t+1 are present state & next state respectively. So, T flip-flop can be used for one of these two functions such as Hold, & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of T flip-flop. Inputs Present State Next State


![167909015-53aa9450-3f28-4202-887a-79d88228f8a0](https://user-images.githubusercontent.com/123359969/214303053-5158a094-770c-4b0f-8d98-1a6ee959b377.png)

From the above characteristic table, we can directly write the next state equation as Q(t+1)=T′Q(t)+TQ(t)′ ⇒Q(t+1)=T⊕Q(t)

Procedure
```
Using NAND gates and wires construct SR Flip-flop
Repeat same steps to construct JK, D, T flipflops
Find RTL logic and timing diagram for all flipflops
End the program
```
PROGRAM

Program for flipflops and verify its truth table in quartus using Verilog programming.

Developed by: Santhosh L

RegisterNumber: 22008479

SR Flip-flop
```
module sr_flipflop(S, R, clock, Q, Qbar);
input S, R, clock;
output Q, Qbar;
wire X, Y;
nand(X, S, clock);
nand(Y, R, clock);
nand(Q, X, Qbar);
nand(Qbar, Y, Q);
endmodule
```
D Flip-flop
```
module d_flipflop(D, clock, Q, Qbar);
input D, clock;
output Q, Qbar;
assign Dbar = ~D;
wire X, Y;
nand(X, D, clock);
nand(Y, Dbar, clock);
nand(Q, X, Qbar);
nand(Qbar, Y, Q);
endmodule
```
JK Flip-flop
```
module jk_flipflop(J, K, clock, Q, Qbar);
input J, K, clock;
output Q, Qbar;
wire P, S;
nand(P, J, clock, Qbar);
nand(S, K, clock, Q);
nand(Q, P, Qbar);
nand(Qbar, S, Q);
endmodule
```
T Flip-flop
```
module t_flipflop(T, clock, Q, Qbar);
input T, clock;
output Q, Qbar;
wire A, B;
nand(A, T, clock, Qbar);
nand(B, T, clock, Q);
nand(Q, A, Qbar);
nand(Qbar, B, Q);
endmodule
```
RTL LOGIC FOR FLIPFLOPS
SR Flip-flop

![sr_ff_rtl](https://user-images.githubusercontent.com/123359969/214303814-4de546e7-2f26-43c9-b04b-795a4d9e3b42.png)


D Flip-flop

![d_ff_rtl](https://user-images.githubusercontent.com/123359969/214303850-023c7316-58a3-438b-86f9-1506b2a1d08d.png)

JK Flip-flop

![jk_ff_rtl](https://user-images.githubusercontent.com/123359969/214303870-b37fa708-57b6-4261-ba23-9cbce06a4fe1.png)


T Flip-flop

![t_ff_rtl](https://user-images.githubusercontent.com/123359969/214303896-f36a7a58-76ef-4674-9949-c47de12c31b4.png)


TIMING DIGRAMS FOR FLIPFLOPS
SR Flip-flop

![sr_ff_td](https://user-images.githubusercontent.com/123359969/214303914-94f0476b-5af6-4b89-a96a-5fd78b265d93.png)

D Flip-flop

![d_ff_td](https://user-images.githubusercontent.com/123359969/214303925-41190155-45fd-4655-beee-fffa3ecc07fe.png)


JK Flip-flop

![jk_ff_td](https://user-images.githubusercontent.com/123359969/214303938-70543127-164f-4718-b639-6e89d62e34e3.png)


T Flip-flop

![t_ff_td](https://user-images.githubusercontent.com/123359969/214303973-bc77f69d-ee07-45b1-a924-f0c43323679a.png)


RESULTS

Thus implementation of flipflops using verilog is verified
