# HackConRD2025_Atacando y Defendiendo Active Directory 

Este repositorio contiene información sobre las técnicas utilizadas en el workshop de **Ataque y Defensa de Active Directory**, donde utilizaran las siguientes tecnica de ataque y defensa en entornos de Active Directory (AD). donde lidere la parte de defensa en su totalidad.

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

### 📌 Nota Importante  
Este workshop fue diseñado exclusivamente para entornos **controlados y de pruebas**. Las técnicas aquí descritas deben ser utilizadas únicamente con fines educativos y de auditoría de seguridad. El uso indebido de estas herramientas en sistemas sin autorización puede ser ilegal.  

---


