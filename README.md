# BOOLEAN_FUNCTION_MINIMIZATION

AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime

Theory:

Boolean function minimization is the process of simplifying Boolean algebraic expressions to reduce the number of logic gates and complexity in a digital circuit, leading to more efficient, faster, and less costly hardware

For minimizing Boolean expressions,we can use a set of rules and laws (like distributive, associative, and complement laws) to simplify Boolean expressions. This method focuses on applying algebraic manipulations to reduce the complexity of the expression by eliminating redundant terms.

Identity Law A ⋅ 1 = A,A + 0 = A

Null Law A ⋅ 0 = 0, A + 1 = 1

Idempotent Law A ⋅ A = A, A + A = A 

Complement Law A ⋅ A′ = 0, A + A' = 1

Distributive Law A ⋅ (B + C) = A ⋅ B + A ⋅ C

De Morgan’s Law (A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′

Absorption Law A ⋅ (A + B) = A, A + (A ⋅ B) = A 

Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C

Commutative law A B = B A,A + B = B + A



Logic Diagram:




Identity law:

<img width="1437" height="747" alt="Screenshot 2025-11-25 223741" src="https://github.com/user-attachments/assets/d159f444-b035-481a-8e0a-ef816a7b2f83" />





Null law:

<img width="1421" height="776" alt="Screenshot 2025-11-25 223801" src="https://github.com/user-attachments/assets/1ddac5e3-1f38-40ec-b558-bc5d84719d1b" />




Idempotent Law

<img width="1019" height="721" alt="Screenshot 2025-11-25 223823" src="https://github.com/user-attachments/assets/52df766c-8305-4e15-b5ca-f218f9d778d0" />


Complement Law

<img width="1023" height="642" alt="Screenshot 2025-11-25 223838" src="https://github.com/user-attachments/assets/1547939e-2c01-4d4a-b620-55e9361fcd87" />






Distributive Law


<img width="1029" height="712" alt="Screenshot 2025-11-25 223900" src="https://github.com/user-attachments/assets/04c7f560-1ca7-4a79-b10c-a626cb9f4521" />


De Morgan’s Law




<img width="1027" height="518" alt="Screenshot 2025-11-25 223918" src="https://github.com/user-attachments/assets/bfe3fac2-2fbf-4d14-ba2f-ffbc33611964" />


Absorption Law

<img width="428" height="163" alt="Screenshot 2025-11-25 223955" src="https://github.com/user-attachments/assets/6bc66a05-3945-49ad-b5c4-78ae0cc4702c" />




Associative Law

<img width="537" height="558" alt="Screenshot 2025-11-25 224107" src="https://github.com/user-attachments/assets/cd02f5fc-72f6-4704-80bf-657a16c1ece2" />





Commutative law

<img width="530" height="624" alt="Screenshot 2025-11-25 224121" src="https://github.com/user-attachments/assets/bb438008-b3a9-49d6-a352-7aaf1c619c6d" />




Procedure:

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


Program:

```

i)
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

```

 ```

ii)
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule


```

Developed by:R.DARSHINI RegisterNumber:25017318


RTL realization:



Output:

i)

<img width="1021" height="531" alt="Screenshot 2025-11-26 194529" src="https://github.com/user-attachments/assets/df8321d2-4645-4ef8-9ed8-108947e4b5e0" />



ii)

<img width="1032" height="531" alt="Screenshot 2025-11-26 194558" src="https://github.com/user-attachments/assets/71981eff-fd69-4002-a4fc-bcaaece01921" />



RTL:

Timing Diagram:

i)

<img width="1028" height="575" alt="Screenshot 2025-11-26 194618" src="https://github.com/user-attachments/assets/a775fa40-7a79-4b13-b02d-e5b2920c0af8" />

ii)

<img width="1032" height="543" alt="Screenshot 2025-11-26 194631" src="https://github.com/user-attachments/assets/2668853f-f417-4b67-a7b7-dae8d721e527" />



Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

