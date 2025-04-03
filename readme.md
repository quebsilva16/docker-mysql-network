# 🐳 MySQL Docker para Desarrollo

**Contenedor MySQL 8 configurable** para entornos de desarrollo, diseñado para compartir una misma instancia entre múltiples proyectos con bases de datos independientes.

## 🌟 Características Clave
- ✅ **MySQL 8.0** listo para desarrollo
- ✅ **Sin bases de datos predefinidas** (totalmente flexible)
- ✅ **Solo usuario root** al inicio (agrega usuarios manualmente)
- ✅ **Persistencia de datos** mediante volúmenes Docker
- ✅ **Red compartida** para conectar múltiples proyectos

## 🚀 Primeros Pasos

### 📋 Prerrequisitos
- Docker Engine ≥ 20.10
- Docker Compose ≥ 2.0

### 🔧 Configuración Inicial
1. **Clona este repositorio**:
   ```bash
   git clone [tu-repo-url] && cd MySQL

### 2. Crear red Docker (requerido solo una vez)
    ```bash
    docker network create mysql_shared_network

### Verifica que se creó correctamente:
    ```bash
    docker network ls | grep mysql_shared_network