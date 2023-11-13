### Alura Challenge: Robot trading BTC-USD 🤖📈

*Robot Trading BTC-USD* es un algoritmo de decisión simple automatizado capaz de tomar decisiones de compra y venta de Bitcoin en tiempo real y está desarrollado en el entorno virtual Google Colaboratory.

El resultado de este código será un gráfico mostrando un periodo de los ultimos 7 días del precio BTC-USD y la decisión del algoritmo en tiempo real, basado en datos normalizados y limpios, que se actualizarán cada 5 minutos.

### **Librerias utilizadas:**
- *Pandas*
- *Numpy*
- *Matplotlib*
- *yfinance*
- *BeautifulSoup*
- *time*

#### 1. Configuración del ambiente:  ⚙
Importando librerías esenciales como Pandas, Numpy, Matplotlib, etc.

#### 2. Obtención de datos: ⛏
 - Recopilación de datos de los ultimos 7 días de BTC-USD en formato JSON mediante la API yfinance.
 - Extracción de precio actual y de indicadores de alta y baja del precio en la ultima hora, mediante Web Scraping en sitio de noticias (https://coinmarketcap.com/)

#### 3. Limpieza de datos: 🧹
Transformación a Dataframe para la identificación y eliminación de outliers y tratamiento de valores nulos. Obtención del precio promedio del Bitcoin.

#### 4. Tomar decisiones: 🤔
Algoritmo de decisión que compara el precio actual y la tendencia. Si el precio es mayor/igual que la media y la tendencia es de baja, entonces se debe vender, pero si el precio actual es menor que la media y la tendencia es de alta, entonces se debe comprar.

#### 5. Visualización: 📈
Creación de gráfico que muestra la evolución del precio BTC-USD durante el periodo de 7 días implementando la librería Matplotlib. Se genera una línea recta que muestra el precio medio y se imprime un mensaje en el gráfico con la acción a realizar “Vender”, “Comprar” o “Esperar".

#### 6. Automatización: 🤖
Ejecución automatizada de las funciones, adicionando la librería "time" para ejecutar cada 5 minutos y actualizar el gráfico.

![](https://github.com/geeorgebixleer/robot-trading-BTC-USD/blob/main/insignia_robot_trading.png)
