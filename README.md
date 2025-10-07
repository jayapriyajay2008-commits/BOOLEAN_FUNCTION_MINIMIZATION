# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
 Boolean function minimization is the process of simplifying Boolean algebraic
 expressions to reduce the number of logic gates and complexity in a digital circuit,
 leading to more efficient, faster, and less costly hardware
 
 For minimizing Boolean expressions,we can use a set of rules and laws (like distributive,
 associative, and complement laws) to simplify Boolean expressions. This method
 focuses on applying algebraic manipulations to reduce the complexity of the expression
 by eliminating redundant terms.
 
 Identity Law A ⋅ 1 = A, A + 0 = A
 Null Law A ⋅ 0 = 0, A + 1 = 1
 Idempotent Law A ⋅ A = A, A + A = A
 Complement Law A ⋅ A′ = 0, A + A' = 1
 Distributive Law A ⋅ (B + C) = A ⋅ B + A ⋅ C
 De Morgan’s Law (A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′
 Absorption Law A ⋅ (A + B) = A, A + (A ⋅ B) = A
 Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C
 Commutative law A B = B A,A + B = B + A
 
**Logic Diagram**
Identity law
<img width="808" height="430" alt="{C71951CC-BB6D-4A5C-93FA-9BF022380EDF}" src="https://github.com/user-attachments/assets/2e2007e5-944b-4e82-a6d7-b7d0c4f57004" />
Idempotent law
<img width="284" height="182" alt="image" src="https://github.com/user-attachments/assets/13070bba-5044-4a31-ac2a-b884e31b9734" />
Complement law
<img width="288" height="184" alt="{99B12E60-1E05-49BE-81B3-17C6F588C945}" src="https://github.com/user-attachments/assets/04880346-c7e8-42fe-a5da-08f18749ca39" />
Distributive law
<img width="719" height="176" alt="image" src="https://github.com/user-attachments/assets/dfd884ff-1a77-4af7-8d6e-7cc9d4d8198d" />
demorgans law
<img width="689" height="581" alt="{720F625C-39DD-4F83-AC09-77F071DBD1CB}" src="https://github.com/user-attachments/assets/f52baf5f-bec9-4aa9-bf4b-6f2c314e1d64" />
Absorption law
<img width="515" height="154" alt="image" src="https://github.com/user-attachments/assets/3addc30c-0687-4d9d-83e1-ba6f3cc0c65d" />
Associative law
<img width="319" height="358" alt="{ABF59225-39F3-4003-A456-DF374A21F3AE}" src="https://github.com/user-attachments/assets/310d2192-8736-4c69-bf0b-c3d4617641bd" />
Commutative law
<img width="303" height="320" alt="{EAE3C4C5-5A75-4F8A-8014-FFB5C901E592}" src="https://github.com/user-attachments/assets/e0ddc16d-95f1-4881-821a-c7346f2cacd8" />
Null law
<img width="686" height="332" alt="{8D8E3922-BECF-4DC4-A4A9-BED656C4E473}" src="https://github.com/user-attachments/assets/6b57d2eb-6fd8-46a3-a4ca-cfbb8b10cca2" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
 Program to implement the given logic function and to verify its operations in quartus
 using Verilog programming.
MINIMIZATION OF BOOLEAN FUNCTION
i)
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

ii)
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule


**RTL realization**

**Output:**
<img width="973" height="502" alt="Screenshot 2025-10-07 084112" src="https://github.com/user-attachments/assets/4f6b5700-e7d7-4649-befe-17367d92e089" />
<img width="986" height="442" alt="Screenshot 2025-10-07 085057" src="https://github.com/user-attachments/assets/5a39d35c-dc98-4de7-87e1-2f8b23ba2eb6" />

**RTL**

**Timing Diagram**
<img width="913" height="830" alt="{84A48B65-E3F7-4B92-AC3E-2F18D14E3F8A}" src="https://github.com/user-attachments/assets/faa33f4b-a857-4e23-8f19-fbceac13838f" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

