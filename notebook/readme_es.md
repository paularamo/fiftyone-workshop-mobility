# 🚦 Taller de FiftyOne: Edición Movilidad 
## Preparación Antes del Taller

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_eqFf8E4gC42y7oipX6BmNi_dJz-MfVv)

¡Bienvenido al **Taller de FiftyOne sobre Movilidad**!  
Para aprovechar al máximo la sesión, por favor sigue los pasos de preparación a continuación.


## Tareas Para Hacer **Un Día Antes** del Taller

### 1. Crea una Cuenta en Hugging Face (**Obligatorio**)
- Regístrate en [huggingface.co](https://huggingface.co/join)
- Ve a [Access Tokens](https://huggingface.co/settings/tokens) y crea un **token de lectura**


### 2. Lecturas Opcionales pero Altamente Recomendadas (📖)
Estos recursos te darán una ventaja y harán que el taller sea más fluido:

- [Cargar datasets desde Hugging Face](https://docs.voxel51.com/integrations/huggingface.html#loading-datasets-from-the-hub)
- [Vistas de Datasets (Filtrado, Corte, Búsqueda)](https://docs.voxel51.com/user_guide/using_views.html)
- [Clustering con Embeddings](https://docs.voxel51.com/tutorials/clustering.html?highlight=embedding)
- [Integración con MosaicML (Embeddings)](https://docs.voxel51.com/integrations/mosaic.html?highlight=embedding)
- [API de Plugins de FiftyOne](https://docs.voxel51.com/api/fiftyone.plugins.html?highlight=plugin#module-fiftyone.plugins)



### 3. Concepto Extra para Explorar: **Embeddings**
Lo exploraremos a fondo durante la sesión, pero si tienes curiosidad:
- [Artículo de CLIP por OpenAI](https://arxiv.org/abs/2103.00020)



## ⏰ Tarea Para Hacer **20 Minutos Antes** del Taller (**Obligatorio**)

> Esto depende de tu velocidad de internet. Puede tardar **10–25 minutos**. Por favor ejecuta lo siguiente **al menos 20 minutos antes del taller** en Google Colab.

Solo ejecuta la siguiente celda en tu notebook de Google Colab:

```python
# ESTE ES EL REQUISITO MÍNIMO DESPUÉS DE INSTALAR TODAS LAS DEPENDENCIAS.
import os
import fiftyone.utils.huggingface as fouh
from huggingface_hub import login

login(token="AGREGA_TU_TOKEN_DE_HF_AQUÍ") 
dataset = fouh.load_from_hub("dgural/bdd100k", persistent=True, name="bdd100k_test")
````

Asegúrate de **reemplazar** `"AGREGA_TU_TOKEN_DE_HF_AQUÍ"` con tu token de Hugging Face.

## 🏆 SUPER BONUS: ¡Conviértete en Contribuidor de Código Abierto!

Si **encuentras un error en la documentación** antes del taller, ganarás una **insignia premium de honor** 😎

* ¡Intenta corregirlo tú mismo y haz un PR!
* ¿No puedes arreglarlo aún? **¡No te preocupes!** Cuéntamelo durante el taller y te guiaré en tu **primera contribución a código abierto.**

Bienvenido al club cool de contribuidores 🚀
