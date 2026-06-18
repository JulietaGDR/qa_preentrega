# Automatización de Pruebas con Python
## Propósito del Proyecto

Este proyecto tiene como objetivo automatizar pruebas funcionales de una aplicación web utilizando herramientas de testing en Python.

Se busca validar el correcto funcionamiento de distintas funcionalidades mediante pruebas automatizadas, mejorando la calidad del software y reduciendo el esfuerzo manual.

---

## Tecnologías Utilizadas

- Python → Lenguaje principal de desarrollo  
- Pytest → Framework de testing  
- Selenium WebDriver → Automatización de navegadores  
- pytest-html → Generación de reportes en HTML  

---
## Requisitos Previos

- Python 3.10 o superior
- Google Chrome
- ChromeDriver compatible
- Git instalado
- Acceso a Internet

## Instalación de Dependencias

### 1. Clonar el repositorio
    git clone 

### 2. Crear entorno virtual (opcional pero recomendado)
    python -m venv env

### 3. Activar entorno virtual

En Windows:
    env\Scripts\activate

En Linux/Mac:
    source venv/bin/activate

### 4. Instalar dependencias
    pip install -r requirements.txt

---

### Pruebas de API

Se realizan con 'https://reqres.in/api'

El requirements.txt instalará la dependencia

2. Crear un archivo .env en la raíz del proyecto, donde escribirá su APIKEY y datos de Login
Ejemplo


X_API_KEY=su_key

EMAIL_USER=su_usuario@reqres.in

PASSWORD_USER=su_pass


3. LLamarlo desde su test usando __from dotenv import load_dotenv__

## Casos de Prueba Automatizados

El proyecto contempla pruebas automatizadas sobre:

- Login exitoso
- Login inválido
- Navegación de usuarios
- Validación de elementos en pantalla
- Validación de respuestas API
- Verificación de códigos HTTP

## Ejecución de Pruebas

Ejecutar las pruebas con:
    pytest -v

---

## Generación de Reportes

Generar reporte HTML con:
    pytest tests/test_saucedemo.py -v --html=reports/report.html

El archivo generado será:
    El reporte generado quedará en:

reports/report.html

Abrirlo en un navegador para ver el detalle de ejecución.

---

## Estructura del Proyecto

    project/

├── conftest.py

├── requirements.txt

├── README.md

├── .gitignore

│
├── tests/\

│   ├── test_saucedemo.py

│   └── commons/

│       ├── __init__.py

│       └── funciones_commons.py
│
├── utils/

├── data/

├── reports/

│   └── report.html

---

## Autora

Julieta García Da Rosa

Automatización de pruebas funcionales utilizando Python, Selenium y Pytest.