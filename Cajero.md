### **Seudocódigo:** 



Proceso CajeroAutomatico

&nbsp;   // Declaración de variables

&nbsp;   Definir saldo, retiro Como Real;



&nbsp;   // Asignación de saldo inicial

&nbsp;   saldo <- 500;



&nbsp;   // Solicitar la entrada del usuario

&nbsp;   Escribir "Bienvenido. Su saldo actual es: ", saldo;

&nbsp;   Escribir "Por favor, ingrese el monto que desea retirar:";

&nbsp;   Leer retiro;



&nbsp;   // Estructura de decisión: verifica si hay fondos suficientes

&nbsp;   Si retiro <= saldo Entonces

&nbsp;       // Acciones si el saldo es suficiente

&nbsp;       saldo <- saldo - retiro;

&nbsp;       Escribir "Retire su dinero";

&nbsp;       Escribir "Su nuevo saldo es: ", saldo;

&nbsp;   SiNo

&nbsp;       // Acciones si el saldo es insuficiente

&nbsp;       Escribir "Fondos insuficientes";

&nbsp;   FinSi



&nbsp;   Escribir "Gracias por su visita.";



FinProceso



### **Código mermaid:** 





flowchart TD

&nbsp;   INICIO (\[Inicio])

&nbsp;   ENTRADA \[/Solicitar al usuario el monto a retirar/]

&nbsp;   PROCESO1 \[Definir saldo = 500]

&nbsp;   DECISION {¿retiro ≤ saldo?}

&nbsp;   PROCESO2 \[Descontar retiro del saldo]

&nbsp;   SALIDA1 \["Retire su dinero"]

&nbsp;   SALIDA2 \["Fondos insuficientes"]

&nbsp;   FIN (\[Fin])



&nbsp;   INICIO -> PROCESO1 -> ENTRADA

&nbsp;   ENTRADA -> DECISION

&nbsp;   DECISION - Sí -> PROCESO2 -> SALIDA1 -> FIN

&nbsp;   DECISION - No -> SALIDA2 -> FIN



