        Del Dato al Negocio:Modelos Predictivos para Impulsar el Crecimiento Bancario


        Introducción: 
En un contexto altamente competitivo, donde los márgenes bancarios dependen cada vez más de la capacidadde anticipar el comportamiento de los clientes, 
este proyecto surge como una respuesta estratégica paratransformar datos históricos en decisiones comerciales inteligentes.Mediante el desarrollo de modelos avanzados de machine learning, 
se ha buscado predecir qué clientes tienenmayor probabilidad de adquirir productos financieros clave como préstamos personales o tarjetas de crédito.

        El objetivo final es claro: 
Optimizar los esfuerzos de marketing directo,Reducir costos operativos,Y maximizar los ingresos, captando oportunamente a los clientes con el mayor potencial.


Este proyecto no solo ofrece un análisis técnico sólido, sino que traza una hoja de ruta práctica paraimplementar los modelos desarrollados en la toma de decisiones comerciales del banco. Para ello, sedesarrollaron y compararon dos modelos predictivos:LightGBM (modelo de boosting)Random Forest (modelo de bagging)Ambos entrenados sobre datos históricos de transacciones de clientes, con balanceo de clases para asegurarque los modelos aprendieran adecuadamente a identificar el segmento minoritario (clientes con altaprobabilidad de adquirir un producto).

        Supuestos del escenario para la simulación

![image](https://github.com/user-attachments/assets/9533ac7d-b719-46ba-a97c-1d4cdf8ade86)


        Datos clave de los modelos

Se evaluaron múltiples métricas, pero dado nuestro objetivo de negocio (maximizar clientes
captados), nos centramos principalmente en:

* Recall (sensibilidad): para captar el mayor porcentaje posible de clientes realmente
interesados.
* Precision: % de predicciones positivas que eran correctas (muchos falsos positivos en este
caso)

![image](https://github.com/user-attachments/assets/10bc26b0-288d-4dbb-8c2a-493dd08fe60c)



        Simulación costo - beneficio

Esto depende de la cantidad de positivos predichos por cada modelo. Podemos aproximarlo
usando la siguiente fórmula:

* N° clientes contactados ≈ TP + FP = TP / Recall

![image](https://github.com/user-attachments/assets/30781b7a-63ac-4d28-b13c-f31509dbc00b)


        Costo total de la campaña

![image](https://github.com/user-attachments/assets/52ff70bd-8a23-4cfc-8bca-ecefc4e1a6a3)


        Ganancia total - Clientes captados por beneficio

![image](https://github.com/user-attachments/assets/1437aebb-293c-4aaa-b8a9-a256531fb5d8)

        
        Beneficio Neto Por Modelo

![Screenshot 2025-07-02 091811](https://github.com/user-attachments/assets/b6e42382-3cd2-4b68-bbee-00782f924d40)


        Estrategia de captación con LightGBM

Dado su altísimo recall (94%), el modelo LightGBM se alinea perfectamente con una estrategia agresiva de
marketing directo donde:

* Preferimos contactar más clientes, incluso con algunos falsos positivos, asegurando así que muy pocos
clientes interesados se pierdan.
* Esto permite maximizar los ingresos derivados de nuevas contrataciones, fortaleciendo el crecimiento de la
cartera activa del banco.


        Con base en los resultados obtenidos:

LightGBM es el modelo óptimo para implementar en la campaña
de captación de préstamos y tarjetas, ya que permite capturar el
70% más de clientes interesados que Random Forest,
traduciéndose en una rentabilidad neta significativamente mayor.

Adicionalmente, al tener un AUC de 0.87, garantiza un
desempeño robusto ante futuros cambios en el mercado,
facilitando la escalabilidad del modelo a nuevos segmentos de
clientes.

        Conclusión general

En un contexto altamente competitivo, donde los márgenes bancarios dependen cada vez más de la capacidad
de anticipar el comportamiento de los clientes, este proyecto surge como una respuesta estratégica para
transformar datos históricos en decisiones comerciales inteligentes.

Mediante el desarrollo de modelos avanzados de machine learning, se ha buscado predecir qué clientes tienen
mayor probabilidad de adquirir productos financieros clave como préstamos personales o tarjetas de crédito.
Conclusión general

Comparado con enfoques tradicionales o modelos alternativos, esta solución logra:

* Un recall de hasta el 94%, asegurando que casi ningún cliente potencial se pierda.
* Un beneficio económico neto un 47% superior, maximizando el retorno sobre cada dólar invertido en
campañas.

Esto posiciona al banco a la vanguardia del uso de analytics para potenciar su crecimiento, permitiendo tomar
decisiones proactivas, eficientes y completamente orientadas a resultados.

Con esta base sólida, se abren las puertas a estrategias futuras de cross-selling, personalización y fidelización
que consolidarán la ventaja competitiva del banco en el mercado.
