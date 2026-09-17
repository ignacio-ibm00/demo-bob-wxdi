# Watsonx Data Intelligence MCP Tools — Demo Guide

---

## 1. View Available Projects

```
"Mostrame los proyectos disponibles dentro de Watsonx Data Intelligence"
```

**Expected Result:** Project `Bob` is active and ready.

---

## 2. View Imported Assets

```
"Mostrame los assets importados en el proyecto"
```

**Expected Result:** Metadata import `Import_Bob` has completed successfully.

---

## 3. Explore Data Lineage

```
"Busca y mostrame el linaje de este proyecto"
```

**Expected Result:** Available assets with lineage information for DB2 connection.

---

## 4. Create Data Quality Rule

```
"Crea una regla de calidad en el proyecto Bob para la tabla VM_Health que valide que la columna VM_name no tenga valores nulos"
```

**Expected Result:** Quality rule generated and executed with results.

---

## 4.1. View Quality Rule Results

```
"Muéstrame el resultado de la ejecución de la regla de calidad que acabamos de crear"
```

**Expected Result:** Detailed execution results of the quality rule.

---

## 5. Create View on VM_HEALTH *(Optional)*

```
"Quiero hacer una nueva vista en el proyecto. Partiendo de VM_HEALTH quiero filtrar y quedarme solo con los registros que tengan HEALTH_SCORE = 20 y que se llame VM_HEALTH_20"
```

**Expected Result:** Filtered view created in project.

---

## 6. Publish Asset to Catalog

```
"Publica el asset VM_Health del proyecto al catálogo Bob"
```

**Expected Result:** Asset published with catalog link.

---

## 7. Create Data Product

```
"Crea un data product con el asset VM_Health que acabamos de publicar en el catálogo"
```

**Expected Result:** Draft data product created in Data Product Hub.

---

## 8. Publish Data Product

```
"Agrégale el dominio Information Technology y publícalo"
```

**Expected Result:** Data product published with domain assignment and final link.

---

## 9. View Data Contract

```
"Muéstrame el data contract del data product que acabamos de crear"
```

**Expected Result:** Published data product contract details.

---

## 10. Impact Analysis

```
"¿Qué pasa si elimino la columna VM_NAME de la DB2? No lo hagas, solo quiero que hagas el análisis."
```

**Expected Result:** Impact analysis showing affected dependencies.

---

## 11. View Published Data Products

```
"Muéstrame los data products publicados"
```

**Expected Result:** List of all published data products in the system.

---

## 12. Consume Data Product

```
"VM Service Health BOB - Quiero consumir este data product"
```

**Expected Result:** Data product consumption request initiated successfully.

---

**Note:** Execute each command individually and wait for completion before proceeding to the next step.


