import pandas as pd
import numpy as np 

# Semilla para reproducibilidad
np.random.seed(42)

# Cantidad de registros
n = 500

# Generar variables
edad = np.random.randint(17, 30, n).astype(float)
genero = np.random.choice(["Masculino", "Femenino", "Otro"], n, p=[0.45, 0.5, 0.05])
origen = np.random.choice(["Local", "Regional", "Nacional"], n, p=[0.4, 0.4, 0.2])
promedio_colegio = np.round(np.random.uniform(1.5, 5.0, n), 2)
puntaje_admision = np.round(np.random.uniform(40, 100, n), 1)
nota_primer_semestre = np.round(np.random.uniform(1.0, 5.0, n), 2)
nivel_socioeconomico = np.random.choice(["Bajo", "Medio", "Alto"], n, p=[0.4, 0.45, 0.15])
beca = np.random.choice(["Sí", "No"], n, p=[0.3, 0.7])
prestamo = np.random.choice(["Sí", "No"], n, p=[0.5, 0.5])
abandono = np.random.choice(["Sí", "No"], n, p=[0.25, 0.75])

# Crear DataFrame
df = pd.DataFrame({
    "edad": edad,
    "genero": genero,
    "origen": origen,
    "promedio_colegio": promedio_colegio,
    "puntaje_admision": puntaje_admision,
    "nota_primer_semestre": nota_primer_semestre,
    "nivel_socioeconomico": nivel_socioeconomico,
    "beca": beca,
    "prestamo": prestamo,
    "abandono": abandono
})

# Introducir valores nulos (~5%)
for col in df.columns:
    df.loc[df.sample(frac=0.05).index, col] = np.nan

# Introducir valores atípicos
outlier_indices = np.random.choice(df.index, size=5, replace=False)
df.loc[outlier_indices, "edad"] = [50, 45, 16, 60, 15]
df.loc[outlier_indices, "nota_primer_semestre"] = [0.2, 5.5, 0.5, 6.0, 1.0]

# Guardar CSV
df.to_csv("dataset_abandono_estudiantil.csv", index=False)

print("✅ Dataset generado correctamente: dataset_abandono_estudiantil.csv")
