# Energías Renovables - Potencia y Producción

Creado por:

*  **V. D. Betancourt**


<img src="https://github.com/vbleal/Energy/blob/main/zImag/Ban_Energy_Power.gif" width="1000" height="300">

<sub>Créditos: Basado en Diseño Visula Co.</sub>







<br>

---

## 📃 Introducción


<details>
<summary>Expandir </summary>

<br>


### 📄 Descripción

El presente proyecto pertenece al ámbito de las Energías Renovables, en particular, en datos de **Potencia Instalada y Producción de Energía** de una Empresa para 3 países donde se tiene presencia.



<br>

### 🎯 Objetivo

El principal objetivo de este análisis es comprender el desempeño operativo de la Empresa a lo largo del tiempo mediante el estudio de la **Potencia Instalada y Producción de Energía**, del **2016** al **2023**. Al profundizar en estos datos, se busca identificar patrones, tendencias y posibles anomalías que podrían influir en la toma de decisiones estratégicas de la empresa.

Posteriormente, el análisis pretende establecer una base sólida para el desarrollo de **modelos predictivos**. Estos modelos serán diseñados para **pronosticar futuros valores** de potencia instalada y producción basándose en los datos históricos disponibles. La capacidad de generar predicciones precisas permitirá a la empresa planificar con mayor efectividad sus inversiones, mantenimientos y estrategias de expansión en los mercados energéticos correspondientes.


  
</details>









<br>

---

## 🗃️ Datos


<details>
<summary>Expandir </summary>

<br>

El dataset **`'datos_potencia_prod.xlsx'`** es una recopilación propia basada en la información pública disponible de la Empresa y está conformado por los siguientes **5 campos**:

* **`"Fecha"`**: Fechas del cierre del año desde el 2016 hasta el 2023.

* **`"Empresa"`**: Corresponde al nombre de la "Empresa_1".

* **`"País"`**: Puede ser **`"España"`**, **`"Francia"`**, **`"Polonia"`**.

* **`"Potencia instalada (MW)"`**: Representa la capacidad máxima de producción de energía eléctrica que la empresa puede alcanzar en condiciones óptimas y sin restricciones mecánicas o de otro tipo. Este dato es crucial para evaluar la capacidad y el crecimiento potencial de la infraestructura energética de la empresa.

* **`"Producción (GWh)"`**: Indica la cantidad real de energía generada por la empresa en un año. Este valor es fundamental para analizar la eficiencia operativa de la empresa, así como la utilización efectiva de su capacidad instalada.





  
</details>













<br>

---

## 🧮 Modelo


<details>
<summary>Expandir </summary>

<br>

### 🔮 Modelo de Redes Neuronales para la Predicción de la Potencia Instalada y la Potencia
<br>

<img src="https://github.com/vbleal/Energy/blob/main/Power/Imag/Modelo_NN_Potencia_Prod.png" width="450" height="350">



  
</details>









<br>

---
##  📊 Resultados

<details>
<summary>Expandir </summary>

<br>



<details>
<summary>POTENCIA INSTALADA </summary>

<br>

### Evolución Anual de la Potencia Instalada

<br>

<img src="https://github.com/vbleal/Energy/blob/main/Power/Imag/Potencia_Barplot.png" width="1000" height="1100">



<br>
<br>


### Pairplot: Potencia-Producción

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Power/Imag/Pairplot_Potencia_Prod.png" width="650" height="500">




<br>
<br>

### Gráficos KDE

#### Distribución de la Potencia Instalada (MW)

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Power/Imag/Potencia_KDE.png" width="500" height="350">




<br>
<br>

### Lineplots

#### Tendencia de la Potencia Instalada y Producción por País

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Power/Imag/Potencia_Lineplot_Hist.png" width="750" height="650">






<br>
<br>

### Heatmap

#### Correlaciones entre Potencia Instalada y Producción

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Power/Imag/Heatmap_Potencia_Prod.png" width="650" height="550">


Una correlación de **`0.78`** entre dos variables, como en este caso entre **`"Potencia instalada (MW)"`** y **`"Producción (GWh)"`** sugiere que la relación es fuerte. Esto implica que los cambios en la potencia instalada pueden predecir de manera razonablemente fiable los cambios en la producción de energía.

Aunque una correlación de **`0.78`** es alta, *no es perfecta*. Esto significa que mientras que gran parte de la variabilidad en la producción de energía puede explicarse por cambios en la potencia instalada, hay *otros factores* que también podrían influir en la producción y que no están capturados solo por la potencia instalada.





</details>





<br>


<details>
<summary>PRODUCCIÓN </summary>

<br>

### Evolución Anual de la Producción por País

<br>

<img src="https://github.com/vbleal/Energy/blob/main/Power/Imag/Prod_Barplot.png" width="1000" height="1100">






<br>
<br>


### Gráficos KDE


#### Distribución de la Producción.

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Power/Imag/Prod_KDE.png" width="500" height="350">





<br>
<br>

### Lineplots

#### Tendencia de la Potencia Instalada y Producción por País

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Power/Imag/Prod_Lineplot_Hist.png" width="750" height="650">









</details>

<br>



<details>
<summary>PROYECCIONES </summary>

<br>


### 🔮 Predicciones 2024-2026 de la Potencia Instalada

#### Predicciones de la Potencia Instalada

<br>

<img src="https://github.com/vbleal/Energy/blob/main/Power/Imag/Potencia_Pred.png" width="700" height="450">


<br>
<br>

#### Histórico y Predicciones de la Potencia Instalada

<br>

<img src="https://github.com/vbleal/Energy/blob/main/Power/Imag/Potencia_Hist_Pred.png" width="500" height="350">




<br>
<br>


### 🔮 Predicciones 2024-2026 de la Producción

#### Predicciones de la Producción


<br>

<img src="https://github.com/vbleal/Energy/blob/main/Power/Imag/Prod_Pred.png" width="700" height="450">


<br>
<br>

#### Histórico y Predicciones de la Producción

<br>

<img src="https://github.com/vbleal/Energy/blob/main/Power/Imag/Prod_Hist_Pred.png" width="500" height="350">




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

*  [Reporte PDF con Código](https://github.com/vbleal/Energy/blob/main/Power/Doc/Energ%C3%ADas%20Renovables%20-%20Potencia%20y%20Producci%C3%B3n.pdf)

<br>





</details>

</details>
















<br>

---

