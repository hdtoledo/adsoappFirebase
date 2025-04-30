# 📱 ADSO Android App – Login & Registro con Firebase

Una aplicación Android desarrollada en Java como parte del proceso formativo en el programa **ADSO (Análisis y Desarrollo de Software)**. Esta app implementa un sistema de autenticación básica (login y registro) utilizando **Firebase Authentication**, con navegación entre pantallas y diseño basado en Material Design.

---

## ✨ Características

- 🧑 Registro de nuevos usuarios con correo y contraseña.
- 🔐 Inicio de sesión con validación de credenciales.
- 🚪 Cierre de sesión (logout) con manejo de sesión en Firebase.
- ➡️ Redirección a una pantalla de bienvenida (`HomePage`) después del login.
- 🎨 Interfaz gráfica moderna usando `TextInputLayout`, `EditText` y estilos de Material Components.
- 🔁 Verificación de sesión activa para evitar reingreso manual si el usuario ya está autenticado (opcional).
- 🔥 Conexión a Firebase en tiempo real con soporte de autenticación segura.

---

## 📂 Estructura del Proyecto

```
app/
├── java/
│   └── com.example.adso02/
│       ├── MainActivity.java          # Pantalla de Login
│       ├── RegisterActivity.java      # Pantalla de Registro
│       └── HomePage.java              # Pantalla post-login con botón de logout
├── res/
│   ├── layout/
│   │   ├── activity_main.xml          # Diseño de Login
│   │   ├── activity_register.xml      # Diseño de Registro
│   │   └── activity_home_page.xml     # Diseño del HomePage
│   └── drawable/
│       └── login.png, round_btn.xml   # Recursos gráficos
```

---

## ⚙️ Tecnologías Usadas

- **Lenguaje:** Java
- **Entorno:** Android Studio
- **Autenticación:** Firebase Authentication
- **UI Components:** Material Components (`TextInputLayout`, `Button`, `EditText`)
- **Firebase SDK:** Versión recomendada en `build.gradle`

---

## 🚀 Cómo ejecutar el proyecto

1. Clona este repositorio:

```bash
git clone https://github.com/hdtoledo/adsoappFirebase.git
```

2. Abre el proyecto con **Android Studio**.

3. Configura tu proyecto en [Firebase Console](https://console.firebase.google.com):
   - Crea un nuevo proyecto.
   - Habilita **Authentication** → método **Email/Password**.
   - Descarga el archivo `google-services.json` y colócalo en la carpeta `app/`.

4. Sincroniza el proyecto (`Sync Project with Gradle Files`).

5. Ejecuta en un emulador o dispositivo físico.

---

## 🔐 Consideraciones de seguridad

- Esta app utiliza Firebase Authentication en modo básico.
- No almacena contraseñas localmente.
- Ideal para pruebas académicas y como base para apps con autenticación.

---

## 🧠 Futuras mejoras (sugerencias)

- Validación de campos (regex, errores de formulario).
- Recuperación de contraseña.
- Persistencia de sesión con SharedPreferences.
- Uso de Firestore para almacenar perfiles de usuario.
- Implementación con `ViewModel` y `LiveData`.

---

#

## 🤝 Autor

**Héctor David Toledo García**  
Desarrollador FullStack
📧 hdtoledo@gmail.com  
🌐 [hdtoledo.dev](https://www.hdtoledo.dev/)  

---

## 📄 Licencia

Este proyecto está licenciado bajo los términos de uso educativo y de libre modificación para fines no comerciales.