# Gráficos

### Tipos de Gráficos

Matplotlib ofrece una amplia variedad de gráficos. Algunos de los más comunes son:

- **Gráfico de líneas:** Ideal para mostrar tendencias a lo largo del tiempo.

~~~~
import matplotlib.pyplot as plt

plt.plot(x, y)
plt.title("Gráfico de Líneas")
plt.show()
~~~~

![image](https://github.com/user-attachments/assets/61930275-8ef5-4f41-bb5a-60a22d6b41c1)


- **Gráfico de dispersión:** Útil para mostrar la relación entre dos variables.

~~~
plt.scatter(x, y)
plt.title("Gráfico de Dispersión")
plt.show()
~~~

![image](https://github.com/user-attachments/assets/33236d00-7fd8-44af-ba62-a0a085b2b8d6)


- **Gráfico de barras:** Perfecto para comparar categorías.

~~~
plt.bar(categorías, valores)
plt.title("Gráfico de Barras")
plt.show()
~~~

![image](https://github.com/user-attachments/assets/3f8820d4-e974-47c1-a0d9-902d4762e694)


- **Histograma:** Para mostrar la distribución de un conjunto de datos.

~~~
plt.hist(datos, bins=10)
plt.title("Histograma")
plt.show()
~~~

![image](https://github.com/user-attachments/assets/d4760811-9af9-4bc1-9dca-807219084223)


- **Gráfico de pastel:** Para mostrar proporciones de un total.

~~~
plt.pie(valores, labels=categorías)
plt.title("Gráfico de Pastel")
plt.show()
~~~

![image](https://github.com/user-attachments/assets/ede27a91-63a9-4332-be8e-0f68b9652a35)


- **Gráfico de cajas:** Para visualizar la distribución de datos y detectar outliers.

~~~
plt.boxplot(datos)
plt.title("Gráfico de Cajas")
plt.show()
~~~

![image](https://github.com/user-attachments/assets/dcd22ea1-cac5-44da-9dfa-c8c0ac310247)



### Estilos para una Presentación Más Profesional

Matplotlib permite personalizar el estilo de los gráficos para que se vean más profesionales. Aquí hay algunos consejos:

- **Cambiar el estilo general**: Usa estilos predefinidos como `ggplot`, `seaborn`, o `bmh`.
  ```
  plt.style.use('seaborn')
  ```

- **Ajustar la paleta de colores**: Utiliza paletas de colores que sean agradables a la vista.
  ```
  plt.plot(x, y, color='dodgerblue')
  ```

- **Mejorar etiquetas y títulos**:
  ```
  plt.title("Título del Gráfico", fontsize=14, fontweight='bold')
  plt.xlabel("Eje X", fontsize=12)
  plt.ylabel("Eje Y", fontsize=12)
  ```

- **Modificar la cuadrícula**: Haz que la cuadrícula sea más sutil.
  ```
  plt.grid(alpha=0.3)
  ```

- **Ajustar el tamaño de la figura**:
  ```
  plt.figure(figsize=(10, 6))
  ```

- **Usar anotaciones**: Añade anotaciones para resaltar puntos clave.
  ```
  plt.annotate('Texto de Anotación', xy=(x_val, y_val), xytext=(x_offset, y_offset),
               arrowprops=dict(facecolor='black', shrink=0.05))
  ```

