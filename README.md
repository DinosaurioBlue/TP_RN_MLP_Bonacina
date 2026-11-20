# TP RN MLP Bonacina

Incluye la consigna y estructura del MLP. La comparación con Softmax forma parte de este TP: se conservan sus registros y los resultados de ambas familias dentro del experimento MLP_20Newsgroups. Hay corridas terminadas, podadas e interrumpidas; no se presentan todas como resultados finales.

## Archivos y ejecución

- Notebook principal: `MLP_TP.ipynb`.
- Dependencias con versiones: `requirements.txt`. Versiones observadas: `entorno-origen.json`.
- Ejecutar `python -m pip install -r requirements.txt` y abrir el notebook con ese entorno en Jupyter o VS Code, usando esta carpeta como directorio de trabajo.
- La primera ejecución descarga 20 Newsgroups y recursos de NLTK y requiere conexión a Internet.
- Separar los archivos no volvió a ejecutar entrenamientos ni verificó una instalación limpia. Los resultados guardados se pueden leer sin entrenar.

## Registros de los experimentos

Registros de MLflow conservados: **548 corridas**. `mlflow.db` contiene únicamente el experimento de este TP. `registros/mlflow/` ofrece las tablas de corridas, parámetros, métricas por paso y últimas métricas en CSV. Los gráficos disponibles se conservan en `mlruns/` y los eventos de TensorBoard en `runs/`.

Para revisar MLflow ejecutar `python ver_registros.py` y abrir la dirección local que indique. Este comando actualiza las rutas de artefactos al directorio actual. Para TensorBoard ejecutar `tensorboard --logdir runs`.

Los modelos entrenados y su preprocesamiento se conservan localmente en `modelos/` cuando estaban disponibles y se excluyen de GitHub. No se entregan los pesos de modelos de MLflow. Las carpetas `runs/`, `mlruns/`, los CSV y la base `mlflow.db` sí se versionan, conforme a la indicación del profesor del 4 de noviembre.

## Procedencia

Separado el 20 de noviembre de 2026 desde https://github.com/DinosaurioBlue/RN_Bonacina_TPs, revisión `6f8566054ae62b94b7cb2c9a09620bc806a473d9`. Los notebooks y los archivos copiados se verificaron por SHA-256; se conservaron sin cambios. El repositorio original y los experimentos auxiliares permanecen en `01 - TP's` como respaldo. Los historiales anteriores continúan disponibles en el repositorio original.
