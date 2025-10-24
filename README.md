# 🔐 CentralAuth

> 🚧 **En desarrollo:** esta aplicación aún no ha sido implementada.  
> El sistema se encuentra en fase de definición y diseño de requisitos.

**CentralAuth** es un **Sistema de Autenticación Centralizado (IdP/SSO)** desarrollado para la universidad U-Tad.  
Su objetivo es proporcionar un punto único de autenticación y gestión de identidades para todas las aplicaciones institucionales, garantizando **seguridad**, **trazabilidad** y **control de acceso** mediante el uso de **tokens JWT**.

[![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)](https://laravel.com/)
[![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)
[![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![Vue.js](https://img.shields.io/badge/Vue.js-42B883?style=for-the-badge&logo=vue.js&logoColor=white)](https://vuejs.org/)

---

## 🔐 Funcionalidades principales

### 1. Autenticación y autorización
- Inicio de sesión único (**SSO**) para todas las aplicaciones registradas.  
- Generación y validación de **tokens JWT** con caducidad configurable.  
- Implementación del flujo **OAuth2 / OpenID Connect (Authorization Code + PKCE)**.  
- Logout centralizado con invalidación de sesiones activas.

### 2. Gestión de usuarios
- Alta individual o masiva mediante importación de **archivos CSV**.  
- Políticas de contraseñas seguras y caducidad periódica.  
- Bloqueo temporal tras múltiples intentos fallidos.  
- Recuperación y cambio de contraseña desde el Portal de Usuario.

### 3. Roles y permisos (RBAC)
- Modelo **Role-Based Access Control** completo.  
- Creación y asignación de roles globales o específicos por aplicación.  
- Roles y permisos reflejados directamente en los **tokens JWT**.

### 4. Registro de aplicaciones cliente
- Registro y configuración de aplicaciones externas desde el Dashboard.  
- Control de **URLs de redirección**, **client_id** y **client_secret**.  
- Compatibilidad con **OAuth2 / OIDC** para integración de nuevas apps.

### 5. Portal de Usuario (React)
- Edición de perfil y cambio de contraseña.  
- Visualización de sesiones activas y revocación de accesos.  
- Historial de actividad y eventos de seguridad.  
- Gestión de tarjetas RFID (si aplica).

### 6. Seguridad y auditoría
- Registro de acciones críticas (logins, cambios de contraseña, bloqueos).  
- Protección ante fuerza bruta y rate limiting.  
- Hashing seguro de contraseñas y comunicación cifrada (**TLS/HTTPS**).  
- Firma asimétrica de tokens (**RS256**) y rotación periódica de claves.

---

## ⚙️ Tecnologías

- **Backend:** Laravel 
- **Frontend:** Vue (Dashboard), React (Portal de Usuario)  
- **Base de datos:** MySQL
- **Metodología:** Ágil (Scrum)

---

## 🧱 Arquitectura prevista

```mermaid
flowchart TD
    A[CentralAuth - IdP / SSO Core]
    A --> B[Dashboard Administrativo - Vue.js]
    A --> C[Portal de Usuario - React.js]
    A --> D[(MySQL Database)]
  ```
    

## 🚀 Como probar

> El sistema **aún no se puede probar**, ya que se encuentra en fase de análisis y documentación de requisitos.  
> Las fases de desarrollo e implementación comenzarán próximamente.



