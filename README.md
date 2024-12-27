# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions 
**boolean experssion**

(i)F1

![WhatsApp Image 2024-12-21 at 23 58 56_76e5bb6d](https://github.com/user-attachments/assets/9b76e370-367a-4a61-9aaf-870377a587bc)

(ii)F2

![WhatsApp Image 2024-12-21 at 23 59 15_5e19b4f9](https://github.com/user-attachments/assets/09cfd01b-6d84-41ba-8b3a-3c15dfab5955)

**Truth Table**

(i)F1

![image](https://github.com/user-attachments/assets/92e559fe-ded8-40ca-81dd-2e300e28e3d6)

(ii)F2

![image](https://github.com/user-attachments/assets/078baebf-e1ab-4c2f-9e21-c7c205b9f250)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.
 
4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:n v mohana krishna 

RegisterNumber:24000587
```

       i)f1

        module funct1(a,b,c,d,f1);
        input a,b,c,d;
        output f1;
        assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
        endmodule

    ii)f2

    module funct2(w,x,y,z,f2);
    input w,x,y,z;
    output f2;
    assign f2=((~y & z)|( w & y )|(x & y));
    endmodule
```


**RTL realization**

(i)F1

![WhatsApp Image 2024-12-24 at 23 34 41_fa6f27a2](https://github.com/user-attachments/assets/bc69fb71-a9f7-4966-8eb1-375a3e8c42e1)

(ii)F2

![min_fun2rtl](https://github.com/user-attachments/assets/707fd939-87eb-4861-b5b8-eab6565db0f2)


**Timing Diagram**

(i)F1

![WhatsApp Image 2024-12-24 at 23 34 49_34d72ac1](https://github.com/user-attachments/assets/dbb9780d-cb07-4064-93da-0bedcae42d21)


(ii)F2
![Screenshot (13)](https://github.com/user-attachments/assets/96394d02-7430-429f-871a-8b6c9e8d2fb2)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

