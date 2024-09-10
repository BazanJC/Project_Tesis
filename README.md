# Deteccion y Clasificacion de Particulas Cargadas en el Detector Cherenkov usando Machine Learning
Este proyecto implementa un sistema para el análisis espectral de partículas de alta energía utilizando el detector Cherenkov. El sistema incluye el uso de Machine Learning para la clasificación de partículas, un pipeline automatizado para el procesamiento de datos, y una interfaz gráfica construida con PySide6.
## Estructura del proyecto

```plaintext
/TesisMLCherenkov/
│
├── /docs/                        # Documentación del proyecto (puede ser generado por Sphinx)
│   ├── index.md                  # Índice de documentación
│   └── pipeline_diagram.png       # Diagramas de pipelines, esquemas del detector, etc.
│
├── /data/                        # Datos crudos y procesados
│   ├── /raw/                     # Datos originales
│   ├── /processed/               # Datos después del preprocesamiento
│   └── data_description.md       # Descripción de los conjuntos de datos
│
├── /notebooks/                   # notebooks de Jupyter de análisis de datos, 
                                        el entrenamiento de los modelos y otras tareas.
│   ├── entrenamiento_modelo.ipynb          # Pruebas del pipeline
│   ├── exploracion_datos.ipynb             # Pruebas del pipeline
│
├── /src/                         # Código fuente del proyecto
│   ├── /ml_pipeline/             # Módulos del pipeline de Machine Learning
│   │   ├── __init__.py
│   │   ├── data_preprocessing.py # Preprocesamiento y transformación de datos
│   │   ├── model_training.py     # Entrenamiento del modelo
│   │   └── evaluation.py         # Evaluación del modelo
│   │
│   ├── /cherenkov_analysis/      # Módulos específicos para el análisis espectral del detector Cherenkov
│   │   ├── spectral_analysis.py  # Análisis espectral
│   │   └── particle_classification.py # Clasificación de partículas
│   │
│   ├── /gui/                     # Interfaz gráfica (PySide6)
│   │   ├── main_window.py        # Ventana principal de la GUI
│   │   └── widgets.py            # Componentes reutilizables
│   │
│   └── run_pipeline.py           # Script para ejecutar todo el pipeline
│
├── /tests/                       # Pruebas automatizadas
│   ├── test_pipeline.py          # Pruebas del pipeline
│   ├── test_gui.py               # Pruebas de la interfaz gráfica
│   └── test_spectral_analysis.py # Pruebas del análisis espectral
│
├── /assets/                      # Recursos estáticos como imágenes o diagramas
│
├── .gitignore                    # Archivos a ignorar por Git
├── requirements.txt              # Dependencias del proyecto (incluye PySide6, sklearn, etc.)
├── README.md                     # Descripción general del proyecto
└── setup.py                      # Archivo de configuración para la instalación del paquete (si es necesario)
```