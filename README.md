# Validador Pp - Partida Específica

Aplicación web para validar combinaciones de **Programa Presupuestario (Pp)** y **Partida Específica** según el catálogo oficial de SADER.

## 🚀 Demo

Accede a la aplicación en: [tu-app.streamlit.app](https://tu-app.streamlit.app)

## ✨ Funcionalidades

### 🔍 Consulta Individual
- Valida una combinación Pp + Partida específica
- Muestra todas las partidas válidas para un Pp
- Agrupa resultados por capítulo de gasto

### 📋 Validación Masiva
- Procesa archivos Excel con múltiples registros
- Soporta formato PIPP oficial
- Soporta archivos con columnas nombradas (Pp/Programa, Partida/Objeto)
- Genera reporte Excel descargable con resultados coloreados

### 📖 Explorador de Catálogo
- Navega el catálogo completo por Pp
- Visualiza partidas agrupadas por capítulo

## 📁 Archivos requeridos

### Catálogo base
El archivo `Pp_-_Partida_Especifica_2026.xlsx` con el catálogo oficial.

Estructura esperada (sin encabezados):
- Columna C (índice 2): Modalidad
- Columna E (índice 4): Programa (3 dígitos)
- Columna G (índice 6): Partida específica (5 dígitos)

### Archivos a validar

**Formato PIPP:**
- Columna J (índice 9): Pp
- Columna K (índice 10): Partida

**Formato con columnas:**
- Columna con "PP" o "PROGRAMA" en el nombre
- Columna con "PARTIDA" u "OBJETO" en el nombre

## 🛠️ Instalación local

```bash
# Clonar repositorio
git clone https://github.com/tu-usuario/validador-pp-partida.git
cd validador-pp-partida

# Instalar dependencias
pip install -r requirements.txt

# Ejecutar
streamlit run app.py
```

## 📦 Despliegue en Streamlit Cloud

1. Sube este repositorio a GitHub
2. Ve a [share.streamlit.io](https://share.streamlit.io)
3. Conecta tu cuenta de GitHub
4. Selecciona el repositorio y archivo `app.py`
5. Click en **Deploy**

## 🎨 Colores institucionales

- Guinda SADER: `#6B1D3D`
- Crema: `#F5F0E6`
- Verde válido: `#2E7D32`
- Rojo error: `#C62828`

## 📄 Licencia

Uso interno SADER.

---

Desarrollado para la Secretaría de Agricultura y Desarrollo Rural (SADER)
