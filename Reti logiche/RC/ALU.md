---
subject: reti logiche
type: definizione
---
Una ALU o arithmetic logic unit è una [[Rete combinatoria]] in grado di eseguire semplici operazioni aritmetiche e logiche.

Alla base di una ALU vi è un [[Full adder]] che permette di eseguire tutte le operazioni desiderate manipolando i dati in ingresso in base all'operazione che desideriamo.

Un adder a $n$ bit ha i seguenti ingressi
* $A[0\dots n]$ un bus contenente il primo numero
* $B[0\dots n]$ un but contenente il secondo numero
* $C_\text{in}$ flag di carry in, utile per concatenare diverse ALU
* $OpCode[0\dots ?]$ un bus contenente il codice binario dell'operazione da eseguire.

#### OpCode
Per comunicare alla ALU che operazione vogliamo che svolga c'è bisogno sempre di un numero di ingressi che riescano a codificare l'operazione in un numero di bit.
Il codice che corrisponde a una certa operazione varia da macchina a macchina, ma di solito tutte le ALU sono in gradi di svolgere queste basiche operazioni:

Bit di modalità logica disattivato ($M=0$):

| OpCode | $C_\text{in}$=0 | $C_\text{in}$=1 |
|:------:|:---------------:|:---------------:|
|000     |$A-B-1$          |$A-B$            |
|001     |$A+B$            |$A+B=1$          |
|010     |$-B-1$           |$-B$             |
|011     |$B$              |$B+1$            |
|100     |$A-1$            |$A$              |
|001     |$A$              |$A+1$            |
|110     |$2^n-1$ (-1)     |$0$              |
|111     |$0$              |$1$              |

Bit di modalità logica disattivato ($M=1$):

| OpCode |$K_3=0$                           |$K_3=1$         |
|:------:|:--------------------------------:|:--------------:|
|000     |$A\oplus B=A\equiv B$             |$A\equiv B$     |
|001     |$A\oplus B$                       |$A+B$           |
|010     |$0\oplus\overline{B}=\overline{B}$|$A+\overline{B}$|
|011     |$0\oplus B=B$                     |$B$             |
|100     |$A\oplus1=\overline{A}$           |$\overline{A}+B$|
|001     |$A\oplus0=A$                      |$A$             |
|110     |$0\oplus 1=1$                     |$1$             |
|111     |$0\oplus0=0$                      |$AB$            |


![[ALU.svg]]