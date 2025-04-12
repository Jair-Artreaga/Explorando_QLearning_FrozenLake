# Q-Learning en FrozenLake - Análisis de Parámetros de Aprendizaje por Refuerzo

## 📋 Descripción
Este proyecto implementa el algoritmo de Q-Learning en el entorno `FrozenLake-v1` utilizando la librería `gymnasium`. A través de diferentes experimentos, se estudia cómo los parámetros del algoritmo afectan el desempeño del agente. Se realizan entrenamientos con distintas configuraciones y se evalúa el comportamiento aprendido.

## 🎯 Objetivos
Comprender el funcionamiento del algoritmo Q-Learning aplicado al entorno FrozenLake y analizar el efecto de los parámetros clave del aprendizaje por refuerzo sobre el rendimiento del agente.

## 🗂 Estructura del Proyecto
```
📂 Explorando_QLearning_FrozenLake
│── 📂 data  # Datos generados para las pruebas
│── 📂 results  # Resultados y análisis
│── 📄 README.md  # Documentación del proyecto
│── 📄 Q_learning.ipynb  # Implementación en Jupyter Notebook
```

## Instalación y Requisitos
Para ejecutar el proyecto, necesitas tener instalado:
- **Python 3.x**
- **Jupyter Notebook**
- **Librerías necesarias** (se pueden instalar con pip):
  ```bash
  pip install notebook
  ```

## Uso
1. Clona este repositorio:
   ```bash
   git clone https://github.com/Jair-Artreaga/Explorando_QLearning_FrozenLake.git
   ```
2. Accede al directorio del proyecto:
   ```bash
   cd Explorando_QLearning_FrozenLake
   ```
3. Ejecuta Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Abre el archivo `Q_learning` y ejecuta las celdas para ver los resultados.

## Pruebas de Rendimientoo	
El experimento gandor fue el 2, el agente ganó 5 de 5 episodios (100%).
Los parámetros modificados fueron:
- α = 0.9 (alta tasa de aprendizaje)
- γ = 0.99 (factor de descuento muy alto)
- epsilon = 1.0 (exploración total)
- decay = 0.0002 (decadencia más rápida de epsilon)
- episodes = 30000 (mayor número de episodios de entrenamiento)

¿Cuál fue el comportamiento del agente al final del entrenamiento?
- El agente aprendió muy bien debido al alto número de episodios (30000) y el valor elevado de γ = 0.99, que permitió valorar las recompensas futuras. La exploración fue adecuada y la política mejoró de manera significativa.


•	¿Cómo explicarías ese resultado en términos de aprendizaje por refuerzo?
- El éxito del agente puede atribuirse a la combinación de parámetros con un alto valor de α que permitió un rápido aprendizaje de nuevas acciones, un factor de descuento alto (γ=0.99) que promovió la consideración de recompensas a largo plazo, y un número elevado de episodios (30000) que brindó suficientes oportunidades para explorar y ajustar la política del agente. La decadencia más rápida de epsilon también permitió una exploración suficiente al principio y una explotación efectiva al final, lo que resultó en una política óptima al final del entrenamiento.


## Contribuciones
Si deseas contribuir a este proyecto:
1. Haz un fork del repositorio.
2. Crea una rama con tus cambios: `git checkout -b nueva-funcionalidad`
3. Realiza un commit de los cambios: `git commit -m 'Añadir nueva funcionalidad'`
4. Sube los cambios: `git push origin nueva-funcionalidad`
5. Abre un Pull Request.

## Autor
**[Roberto Jair Arteaga Valenzuela]**
