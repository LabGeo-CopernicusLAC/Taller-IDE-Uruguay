<p align="center">
<img src="https://www.copernicuslac-chile.eu/wp-content/uploads/2024/05/logo_copernicuslac_chile.svg" alt="Copernicus LAC Chile" width="1600"/>
</p>

 
# Taller CopernicusLAC Chile - IDE Uruguay: Exploración aplicada de Atlas Urbano, Cobertura y Uso de Suelo y datos *in situ* para la generación e interpretación de evidencia territorial

Taller dictado por el Servicio de Atlas Urbano y el Servicio de Cobertura y uso de suelos de CopernicusLAC Chile coordinad en conjunto con la IDE Uruguay.
## ¿Cuándo se dicta?

| Sesión | Fecha | Horario |
|---|---|---|
| 1 · Virtual (Zoom) | 6 octubre 2026 | 10:00 – 12:00 |
| 2 · Presencial (IDE-Uruguay) | 8 octubre 2026 | 09:00 – 13:00 |

## Prerrequisitos

Se requierede `Git` y `Jupyter Notebook` para poder realizar este taller. Se recomienda que se instale la última distribución de [Anaconda](https://www.anaconda.com/docs/main) o de [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (más ligero) en su sistema operativo. Las distribuciones de Anaconda y Miniconda incluyen Jupyter Notebook.

## Instalación desde GitHub
La manera más simple para instalar los paquetes es via `Git`. Los usuarios pueden clonar este repositorio ejecutando los siguientes comandos desde su `terminal` (Linux/OSx) o desde el `Anaconda prompt`.

Si no tienes tienes `Git` instalado o no sabes si esta instalado, recomendamos asegurarte que `conda` está actualizado mediante el siguiente código:

```bash
conda update -n base conda
conda update --all
```
Ahora podemos asegurarnos de tener `Git` ejecutando la siguiente línea:

```bash
conda install git
```

En general el terminal se encuentra en el menú de inicio de la mayoría de las distribuciones de Linux y en la carpeta de Aplicaciones/Utilidades en OS X. Como alternativa, se debería poder abrir el terminal de Anaconda desde el menú de inicio (o desde el dock, o ejecutando el Anaconda Navigator). 

Una vez abierto el terminal, se debe navegar hacia la carpeta donde deseas colocar el taller  

```bash
cd /ruta/a/carpeta/taller_copernicus_lac
```

Una vez en la carpeta correcta, ejecutar el siguiente comando:

<!-- Una vez abierto el terminal, ejecutar el siguiente comando: -->
```bash
git clone --recurse-submodules --remote-submodules https://github.com/LabGeo-CopernicusLAC/Taller-IDE-Uruguay.git
```

Esto creará una copia local de todos los archivos relevantes, incluyendo los Jupyter Notebooks a ejecutar, códigos auxiliares y datos.

## Jupyter-Lab

Este taller es compatible con Python 3.11. Frente a las multiples opciones posibles, se recomienda que los usuarios instalen el paquete de Anaconda adecuado para su sistema operativo.
Para asegurarse que se cuente con todas las dependencias requeridas para la ejecución del taller, se recomienda que se configure el entorno de Python adecuado, como se explica a continuación.

### Entorno de Python

Python permite a los usuarios crear entornos específicos que se adapten a sus proyectos.
Los tutoriales incluidos en este taller requieren de varios paquetes que no vienen incluidos por defecto en Anaconda. En este directorio, los usuarios encontrarán un archivo *environment.yaml* que se puede utilizar para configurar un entorno con todos los paquetes necesarios ya instalados.

Para crear el entorno, debes abrir **Anaconda Prompt** (Windows) o el **terminal** (Linux/OS X) y navegar hasta la carpeta del repositorio que descargaste en la sección «Instalación» anterior. 

En esta carpeta hay un archivo llamado `environment.yml`, el cual contiene toda la información para instalar los paquetes a utilizar. Nuevamente en la carpeta correcta, ejecutar el siguiente comando:

```bash
cd Taller-IDE-Uruguay
conda env create -f environment.yml
```

Esto crea un entorno de Python llamado **2026Coplac**. El entorno no se activa por defecto, por lo que para activarlo ejecutamos:

```bash
conda activate 2026Coplac
```
<!--
Como último paso antes de iniciar JupyterLab, vamos a registrar el entorno como *kernel* en Jupyter, ejecutando:

```bash 
python -m ipykernel install --user --name 2026Coplac --display-name "Python (2026Coplac)"
```
 -->
```bash
# Windows
setup_kernel.bat
# OS X / Linux
bash setup_kernel.sh
```

Ahora sí, estamos listos para iniciar JupyterLab y realizar el taller!!

*Nota: Recordar que es necesario activar el entorno en cada sesión nueva*

### Jupyter Lab

Este Taller se basa en una serie de cuadernos de Jupyter ([Jupyter Notebooks](https://jupyter.org)), diseñados para ejecutarse en Jupyter Lab.
Los cuadernos de Jupyter facilitan el aprendizaje interactivo al permitirnos combinar código, descripciones de texto y visualizaciones de datos.

Para ejecutar Jupyter Notebook, abre un terminal o el símbolo del sistema de Anaconda y asegúrate de haber activado el entorno correcto. Una vez más, navega hasta la carpeta del repositorio. Ahora puedes ejecutar Jupyter utilizando:
`jupyter lab` o `jupyter-lab`, dependiendo de tu sistema operativo.

*Nota: Es importante ejecutar Jupyter Lab desde el directorio correcto. Jupyter Lab no puede encontrar nada que esté “por encima” de él en un árbol de directorios.

¡Ahora ya puedes ejecutar los cuadernos!

<!-- ## Dependencias
Item | Version | licencia | link info
## Estructura repositorio
El repositorio del taller cuenta con las siguientes carpetas
```
Taller_IDE_CopernicusLAC-Chile/
├── notebooks/
│   ├── 00_test_entorno.ipynb
│   ├── 01_preparacion_datos.ipynb
│   └── 02_taller_indices_valparaiso.ipynb
│
├── scripts/
│   ├── crear_areas_estudio.py
│   ├── descargar_capas_subpesca.py
│
├── tests/
│   ├── verificar_sintaxis.py
│   ├── test_nucleo_indices.py
│   └── verificar_salidas.py
│
├── data/
│   ├── sst/
│   ├── chl/
│   └── shapes/
│       ├── areas_estudio/
│       └── subpesca/
│
├── outputs/
│   ├── figures/  
│   └── tables/
│
├── images/
│
├── environment.yml
├── setup_kernel.bat
├── setup_kernel.sh
└── Guia_Descargas_Oceanos.md
```
 -->
## Contacto

Cualquier duda puedes escribirnos al soporte técnico  — [tallerIDEUruguay2026@copernicuslac-chile.eu](mailto:tallerIDEUruguay2026@copernicuslac-chile.eu)
