# Curso Data Science - Ingenias - Fundación YPF + Media Chicas   :woman_student: :woman_technologist:

<p align="center">
      <img src=https://github.com/mdcorva/Proyecto-energia-renovable-Argentina/blob/main/logo.png width="300">
</p>


### Integrantes: 
- Eugenia Aciar [**LinkedIn**](https://www.linkedin.com/in/eugenia-aciar/)
- Eileen Corbalán [**LinkedIn**](https://www.linkedin.com/in/eileen-corbalan/)
- Dolores Corva [**LinkedIn**](https://www.linkedin.com/in/m-dolores-corva/)
- Julia Panei [**LinkedIn**](https://www.linkedin.com/in/julia-panei/)
- Evelin Paez 

### Objetivo del proyecto :computer: :
Predecir la contribución de las fuentes de energías renovables a la satisfacción de la demanda eléctrica del país. 

#### Origen del Dataset:
El dataset se descargó de la página de CAMMESA (Compañía Administradora del Mercado Mayorista Eléctrico Sociedad Anónima). 

#### Descripción del dataset  :
Este dataset contiene la información de la energía generada por fuentes de Energías Renovables y su contribución al sistema eléctrico de Argentina. 
La Base de Datos es de paso mensual, desde enero 2011 hasta junio de 2023, conteniendo los siguientes campos con una cantidad total de 15999 registros. 

#### **Diccionario de variables  :bookmark::**
|**Feature**|**Descripción**|
|-----------|---------------|
|anio       | Año           |
|central    | Siglas del nombre de la central energética|
|central_des| Nombre completo de la central energética|
|maquina    | Nombre de la máquina utilizada en la central|
|fuente_de  | Tipo de guente de energía renovable: biodisel, hidrúlico, eólico, solar, biomasa|
|region     | Región del país donde se encuentra la central|
|energia_gen| Energía Generada en GWh por la central en el mes y año correspondiente|
|prov       | Provincia donde se ubica la central|
|mes        | Mes del año abreviado a las primeras tres letras|
      
## Desarrollo :chart_with_upwards_trend:
Se comenzó con un exhaustivo Análisis Exploratorio de los datos (EDA) que nos permitió responder preguntas como: ¿Cuál es la cantidad de datos que tenemos por año? ¿Cuánta energía de fuentes renovables se produjo por año?, entre otras. 

De todas formas, nuestra pregunta principal es: **¿Cuánta energía eléctrica se generará a partir de cada fuente de energía renovable?**. Para responderla utilizamos aprendizaje supervisado.  
Como la variable que queremos predecir , es una variable numérica continua decidimos probar con distintos MODELOS DE REGRESIÓN. Para esto, en primer lugar se crearon distintos datasets correspondientes a cada fuente de energía  y luego se convirtieron todas las variables categóricas a variables numéricas. Estos modelos de regresión fueron: Regresión Lineal, RandomForest y Support Vector Machine. 

Finalmente podemos concluir que con el dataset elegido, con el EDA y con los modelos elegidos pudimos correr un modelo completo en particular para la energía **solar** y podría considerarse que los resultados no fueron malos y sí responden a nuestra pregunta principal. 
