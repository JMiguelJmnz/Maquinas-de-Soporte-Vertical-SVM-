# Maquinas de Soporte Vertical (SVM)

análisis de clasificación mediante Máquinas de soporte vectorial que permita desarrollar un modelo predictivo para analizar porqué los empleados deciden irse con la competencia.

después de haber limpiado y pre procesado la información, dividimos nuestras bases de entrenamiento y prueba.
<br>![image](https://github.com/user-attachments/assets/14e115ea-13ca-4d17-a0a0-5ad817bee69a)

***Radial Basis function***

Comenzando con la utilización del kernel RBF para SVM realizamos el modelo y su mapa de calor para observar cómo se comporta
<br>![image](https://github.com/user-attachments/assets/987932a4-440d-4542-87cc-78ffb7d2f729) ![image](https://github.com/user-attachments/assets/69a5504e-f246-4319-a962-75aba375373e)

La utilización del kernel Radial Basis Function (RBF) no resulta ser muy óptimo para este caso ya que aunque no tuvo errores con el personal que no dejó la compañía, hace una pobre estimación de los que sí se fueron que es el factor más importante de este estudio.
<br>![image](https://github.com/user-attachments/assets/6b8c1359-9673-421f-9664-ef2598a913fd)

***Linear***

Continuamos con el modelo linear
<br>![image](https://github.com/user-attachments/assets/c55806e3-c623-4cfc-9291-e5e086e0038a) ![image](https://github.com/user-attachments/assets/9063c825-f9eb-4b6f-8e59-59f8acd5ff57)

Aunque este kernel (lineal) mejora contra el anterior, sigue realizando un pronóstico pobre sobre el factor importante y el pronóstico acertado de los empleados que se fueron sigue siendo opacado por los errores que tuvo, convirtiéndolo en una herramienta poco útil para este caso

<br>![image](https://github.com/user-attachments/assets/6e5a80c1-52a6-496d-a429-18819a7a0441)

***Polinomial***

<br>![image](https://github.com/user-attachments/assets/27215a1f-5de2-409d-b34a-21a5ed463c01) ![image](https://github.com/user-attachments/assets/1582c869-ab63-4a93-ada1-2382a63eb876)

El kernel polinomial fue incapaz de determinar si un empleado deja la compañía, descartando este método, también demuestra que tener un valor alto en un aspecto, como sería aquí los valores pronosticados contra los reales de los que se quedan en la compañía, no tienen utilidad si no hay un porcentaje aceptable de los empleados que se fueron.
<br>![image](https://github.com/user-attachments/assets/86eacfee-d723-404b-850b-3aa0cc61147e)

***Sigmoidal***
<br>![image](https://github.com/user-attachments/assets/235fc2d0-2497-4a16-939d-cf197d4c161e) ![image](https://github.com/user-attachments/assets/caa7364f-7527-4bbe-9646-6b4ab911af90)

El kernel Sigmoidal parece ser el más apropiado para este caso debido a tener el balance más óptimo de los casos anteriores, es el modelo que obtuvo un mayor número del factor que resulta más importante determinar que en este caso es los empleados que se fueron de la compañía y aunque no es óptimo, o confiable, los errores obtenidos se balancean entre sí, lo que nos permite usar este método para obtener cierta informacion util pero la utilización de otro metodo u optimización de los datos sería recomendado.
<br>![image](https://github.com/user-attachments/assets/0adbdcb6-8807-421e-a00b-697e1fe2d4bf)

Tomando este último método como el más adecuado y utilizándolo para predecir el resultado del siguiente empleado:
<br>![image](https://github.com/user-attachments/assets/3025b7b6-2f9d-423a-8f70-a363be200997)

Obtenemos que el empleado se quedara en la compañía.
<br>![image](https://github.com/user-attachments/assets/9fbc713c-8388-4a3e-9c6c-05e20951b002)
