# Practica-4.--Extension-de-Software-para-Convertir-Expresiones-Regulares

---

## 👥 Autores

- **Gustavo Sebastián Bonilla Ojeda** — 2025630175  
- **Ximena Velázquez Mendoza** — 2024630176  
- **Yoltic Isaí Velázquez Ramos** — 2025230228  

📍 *ESCOM - Instituto Politécnico Nacional*  
📅 *Fecha: 30 de abril de 2026*  

---

## 🚀 Características

### 🔹 Conversión de AFD a Expresión Regular (GNFA)

El sistema implementa el **algoritmo de eliminación de estados**, que transforma un **AFD** en una **Expresión Regular equivalente**.

✔ Convierte automáticamente autómatas deterministas en ER  
✔ Usa estados `START` y `END` auxiliares  
✔ Muestra paso a paso la eliminación de estados  
✔ Genera la expresión regular final

Ejemplo de salida:

```text
━━━ Algoritmo de Eliminación de Estados ━━━

[*] Eliminando estado q0...
    -> Estado actualizado.

[*] Eliminando estado q1...
    -> Estado actualizado.

Expresión Regular: (a+b)*abb
````

---

### 🔹 Validación de Casos Prácticos con Expresiones Regulares

Permite validar cadenas reales usando ER predefinidas:

#### 📧 Correo electrónico

```regex
^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$
```

#### 📱 Número telefónico (10 dígitos)

```regex
^\d{10}$
```

#### 📅 Fecha (dd/mm/yyyy)

```regex
^(0[1-9]|[12][0-9]|3[01])/(0[1-9]|1[012])/\d{4}$
```

✔ Retroalimentación visual:

* ✅ Válido
* ❌ Inválido

---

### 🔹 Visualización de AFD de Casos Reales

El sistema genera automáticamente autómatas para:

* 📱 Teléfono de 10 dígitos
* 📧 Correo electrónico
* 📅 Fecha válida

Usa:

* `matplotlib`
* `networkx`

Para mostrar el diagrama de estados del AFD.

---

## 🛠 Tecnologías usadas

* Python 3
* Tkinter
* re (Regex)
* Matplotlib
* NetworkX

---
