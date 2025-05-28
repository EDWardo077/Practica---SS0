**Parte Práctica – Tema 2: Grupos de Trabajo**

1. Pulsa `Windows + R`, escribe `sysdm.cpl` y presiona Enter.
    
2. En la pestaña **Nombre de equipo**, haz clic en **Cambiar**.
    
3. Cambia el nombre del equipo a **SSO4** en todas las máquinas y confirma.
    
4. Haz clic derecho sobre la red a la que estás conectado, selecciona **Propiedades** y verifica que el perfil de red sea **Privado**.
    
5. Pulsa `Windows + R`, escribe `control` y presiona Enter.
    
6. Ve a **Centro de redes y recursos compartidos**, luego selecciona **Cambiar configuración de uso compartido avanzado** (panel izquierdo).
    

**Configuraciones a realizar:**

- **Privado:**
    
    - Activar detección de redes.
        
    - Activar uso compartido de archivos e impresoras.
        
- **Invitado o público:**
    
    - Activar detección de redes.
        
    - Activar uso compartido de archivos e impresoras.
        
- **Todas las redes:**
    
    - Activar uso compartido para carpetas públicas.
        
    - Desactivar el uso compartido con protección por contraseña.


---

## 🔧 **Parte Práctica para el Tema 3: Administración de Cuentas Locales**

### 🛠️ **Visualización de SID y SAT del Usuario**

**Objetivo**: Mostrar cómo un usuario puede ver su SID y token de seguridad (SAT).

### 📋 Actividad:

1. **Abrir PowerShell o CMD como administrador.**
    
    - Usa: `whoami /all`
        
2. **Explica los resultados:**
    
    - SID del usuario (línea principal).
        
    - Grupos a los que pertenece el usuario.
        
    - Privilegios locales (como `SeShutdownPrivilege`, etc.).
        
3. **Demuestra cómo crear un usuario local:**
    
    - En PowerShell:
        
        ```powershell
        net user UsuarioTest123 MiContraseña123 /add
        ```
        
    - Explica que se genera un nuevo SID para esa cuenta.
        
