# Energías Renovables - Análisis Financiero y de Resultados

Creado por:

*  **V. D. Betancourt**


<img src="https://github.com/vbleal/Energy/blob/main/zImag/Ban_Energy_Financials.gif" width="1000" height="300">

<sub>Créditos: Basado en Diseño K. Chistiakova.</sub>





<br>

---

## 📃 Introducción


<details>
<summary>Expandir </summary>

<br>


### 📄 Descripción

El presente proyecto pertenece al ámbito de las **Energías Renovables**. En particular, está enfocado en datos de **Estados Financieros y de Resultados** de una **Empresa**.



<br>

### 🎯 Objetivo


El presente proyecto tiene como finalidad estudiar la **Información Financiera Anual de la Empresa**, del **2011** al **2023**, por medio de:

* Generar un *Análisis Exploratorio de Datos*, incluyendo diversas visualizaciones diseñadas en Seaborn.

* Generar *Predicciones* con diferentes modelos, tales como: Redes Neuronales y Regresión Múltiple.

  
</details>









<br>

---

## 🗃️ Datos


<details>
<summary>Expandir </summary>

<br>


Se ha creado un fichero en MS Excel, llamado **`'fin_data_energy.xlsx'`**, con la **Información Financiera Anual** de la Empresa, disponible en su sitio web, por lo que es *información pública*.

El dataset **`'fin_data_energy.xlsx'`** consta de **17 campos** que se describen a continuación.

<br>

### Cuentas de Referencia

* **`Fecha`**: Indica cuándo se recogieron o reportaron los datos financieros.

* **`Empresa`**: El nombre de la empresa a la que pertenecen los datos financieros. Aunque el Análisis de este proyecto trata de una sola Empresa, el dataset hace distinción entre 2 empresas debido al cambio de nombre de la empresa original, a partir de 2015.



<br>

### Cuentas del Balance

* **`Activo no corriente`**: Se refiere a los activos que no se espera que se conviertan en efectivo o que no se usarán dentro de un año. Ejemplos incluyen bienes inmuebles, maquinaria y patentes.

* **`Activo corriente`**: Incluye todos los activos que se espera que se conviertan en efectivo, se vendan o se consuman en el plazo de un año o menos. Ejemplos comunes son el efectivo, inventarios y cuentas por cobrar.

* **`Total Activo`**: La suma de los activos corrientes y no corrientes. Representa todos los recursos económicos controlados por la empresa.

* **`Patrimonio neto`**: También conocido como capital propio, es el valor residual de los activos de la empresa menos sus pasivos. Es básicamente lo que los propietarios de la empresa poseen.

* **`Pasivo no corriente`**: Deudas o obligaciones financieras que no se espera que sean liquidadas dentro del próximo año fiscal. Ejemplos incluyen préstamos a largo plazo y bonos emitidos.

* **`Pasivo corriente`**: Deudas o obligaciones que deben ser pagadas dentro de un año. Incluye cosas como cuentas por pagar, deudas a corto plazo y otros pasivos a corto plazo.

* **`Total Pasivo`**: Representa la suma de los pasivos corrientes y no corrientes.

* **`Total Pasivo y Patrimonio`**: Es la suma del Patrimonio neto y el Total Pasivo.




<br>

### Cuentas de Resultados

* **`Ingresos de las operaciones`**: Los ingresos generados por las actividades principales de la empresa, excluyendo los ingresos extraordinarios.

* **`Margen Bruto`**: Los ingresos de las operaciones menos el costo de los bienes vendidos. Es una medida de la eficiencia de producción y ventas de la empresa.

* **`EBITDA`**: Acrónimo de "Earnings Before Interest, Taxes, Depreciation, and Amortization" (Ganancias antes de intereses, impuestos, depreciación y amortización). Es un indicador de la rentabilidad operativa de la empresa antes de ciertos factores financieros y contables.

* **`EBIT`**: Acrónimo de "Earnings Before Interest and Taxes" (Ganancias antes de intereses e impuestos). Similar al EBITDA pero sin excluir la depreciación y la amortización.

* **`Resultado antes de impuestos`**: Las ganancias de la empresa antes de que se hayan deducido los impuestos. Indica la rentabilidad antes de la intervención fiscal.

* **`Resultado consolidado del ejercicio`**: Las ganancias totales de la empresa, incluyendo todas sus subsidiarias, después de deducir gastos e impuestos.

