# LAB_4

# OBJETIVOS

## OBJETIVO GENERAL 
 
* Demostrar el teorema de superposición con el uso de calculos y el simulador de circuitos tinkercad para sustentar conocimientos teóricos.

## OBJETIVO ESPECIFICO


# MARCO TEORICO

![Superposicion-teorico](https://user-images.githubusercontent.com/93361435/147123371-db1ebed1-6591-48df-8a93-772a95f5fedf.jpg)

**CODIGO DE COLORES PARA RESISTORES DE 4 BANDAS** 

| DIGITO | COLOR |
|--------|------------|
| 0 | Negro |
| 1 | Café |
| 2 | Rojo |
| 3 | Naranja |
| 4 | Amarillo |
| 5 | Verde |
| 6 | Azul |
| 7 | Violeta |
| 8 | Gris |
| 9 | Blanco |

TOLERANCIA : Oro +- 5%; Plata +- 10%.


# PROCEDIMIENTO

**Se utilizo los siguientes materiales:** 

| CANTIDAD | MATERIAL |
|--------|------------|
| 2 | Fuente de voltaje en C.D. |
| 2 | Multimetro Digital |
| 1 | Resistor de 1 Kilo-Ohmios |
| 1 | Resistor de 470 Ohmios |
| 1 | Resistor de 820 Ohmios |
| 1 | Resistor de 2.2 Kilo-ohmios |
| 1 | Protoboard |

Se procede a armar el circuito de la figura en tinkercad: 

![image](https://user-images.githubusercontent.com/93361435/147123612-12e60421-4512-4404-b8ea-61c287b838be.png)

Se midio la corriente y el voltaje en el lugar requerido. 

Luego se procedio a reemplazar una de las fuentes por su resistencia interna y se realizo la medición de voltaje y corriente en el lugar requerido, se realizo el mismo proceso para la otra fuente de voltaje, estos valores fueron anotados en una tabla para su respectivo análisis. 

**CIRCUITO 1 (12 V)** 

Para el procedimiento teorico en primer lugar se sustituyo la fuente de 20 V por su resistencia interna y se realizo los siguientes calculos: 

![Superposicion 1](https://user-images.githubusercontent.com/93361435/147174889-344dcbd0-0aa6-46c2-a3be-2339960901ad.png)

Para la medición en tinkercad como se dijo anteriormente se reemplaza la fuente de 20 V por su resistencia interna y se midio el voltaje y corriente requeridos y se obtuvo los siguientes resultados: 

![image](https://user-images.githubusercontent.com/93361435/147174953-51f43e0e-4de2-436b-b4ee-a49962e8312e.png)

#### CIRCUITO 2 (20 V)

- como primer paso se procede a cambiar la fuente de 12v por un cable, es decir, la ponemos en corto de la siguiente manera:  
![image](https://user-images.githubusercontent.com/93398718/147181441-af81e229-35cb-4cb9-95ff-2e56406369e6.png)
- debemos tomar en cuenta que el cable que esta en paralelo con R4 pone a R4 en corto de modo que su resistencia es cero. de esta manera obtenemos un circuito con R3 y R2 en paralelo, el cual se resuelve de la siguiente manera:    
![image](https://user-images.githubusercontent.com/93398718/147181853-d6b3c3a9-3042-46cc-af1d-757946331b81.png)    
![image](https://user-images.githubusercontent.com/93398718/147182083-c108681f-1e35-4b00-9952-25d31e9ca668.png)  
![image](https://user-images.githubusercontent.com/93398718/147182183-bf7b9900-bd59-4426-a14d-db9f2c511544.png)  
- como se puede notar, ahora disponemos de un circuito con dos resistencias en serie, de tal manera que hacemos uso del divisor de voltaje para hallar el voltaje de REQ.      
![image](https://user-images.githubusercontent.com/93398718/147182578-308371d2-0cb1-4eca-aa5b-7e45a39487f1.png)  
- debemos recordar que REQ es resultado de R2 y R3 las cuales se encontraban en paralelo, por tal motivo el voltaje de REQ es el mismo que el de R2 y R3, de esta manera podemos determinar que VA es lo siguiente:    
![image](https://user-images.githubusercontent.com/93398718/147183052-cc71b69e-6b57-4343-ae63-b2fc55d8a8de.png)  
- para la corriente en Ix podemos asumir que sera la misma que la corriente en VA, sin embargo el cable que esta en paralelo con R4 provoca que esta resistencia tienda a cero, de manera que Ix=0 en este analisis.



 


# RESPUESTA DE INTERROGANTES Y CALCULO DE ERROR

**CIRCUITO 1 (12 V)** 

Tabulando los datos obtenidos anteriormente: 

|Corriente IX Medido | Corriente IX Calculado | Voltaje VA Medido | Voltaje VA Calculado|
|--------------------|------------------------|-------------------|---------------------|
| 25.5 mA | 25.53 mA | 6.53 V | 6.527 V|

El respectivo calculo del error es: 

- Para la corriente IX: 
   ![image](https://user-images.githubusercontent.com/93361435/147175507-1af68fc9-069e-4e20-901f-170f7b21f4bb.png)
- Para el voltaje VA: 
   ![image](https://user-images.githubusercontent.com/93361435/147175609-21769281-79f6-49b5-9390-a38f16cd00f3.png)


**CIRCUITO 2 (20 V)**

**CIRCUITO 3 (12 Y 20 V)**

Una vez que se obtuvo los datos de la resistencia y el voltaje en los 2 diferentes casos, se procede a calcular la corriente total en la resistencia 4 (R4) de valor de 470 ohmios, como se observa las 2 corrientes tiene el mismo sentido, debido a esto tenemos que sumar los 2 corrientes que se obtuvo para así hallar la corriente total, y su valor es de 25,5 mA.

De la mima manera se hace con el voltaje, en este caso los voltajes se tienen que restar ya que no tienen el mismo sentido, se obtiene el resultado de 952 mV.

Para verificar los resultado anteriores, se procede a realizar el circuito en un simulador, en este caso se utilizó el simulador Tinkercad.

![image](https://user-images.githubusercontent.com/93561706/147183327-d147fb7f-f281-4119-bee0-2f9e69d1156a.png)

Como se logra observar los resultados antes mencionados son los mismos que se obtuvo en el simulador, por ende se confirma que el procedimiento estuvo bien elaborados.

# VIDEO


# CONCLUSIONES


# BIBLIOGRAFIA

- Floyd, T. (2007). *Principios de circuitos eléctricos*. Octava edición. Mexico. Editorial Pearson.
- Robbins, A., Miller, W. (2008) *Analisis de circuitos Teoria y Practica*. Cuarta Edicion. Mexico. Editorial CENGAGE Learning.

