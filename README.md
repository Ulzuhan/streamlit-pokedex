# 🔴 Pokédex Interactiva

Una aplicación web interactiva para explorar y comparar Pokémon, construida con **Streamlit** y potenciada por datos de la **PokéAPI**.

## 📋 Descripción

Esta es una Pokédex moderna e interactiva que permite a los usuarios explorar información detallada sobre los primeros Pokémon. La aplicación ofrece múltiples formas de interactuar con los datos, incluyendo búsqueda, filtrado avanzado y comparación de stats.

## ✨ Características

- 🔍 **Búsqueda por nombre**: Encuentra Pokémon rápidamente escribiendo su nombre
- 🏷️ **Filtrado por tipo**: Selecciona uno o múltiples tipos (fuego, agua, eléctrico, etc.)
- 👑 **Filtro de legendarios**: Visualiza solo los Pokémon legendarios
- 📊 **Filtro por stats**: Establece un mínimo de total de stats para búsquedas más específicas
- 📈 **Gráficos de radar**: Visualiza los stats (HP, Ataque, Defensa, etc.) de cualquier Pokémon
- ⚖️ **Comparador**: Compara directamente dos Pokémon lado a lado con sus stats superpuestos
- 🎨 **Interfaz moderna**: Diseño limpio y responsivo con tema oscuro
- 📱 **Galería visual**: Explora Pokémon en un formato de cartas ajustables

## 📁 Estructura del Proyecto

```
streamlit-pokedex/
├── app.py                    # Aplicación principal de Streamlit
├── pokemon.csv              # Dataset con información de Pokémon
├── preparar_datos.ipynb     # Notebook para procesar y limpiar datos
└── README.md               # Este archivo
```

## 🛠️ Requisitos

- Python 3.8+
- pandas
- streamlit
- plotly

## 📦 Instalación

1. Clona el repositorio o descarga los archivos
2. Instala las dependencias:

```bash
pip install pandas streamlit plotly
o
pip install -r requirements.txt
```

## 🚀 Cómo Ejecutar

Desde el directorio del proyecto, ejecuta:

```bash
streamlit run app.py
```

Luego accede a la aplicación en tu navegador (típicamente en `http://localhost:8501`)

## 📊 Datos

El dataset `pokemon.csv` contiene información de los primeros Pokémon incluyendo:
- **ID**: Número de identificación
- **Nombre**: Nombre del Pokémon
- **Tipos**: Tipo primario y secundario
- **Stats**: HP, Ataque, Defensa, Ataque Especial, Defensa Especial, Velocidad
- **Total de Stats**: Suma de todos los stats
- **Sprite**: URL de la imagen del Pokémon
- **Altura y Peso**: Medidas físicas
- **Legendario**: Indicador de si es Pokémon legendario

Los datos fueron procesados a partir de la **PokéAPI**.

## 🎯 Funcionalidades Detalladas

### Pestaña "Inicio"
Página de bienvenida con información general de la Pokédex

### Pestaña "Pokedex"
- Galería completa de Pokémon
- Controla cuántas cartas mostrar por fila (3-8)
- Selecciona cuántas Pokémon visualizar (hasta 48 o todas)
- Aplica todos los filtros de la barra lateral

### Pestaña "Ficha"
- Selecciona un Pokémon específico
- Visualiza su imagen (sprite)
- Muestra detalles: ID, nombre, tipo, altura, peso y stats totales
- Gráfico radar interactivo con todos los stats

### Pestaña "Comparador"
- Elige dos Pokémon para comparar
- Gráfico radar superpuesto mostrando los stats de ambos
- Indicador automático del ganador por total de stats

## 🎨 Paleta de Colores

Los Pokémon se colorean según su tipo primario:
- 🔥 Fuego: #EE8130
- 💧 Agua: #6390F0
- ⚡ Eléctrico: #F7D02C
- 🌿 Planta: #7AC74C
- Y muchos más...

## 📝 Notas Técnicas

- **Caching**: La función `cargar()` usa `@st.cache_data` para optimizar la carga del CSV
- **Responsive Design**: La aplicación se adapta a diferentes tamaños de pantalla
- **HTML personalizado**: Usa `unsafe_allow_html=True` para elementos HTML/CSS personalizados

## 🎓 Contexto Educativo

Este proyecto es parte del **Bootcamp 202605** y fue desarrollado como ejercicio de:
- Manipulación de datos con Pandas
- Creación de aplicaciones web interactivas con Streamlit
- Visualización de datos con Plotly
- Gestión de datasets CSV

## 📚 Recursos

- [Documentación de Streamlit](https://docs.streamlit.io/)
- [Plotly Graph Objects](https://plotly.com/python/graph-objects/)
- [PokéAPI](https://pokeapi.co/)
- [Pandas Documentation](https://pandas.pydata.org/docs/)

## 👤 Autor

Desarrollado como parte del bootcamp de programación

---

**¡Atrapa todo lo que puedas! 🎮**
