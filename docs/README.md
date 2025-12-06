**Analisis de Sequia y Precipitacion en el Limari Precordillerano**

Autor: Ignacio Pizarro
Contacto: ignacio.pizarro@uc.cl 

**Sobre el Proyecto:**

Este proyecto analiza el comportamiento historico de las precipitaciones y la severidad de las sequias en el Limari precordillerano, compuesto por las comunas de Combarbala y Monte Patria (Region de Coquimbo, Chile), una zona caracterizada por la transhumancia y la sensibilidad al fenómeno ENOS (El Niño Oscilación Sur).Para analizar este fenomeno, se ha optado por utilizar datos de las estaciones meteorológicas Las Ramadas (Monte Patria) y Cogoti (Combarbala), realizando boxplots de precipitación mensual y series de tiempo para calcular el Indice Estandarizado de Precipitacion y Evapotranspiracion (SPEI) para identificar tendencias de sequia durante el periodo 1970 - 2015. Los datos crudos han sido extraidos de la plataforma Explorador Climatico (https://explorador.cr2.cl) desarrollado por el Centro de Ciencia del Clima y la Resiliencia (CR2), la cual tiene disponible datos historicos de precipitacion, temperatura y otras variables.

**Estructura del Proyecto:**

El proyecto esta organizado de la siguiente manera:

```bash
Precipitacion_y_sequia_Combarbala/
├── _quarto.yml          # Configuracion del sitio web
├── index.qmd            # Pagina de inicio y analisis de datos
├── spei.qmd             # Codigo R y Graficos
├── styles.css           # Estilos personalizado
├── README.md            # Informacian general del proyecto
├── data/
│   ├── data_raw/        # Archivos CSV crudos por estacion
│   └── data_procesada/  # Datos limpios y unificados
├── docs/                # Carpeta de salida (Sitio Web generado)
└── figuras/             # Graficos exportados en PNG
```

**Herramienta de analisis y Paquetes**

El trabajo completo fue realizado en RStudio utilizando los siguientes paquetes:

pacman: Gestor de paquetes para hacer eficiente la instalacion.
tidyverse: Manipulacion, visualizacion y limpieza de datos.
SPEI: Calculo de índices de sequia y evapotranspiracion (metodo Hargreaves).
lubridate: Manejo de fechas.
here y fs: Gestion de rutas de archivos.
Quarto: Generacion del sitio web.

**Declaración de uso de Inteligencia Artificial**

El autor declara haber utilizado Inteligencia Artificial, especificamente Google Gemini, para resolver dudas y generar una estructura mas eficiente del código. Para asegurar el correcto uso de la herramienta, se reviso el código y los datasets, ademas de comparar los resultados con otros estudios que utilizan SPEI, como los de Meza (2013) y del Núcleo Milenio AndesPeat.

**Agradecimientos**

El autor agradece al Centro de Ciencia del Clima y la Resiliencia (CR2) por los datos entregados. Tambien a los crianceros de Combarbala por la entrega de sus relatos para el proyecto de tesis "Mas alla de la Cordillera: Cambio climatico y Transhumancia en Combarbala". Sus historias nutren la curiosidad y urgencia de pensar la crisis climatica en un territorio tan fragil como el Limari.
