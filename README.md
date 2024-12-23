# Introducción

La diabetes es una de las enfermedades crónicas más prevalentes y de mayor impacto en la salud pública a nivel mundial. Según la Organización Mundial de la Salud (OMS), el número de personas con diabetes ha ido aumentando significativamente en las últimas décadas debido al envejecimiento de la población, los estilos de vida sedentarios y los malos hábitos alimenticios.

La diabetes puede clasificarse principalmente en dos tipos: diabetes tipo 1, una enfermedad autoinmune que destruye las células productoras de insulina; y diabetes tipo 2, relacionada con factores como la obesidad y el estilo de vida. Es por esto que lña detección temprana y la clasificación de individuos en riesgo es clave para diseñar intervenciones preventivas y reducir las complicaciones asociadas con la enfermedad.

En este contexto, los modelos de aprendizaje automático (Machine Learning) ofrecen herramientas potentes para la clasificación y predicción, permitiendo analizar grandes volúmenes de datos y detectar patrones complejos que no son evidentes a simple vista.

![image](https://github.com/user-attachments/assets/3ddeca09-1aea-49c2-89bf-b1856db33d86)

# Descripción del Problema

En este trabajo, se analizará un [dataset](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset/data) que contiene información de salud relacionada con factores de riesgo para la diabetes. Las variables incluyen datos como presión arterial alta, colesterol alto, índice de masa corporal (BMI), hábitos de estilo de vida (actividad física, consumo de frutas y verduras, tabaquismo), variables demográficas (edad, género, educación e ingresos) y condiciones preexistentes como enfermedades cardíacas o ataques.

# Objetivo

El objetivo principal de este estudio es desarrollar un clasificador basado en Machine Learning que permita predecir el riesgo de sufrir diabetes de un individuo utilizando las variables proporcionadas en el dataset, por tanto la variable objetivo será Diabetes_012.

# Descripción del Dataset

El dataset contiene los siguientes parámetros y cuenta con 253.680 datos.

## 1. Diabetes_012
**Clasificación del estado de diabetes:**
- `0`: No diabetes
- `1`: Prediabetes
- `2`: Diabetes

## 2. HighBP
**Presión arterial alta:**
- `0`: No high BP
- `1`: High BP

## 3. HighChol
**Colesterol alto:**
- `0`: No high cholesterol
- `1`: High cholesterol

## 4. CholCheck
**Revisión de colesterol en los últimos 5 años:**
- `0`: No check
- `1`: Sí, chequeo de colesterol en los últimos 5 años

## 5. BMI
**Índice de Masa Corporal (Body Mass Index).**

## 6. Smoker
**¿Ha fumado al menos 100 cigarrillos en su vida? (Nota: 5 paquetes = 100 cigarrillos):**
- `0`: No
- `1`: Sí

## 7. Stroke
**¿Le han diagnosticado un accidente cerebrovascular?:**
- `0`: No
- `1`: Sí

## 8. HeartDiseaseorAttack
**¿Le han diagnosticado enfermedad coronaria (CHD) o infarto de miocardio (MI)?:**
- `0`: No
- `1`: Sí

## 9. PhysActivity
**Actividad física en los últimos 30 días (no incluye trabajo):**
- `0`: No
- `1`: Sí

## 10. Fruits
**Consumo de frutas al menos 1 vez por día:**
- `0`: No
- `1`: Sí

## 11. Veggies
**Consumo de vegetales al menos 1 vez por día:**
- `0`: No
- `1`: Sí

## 12. HvyAlcoholConsump
**Consumo excesivo de alcohol:**
- `0`: No
- `1`: Sí  
*(Definición: Hombres >14 bebidas/semana, Mujeres >7 bebidas/semana)*

## 13. AnyHealthcare
**¿Tiene algún tipo de cobertura de salud, como seguro o planes prepagos?:**
- `0`: No
- `1`: Sí

## 14. NoDocbcCost
**¿No pudo ver al médico en los últimos 12 meses debido a costos?:**
- `0`: No
- `1`: Sí

## 15. GenHlth
**Calificación general de la salud:**
- `1`: Excelente
- `2`: Muy buena
- `3`: Buena
- `4`: Regular
- `5`: Mala

## 16. MentHlth
**Número de días en los últimos 30 días en que la salud mental no fue buena (estrés, depresión, emociones):**
- Escala: `1-30 días`

## 17. PhysHlth
**Número de días en los últimos 30 días en que la salud física no fue buena (enfermedades o lesiones):**
- Escala: `1-30 días`

## 18. DiffWalk
**¿Tiene serias dificultades para caminar o subir escaleras?:**
- `0`: No
- `1`: Sí

## 19. Sex
**Género:**
- `0`: Femenino
- `1`: Masculino

## 20. Age
**Categoría de edad (13 niveles):**
- `1`: 18-24 años
- `2`: 25-29 años
- `3`: 30-34 años
- `4`: 35-39 años
- `5`: 40-44 años
- `6`: 45-49 años
- `7`: 50-54 años
- `8`: 55-59 años
- `9`: 60-64 años
- `10`: 65-69 años
- `11`: 70-74 años
- `12`: 75-79 años
- `13`: 80 años o más

## 21. Education
**Nivel educativo:**
- `1`: Nunca asistió a la escuela o solo kinder
- `2`: Grados 1 a 8 (Primaria)
- `3`: Grados 9 a 11 (Secundaria incompleta)
- `4`: Grado 12 o GED (Secundaria completa)
- `5`: 1 a 3 años de universidad o escuela técnica
- `6`: Universidad completa (4 años o más)

## 22. Income
**Nivel de ingresos (8 niveles):**
- `1`: Menos de $10,000
- `2`: Entre $10,000 y menos de $15,000
- `3`: Entre $15,000 y menos de $20,000
- `4`: Entre $20,000 y menos de $25,000
- `5`: Entre $25,000 y menos de $35,000
- `6`: Entre $35,000 y menos de $50,000
- `7`: Entre $50,000 y menos de $75,000
- `8`: $75,000 o más


