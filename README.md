# FlaskAPI - Gestión Académica 📊  
**Sistema de evaluación y análisis de datos académicos**  

API robusta para gestión de calificaciones, generación de reportes estadísticos y seguimiento del desempeño estudiantil, construida con Django REST Framework.

## 🌟 Características Principales

🔹 **Gestión de Calificaciones**: Registro y consulta de resultados académicos  
🔹 **Análisis Estadístico**: Cálculo de promedios, modas y percentiles  
🔹 **Dashboard Integrado**: Preparación de datos para visualización  
🔹 **Exportación de Datos**: Generación de reportes en PDF/Excel  
🔹 **API Segura**: Autenticación por roles (Estudiante/Profesor/Admin)  

## 🛠 Stack Tecnológico  

| Componente       | Tecnologías/Librerías                |
|------------------|--------------------------------------|
| Backend          | Python 3.10+, Django 4.1+, DRF 3.13 |
| Base de Datos    | PostgreSQL 13                        |
| Autenticación    | JWT (djangorestframework-simplejwt)  |
| Documentación    | drf-spectacular                      |
| Análisis Datos   | Pandas, NumPy                        |
| Reportes         | ReportLab, openpyxl                  |

## 🚀 Instalación Rápida

```bash
git clone https://github.com/matias-bello-rodriguez/api_evaluacion2.git
cd api_evaluacion2
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate    # Windows
pip install -r requirements.txt
```

##⚙ Configuración
1. **Crear archivo .env**
```bash
SECRET_KEY=tu_clave_secreta_django
DB_NAME=evaluacion_db
DB_USER=usuario
DB_PASSWORD=contraseña
DEBUG=True
```
2. **Migraciones inciales**
```bash
python manage.py migrate
```
3. **Cargar datos iniciales**
```bash
python manage.py loaddata fixtures/datos_iniciales.json
```

##🏃 Ejecución

**Server de desarrollo**
```bash
python manage.py runserver
```

**Documentación**
```bash
[python manage.py runserver
](http://localhost:8000/api/schema/swagger-ui/
)```

