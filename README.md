**FULL_ADDER**

**Aim:**

To simulate and synthesis Full adder using vivado.

**Apparatus Required:**

vivado 2023.2 software.

**Procedure:**

STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.

**Truth Table**

![301804329-02ead8f5-d958-4c89-ac51-368ca086cf41](https://github.com/pullurur/FULL_ADDER/assets/161436550/1592ac0c-96f6-44e1-92a1-47ecf5b7a3dd)

**Circuit Diagram**

![301804439-418e00aa-ed19-4ab3-a413-bae9575bff0e](https://github.com/pullurur/FULL_ADDER/assets/161436550/3f31de02-4643-4e93-8fbd-51265e22d4d1)

**Program**

module FA(a,b,cin,sum,cout);

input a,b,cin;

output sum,cout;

wire w1,w2,w3;

xor g1(w1,a,b);

and g2(w2,w1,cin);

and g3(w3,a,b);

xor g4(sum,w1,cin);

or g5(cout,w2,w3);

endmodule

**output**

![318192816-a2734052-ad50-4ec1-8dfc-baeb0a5431af](https://github.com/pullurur/FULL_ADDER/assets/161436550/8b2b8466-187f-4e84-947c-1cc5b98d37b3)

**Result**
Thus the verilog program for Full adder has been simulated and verified successfully.
