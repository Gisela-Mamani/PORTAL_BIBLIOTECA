# Portal de Biblioteca



## Estructura del proyecto

```
portal_biblioteca/
├── venv/
├── app.py
├── requirements.txt
├── .gitignore
├── templates/
│   ├── base.html
│   ├── index.html
│   ├── login.html
│   ├── libros.html
│   └── perfil.html
├── static/
│   └── style.css
└── README.md
```

## Usuarios de prueba

| Usuario | Contraseña |
|---------|------------|
| carlos  | 1111       |
| laura   | 2222       |
| diego   | 3333       |

## Instrucciones para ejecutar el proyecto

### 1. Crear y activar el entorno virtual

```bash
# Crear el entorno virtual
python -m venv venv

# Activar el entorno virtual
# En Windows:
venv\Scripts\activate
# En macOS / Linux:
source venv/bin/activate
```

### 2. Instalar Flask dentro del entorno virtual

```bash
pip install -r requirements.txt
# o bien:
pip install Flask
```

### 3. Ejecutar la aplicación

```bash
python app.py
```

La aplicación quedará disponible en `http://127.0.0.1:5000/`.

## Control de versiones (Git y GitHub)

Pasos sugeridos para cumplir con los commits mínimos requeridos:

```bash
git init
git add app.py templates static requirements.txt .gitignore README.md
git commit -m "Proyecto inicial"

# luego de implementar el formulario de acceso:
git add .
git commit -m "Implementa formulario de acceso"

# luego de implementar sesiones y protección de rutas:
git add .
git commit -m "Implementa sesiones y protección de rutas"

# luego de implementar Jinja2 y cookies:
git add .
git commit -m "Implementa Jinja y cookies"

# Subir a GitHub:
git remote add origin <URL_DEL_REPOSITORIO>
git branch -M main
git push -u origin main
```
