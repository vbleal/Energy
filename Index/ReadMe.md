# Energías Renovables - Índice Bursátil

Creado por:

*  **V. D. Betancourt**


<img src="https://github.com/vbleal/Energy/blob/main/zImag/Ban_Energy_Index.gif" width="1000" height="300">

<sub>Créditos: Basado en Diseño Canvalisa.</sub>





<br>

---

## 📃 Introducción


<details>
<summary>Expandir </summary>

<br>


### 📄 Descripción

El presente proyecto pertenece al ámbito de las **Energías Renovables**. En particular, está enfocado en datos del **Índice Bursátil** de una **Empresa**.



<br>

### 🎯 Objetivo

El presente proyecto tiene como finalidad estudiar la **Índice Bursátil de la Empresa**, por medio de:

* Generar un *Análisis Exploratorio de Datos*, incluyendo diversas visualizaciones diseñadas en Seaborn.

* Generar un *Análisis de Riesgo de Mercado* por medio del cálculo del Value-at-Risk (VaR).

* Generar *Predicciones* con diferentes modelos, tales como: Redes Neuronales y Series Temporales.


  
</details>









<br>

---

## 🗃️ Datos


<details>
<summary>Expandir </summary>

<br>

Los datos empleados del Índice Bursátil de la Empresa se extraen desde la plataforma de datos llamada **Yahoo Finance**, usando código de Python.





  
</details>













<br>

---

## 🧮 Modelo


<details>
<summary>Expandir </summary>

<br>

### Modelo de Redes Neuronales para Predicciones Pasadas y Futuras

<br>

<img src="https://github.com/vbleal/Energy/blob/main/Index/Imag/adxmc_model_nn.png" width="500" height="300">



  
</details>









<br>

---
##  📊 Resultados

<details>
<summary>Expandir </summary>

<br>



<details>
<summary>ANÁLISIS EXPLORATORIO DE DATOS (EDA) </summary>

<br>

### Evolución del Precio ('Close') del Índice


<img src="https://github.com/vbleal/Energy/blob/main/Index/Imag/adxmc_evolution_close.png" width="1000" height="500">



<br>
<br>

### Estadística Descriptiva del Precio ('Close') del Índice por Año


<img src="https://github.com/vbleal/Energy/blob/main/Index/Imag/adxmc_yearly_close_stat.png" width="600" height="350">




<br>
<br>


### Velas Japonesas 


#### Con Período Semanal

<br>

<img src="https://github.com/vbleal/Energy/blob/main/Index/Imag/adxmc_candle_weekly.png" width="500" height="400">


<br>
<br>

#### Últimos Meses

<br>

<img src="https://github.com/vbleal/Energy/blob/main/Index/Imag/adxmc_candle_last_months.png" width="500" height="400">


<br>
<br>

#### Gráfico de Línea

<br>

<img src="https://github.com/vbleal/Energy/blob/main/Index/Imag/adxmc_candle_line.png" width="500" height="400">





<br>
<br>

### Boxplot 


<img src="https://github.com/vbleal/Energy/blob/main/Index/Imag/adxmc_boxplot.png" width="700" height="450">




<br>
<br>

### Boxplot 


<img src="https://github.com/vbleal/Energy/blob/main/Index/Imag/adxmc_violinplot.png" width="700" height="450">







</details>





<br>
<br>


<details>
<summary>RIESGO DE MERCADO </summary>

<br>

### VaR por Metodología Histórica (VaR Hist)

<br>

El cálculo del **VaR por Metodología Histórica** (abreviado **VaR Hist**) utiliza datos históricos para simular posibles pérdidas futuras y determinar el umbral de pérdida correspondiente al nivel de confianza seleccionado.

<br>

**Resultado**: 

* El VaR Histórico al 95.0% de nivel de confianza obtenido para el Índice fue: **-4.03%**.

* Esto equivale a una **pérdida potencial** de **€4,026.84** por cada €100,000 invertidos.

<br>

**Interpretación**: 

* Bajo condiciones normales de mercado, 
existe un **95% de probabilidad** de que 
se obtenga una **pérdida no mayor que €4,026.84**. 
Esto es el **4.03%** del total invertido (€100,000). 

* Por lo tanto, existe un **5% de probabilidad** 
de que, en un día, se consiga una **pérdida mayor que €4,026.84**.






<br>
<br>

### VaR por Simulación Monte Carlo (VaR SMC)

<br>

El cálculo del Value-at-Risk (VaR) usando **Simulación Monte Carlo** (abreviado **VaR SMC**) es un método más complejo que la metodología histórica, pero ofrece la ventaja de poder modelar escenarios futuros basados en estimaciones estadísticas.

Este enfoque utiliza la simulación aleatoria para generar posibles resultados futuros basados en los retornos históricos, permitiendo calcular el VaR bajo diversas condiciones de mercado.


<br>

**Resultado**: 

* El VaR por Simulación Monte Carlo al 95.0% de nivel de confianza obtenido para el Índice fue: **€5,426.28**

<br>

**Interpretación**: 

* Bajo condiciones normales de mercado, existe un **95% de probabilidad** 
de que se obtenga una **pérdida no mayor que €5,426.28** en el próximo día.






</details>









<br>
<br>


<details>
<summary>PROYECCIONES </summary>

<br>


### 🔮 Predicciones Pasadas

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Index/Imag/adxmc_model_nn_hist_pred_pasadas.png" width="1000" height="500">





<br>


### 🔮 Predicciones Futuras

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Index/Imag/adxmc_model_nn_pred_futuras.png" width="1000" height="500">

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Index/Imag/adxmc_model_nn_hist_pred_futuras.png" width="1000" height="500">









</details>

  
</details>








<br>

---
## 💼 Documentación


<details>
<summary>Expandir </summary>

<br>

<details>
<summary>Reporte </summary>

<br>

*  [Reporte PDF con Código](https://github.com/vbleal/Energy/blob/main/Index/Doc/Energ%C3%ADas%20Renovables%20-%20Index.pdf)

<br>







</details>

</details>
















<br>

---

