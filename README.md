# ATL Project — Model Transformation: Dictionary to Thematic Dictionaries

## Objective

This project aims to transform a **model representing a general dictionary** into **four thematic dictionaries** using **ATL (Atlas Transformation Language)** within the **Eclipse** environment.

---

## Project Steps

### 1. Define and Implement Source and Target Metamodels

- **Source Metamodel**: Represents a dictionary composed of multiple entries.
- **Target Metamodel**: Represents four separate thematic dictionaries each containing the relevant entries.

> Metamodels are defined using Ecore via the **Eclipse Modeling Framework (EMF)**.

---

### 2. Create a Source Model Compliant with the Source Metamodel

- Creation of a model `Dictionnaire.xmi` containing various entries with different themes.
- Tool used: **Sample Ecore Model Editor** or a custom-built editor.

---

### 3. Write ATL Transformation Rules

- ATL rules map elements from the source model to the appropriate elements in the target models.
- Each entry is redirected to the thematic dictionary matching its theme.


### 4. Implement the MMS2MMC Transformation in ATL Using Eclipse
- ATL module: Dict2Dict.atl

- Configuration of the model-to-model (M2M) transformation using Eclipse.

- Use ATL Launch Configuration to run the transformation.

### 5. Project Structure

DictionaryATL/
│
├── metamodels/
│   ├── dictionnaire.ecore
│   └── dictionnaireCible.ecore
│
├── models/
│   ├── Dictionnaire.xmi
│   └── Dict_resultats.xmi
│
├── Dict2Dict.atl
│ 
├── Dict2Dict.asm
│
└── README.md

### 6. Expected Results
A source dictionary model successfully transformed into four thematic dictionary models.

Correct thematic classification of entries based on the defined transformation rules.

A fully operational ATL project within Eclipse.

### 7. echnologies Used
Eclipse IDE (with ATL plugin)

EMF (Eclipse Modeling Framework)

ATL (Atlas Transformation Language)

XMI / Ecore

