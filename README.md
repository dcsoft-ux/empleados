# 🧩 Proyecto Empleados

Aplicación web desarrollada con **Django** para la gestión de empleados dentro de una organización.  
Permite registrar, consultar, actualizar y eliminar información de empleados, incluyendo datos personales, cargo, área y fotografía.

---

## 🚀 Características principales

- 📋 CRUD completo de empleados (crear, leer, actualizar, eliminar)
- 📸 Carga y visualización de fotos de perfil
- 🧭 Interfaz con plantillas HTML y CSS personalizadas
- 🗃️ Base de datos relacional integrada (PostgreSQL o SQLite)
- ⚙️ Panel administrativo de Django
- 🔐 Configuración modular y adaptable para distintos entornos

---

## 🏗️ Estructura del proyecto

```bash
empleados/
├── applications/           # Aplicaciones internas del proyecto
├── empleado/               # App principal: modelos, vistas y URLs
├── media/                  # Archivos cargados (fotos de empleados)
├── static/                 # Archivos estáticos (CSS, JS, imágenes)
├── templates/              # Plantillas HTML
├── manage.py               # Script principal de Django
├── requirements.txt        # Dependencias del proyecto
└── README.md               # Este archivo
⚙️ Instalación y configuración local
1️⃣ Clonar el repositorio
bash
Copiar código
git clone https://github.com/dcsoft-ux/empleados.git
cd empleados
2️⃣ Crear entorno virtual
bash
Copiar código
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
3️⃣ Instalar dependencias
bash
Copiar código
pip install -r requirements.txt
4️⃣ Configurar la base de datos
Edita el archivo settings.py para usar tu motor de base de datos (por defecto SQLite).

Ejemplo con PostgreSQL:

python
Copiar código
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'empleados_db',
        'USER': 'postgres',
        'PASSWORD': 'tu_password',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}
5️⃣ Ejecutar migraciones y levantar el servidor
bash
Copiar código
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
Accede a la aplicación en 👉 http://127.0.0.1:8000

🧠 Tecnologías utilizadas
Componente	Descripción
Python 3.12+	Lenguaje base del proyecto
Django 5.x	Framework web principal
HTML / CSS / JS	Interfaz de usuario
Bootstrap / Tailwind (opcional)	Estilo visual
PostgreSQL / SQLite	Base de datos
GitHub Actions	Automatización y CI/CD

🧩 Próximas mejoras
 Autenticación de usuarios y roles

 API REST con Django REST Framework

 Exportar reportes en PDF / Excel

 Interfaz más moderna con Vue o React

 Dockerización del proyecto

👨‍💻 Autor
Carlos Andrés Daza Parra
Desarrollador web, docente e investigador.

🌐 LinkedIn

💻 GitHub

📧 contacto: cdazaparra@gmail.com

📄 Licencia
Este proyecto está bajo la licencia MIT — libre para uso, modificación y distribución, siempre que se mantenga la atribución al autor original.
