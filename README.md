# 🚗 Simulación del Sistema de Pago de Parqueadero - Centro Comercial Supercentro

## 📌 Descripción

Este proyecto implementa un modelo de **Simulación de Eventos Discretos** utilizando Python y la librería SimPy para analizar el desempeño del sistema de pago de parqueaderos del Centro Comercial Supercentro.

El objetivo es determinar si la infraestructura actual de **tres cajeros independientes** es suficiente para atender la demanda de usuarios y mantener tiempos de espera aceptables.

---

## 🎯 Objetivos

* Analizar el comportamiento de los diferentes tipos de usuarios.
* Determinar el cajero con menor y mayor tiempo promedio de atención.
* Evaluar los tiempos de espera generados en el sistema.
* Identificar el estado estable de la simulación.
* Aplicar procesos de verificación, calibración y validación.
* Proponer estrategias de mejora para optimizar la atención.

---

## ⚙️ Tecnologías Utilizadas

* Python 3
* SimPy
* Pandas
* NumPy
* Matplotlib
* SciPy

---

## 👥 Tipos de Usuarios

| Tipo de Usuario | Tiempo Medio de Servicio (min) | Probabilidad |
| --------------- | ------------------------------ | ------------ |
| Rápido          | 1                              | 25 %         |
| Normal          | 3                              | 20 %         |
| Lento           | 4                              | 27.5 %       |
| Muy Lento       | 6                              | 27.5 %       |

---

## 🔬 Metodología

El sistema fue modelado mediante simulación de eventos discretos considerando:

* Tres cajeros independientes.
* Disciplina FIFO (First In First Out).
* Tiempos de llegada y servicio con distribución exponencial.
* Selección aleatoria de cajero por parte del usuario.
* Eliminación del período transitorio mediante Warm-Up.

---

## 📊 Resultados Principales

* Tiempo promedio de atención por cajero cercano a 3.5 minutos.
* Distribución de usuarios consistente con las probabilidades definidas.
* Tiempo promedio de espera elevado, indicando saturación del sistema.
* Identificación del estado estable después del período de calentamiento.

---

## 💡 Conclusiones

Los resultados muestran que la capacidad actual de tres cajeros no es suficiente para atender la demanda del sistema bajo las condiciones simuladas.

Se recomienda:

* Implementar una fila única centralizada.
* Incrementar el número de cajeros.
* Evaluar esquemas de atención diferenciados para usuarios rápidos.

---

## ▶️ Ejecución

Instalar dependencias:

```bash
pip install simpy pandas numpy matplotlib scipy
```

Ejecutar el archivo principal:

```bash
python simulacion_parqueadero.py
```

---

## 📚 Autor

Jessica Serna Vargas

Proyecto académico – Simulación de Eventos Discretos.