* **`Resultado neto atribuible a la sociedad dominante`**: El beneficio neto que corresponde a la empresa matriz después de considerar los intereses de minoritarios y otros factores. Es la parte del beneficio neto que realmente pertenece a la empresa controladora.



<br>

### Notas importantes

* La información original se encuentra en **miles de euros**.

* El dataset **`'fin_data_energy.xlsx'`** contiene los datos en **euros**.

* En este Proyecto/Notebook, se toma la información en euros del dataset **`'fin_data_energy.xlsx'`** y se trabaja en **millones de euros**.

* Se identificó en la información original que el campo **`'Total Pasivo'`** incluía los datos del Pasivo y del Patrimonio. Con la finalidad de ahorrar tiempo, el dataset **`'fin_data_energy.xlsx'`** contiene la separación de esta información. Es decir, ahora **`'Total Pasivo'`** contiene sólo los datos de los Pasivos, se creó una nueva columna para el **`'Patrimonio neto'`**, y el **`'Total Pasivo y Patrimonio'`** es la suma de los 2 campos anteriores.


  
</details>













<br>

---

## Modelo


<details>
<summary>Expandir </summary>

<br>

### Modelo de Redes Neuronales

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/Modelo_NN_Financials.png" width="500" height="370">


  
</details>









<br>

---
##  📊 Resultados

<details>
<summary>Expandir </summary>

<br>



<details>
<summary>BALANCE </summary>

<br>

### Evolución Anual del Activo, Pasivo y Patrimonio Neto


<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/Balance_Barplot_Hist.png" width="900" height="1000">



<br>
<br>


### Pairplot: Activo, Pasivo, y Cuentas de Resultados

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/Pairplot_Balance_Resultados.png" width="900" height="1000">




<br>
<br>

### Gráficos KDE


<br>

#### Distribución del Activo Corriente

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/KDE_AC.png" width="400" height="300">




<br>

#### Distribución del Pasivo Corriente

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/KDE_PC.png" width="400" height="300">






<br>
<br>

### Lineplots

<br>

#### Tendencia de Activos y Pasivos

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/Lineplot_Subplots_Activos_Pasivos.png" width="1000" height="400">



<br>

#### Tendencia de Activos y Pasivos en Conjunto

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/Lineplot_Activos_Pasivos.png" width="800" height="500">






<br>
<br>

### Heatmap

<br>

#### Correlaciones

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/Heatmap.png" width="800" height="500">





<br>

#### Correlaciones Positivas

<br>
<img src="" width="500" height="300">




<br>

#### Correlaciones Negativas

<br>
<img src="" width="500" height="300">






</details>





<br>


<details>
<summary>CUENTAS DE RESULTADOS </summary>

<br>

### Evolución Anual de las Cuentas de Resultados


<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/Resultados_Barplot_Hist.png" width="1000" height="1100">






<br>
<br>

### EBITDA vs Resultado Consolidado

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/Scatterplot_EBITDA_Res.png" width="500" height="300">




<br>
<br>


### Gráficos KDE


#### Distribución del EBITDA

<br>

<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/KDE_EBITDA.png" width="500" height="300">



<br>


#### Distribución del Resultado antes de Impuestos

<br>

<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/KDE_Resultados.png" width="500" height="300">






</details>

<br>



<details>
<summary>PROYECCIONES </summary>

<br>


### 🔮 Proyecciones del Balance con Redes Neuronales

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/Pred_NN_Balance.png" width="800" height="450">





<br>


### 🔮 Proyecciones de Cuentas de Resultados con Redes Neuronales

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/Pred_NN_Res.png" width="800" height="450">







<br>


### 🔮 Proyecciones del Balance con Regresión Múltiple

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/Pred_RM_Balance.png" width="800" height="450">






<br>


### 🔮 Proyecciones de Cuentas de Resultados con Regresión Múltiple

<br>
<img src="https://github.com/vbleal/Energy/blob/main/Financials/Imag/Pred_RM_Res.png" width="800" height="450">







</details>

  
</details>








<br>

---
## 💼 Documentación


<details>
<summary>Expandir </summary>

<br>

<details>
<summary>Reporte con Código </summary>

<br>

*  [Reporte PDF con Código](https://github.com/vbleal/Energy/blob/main/Financials/Doc/Energ%C3%ADas%20Renovables%20-%20An%C3%A1lisis%20Financiero%20Empresa.pdf)

<br>







</details>

</details>
















<br>

---
