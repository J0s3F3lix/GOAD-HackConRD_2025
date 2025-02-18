# HackConRD2025_Atacando y Defendiendo Active Directory 

Este repositorio contiene información sobre las técnicas utilizadas en el workshop de **Ataque y Defensa de Active Directory**, donde utilizaran las siguientes técnicas de ataque y defensa en entornos de Active Directory (AD). donde lidere la parte de defensa en su totalidad. por eso traigo el listado de las actividades, pero solo me enfocare en presentar la parte de defesa.

## 🔥 Vulnerabilidades a Explotar Durante el Workshop  

### 🛠️ Acceso Inicial  
Técnicas utilizadas por atacantes una vez que han ingresado a la red corporativa:  
- **Kerberoasting** – Extracción de hashes de servicio Kerberos para descifrar contraseñas.  
- **ASREPRoasting** – Ataque contra cuentas que no requieren preautenticación en Kerberos.  
- **SMB Relay** – Ataque de retransmisión de autenticación en SMB para escalar privilegios.  

### 🚀 Explotación  
Técnicas utilizadas para **movimiento lateral**, **escalada de privilegios** y **enumeración de AD**:  
- **Enumeración con BloodHound** – Identificación de rutas de ataque dentro de AD.  
- **ADCS ESC4** – Abuso de Microsoft Active Directory Certificate Services para obtener acceso privilegiado.  
- **Abuso de ACLs (Listas de Control de Acceso)**:  
  - **GenericWrite** – Modificación de atributos en objetos de AD para escalar privilegios.  
  - **RBCD (Resource-Based Constrained Delegation)** – Abuso de delegación restringida para comprometer otras cuentas.  
  - **Shadow Credentials** – Inyección de credenciales en objetos de AD para persistencia y movimiento lateral.  

### 🎯 Post-Explotación  
Técnicas utilizadas por atacantes para **mantener persistencia** dentro del dominio:  
- **Pass-the-Hash** – Uso de hashes de contraseñas en lugar de credenciales en texto claro para autenticarse.  
- **Golden Ticket** – Creación de tickets Kerberos falsificados con privilegios de administrador de dominio.  
- **DCSync (NTDS.dit)** – Extracción de hashes de contraseñas desde el controlador de dominio.  

---


# 🔒 Defensa

Este directorio contiene la información de ataque para el workshop de **"Ataque y Defensa de Active Directory"**.

## 📢 Para el archivo: **GOAD_HackConRD2025_GPO**

Este archivo describe la estructura que recomendamos crear mediante una política de Active Directory (GPO). Contiene las mitigaciones básicas diseñadas para el ambiente específico de **Active Directory GOAD** (Game Of Active Directory). 

**Importante:** Esta estructura está pensada para un ambiente **GOAD** y **no debe ser ejecutada en otros entornos** sin antes verificar que las configuraciones sean adecuadas.

## 📢 Para el archivo: **GOAD_HackConRD2025_Script_AD**


- **Guardar como `.ps1`**: Este script debe guardarse con la extensión `.ps1` (por ejemplo, `GOAD_HackConRD2025_Script_AD.ps1`).
  
El script debe ser ejecutado con privilegios de administrador en el controlador de dominio donde se aplicará la configuración.
Este script está diseñado específicamente para un entorno de **Active Directory GOAD**. **No debe ser ejecutado en otros entornos** sin primero verificar que las configuraciones sean apropiadas.

---
👾 ¡Gracias por leer!👾
📢 **¡Contribuye!** Si tienes sugerencias, mejoras o encuentras errores, ¡haz un pull request o abre un issue! 🚀  
❤️ **Con amor, NickGitHub: [J0s3F3lix](https://github.com/J0s3F3lix)**  

