
# Sistema de Gestión de Personas con Java EE

**Readme y proyecto realizado por Jorge Herraiz Soler — Todos los derechos reservados, prohibida su reproducción sin autorización del autor [@jherraizsoler](https://github.com/jherraizsoler)**

---

## 📌 Descripción del Proyecto
Este proyecto es una aplicación web empresarial para la **gestión de personas**, desarrollada sobre la plataforma **Java EE (Jakarta EE)**.  

Implementa la arquitectura **MVC (Modelo-Vista-Controlador)** y utiliza **CDI** para la inyección de dependencias, garantizando un diseño desacoplado y mantenible.  

La aplicación permite realizar operaciones **CRUD (Crear, Leer, Actualizar, Borrar)** sobre la información de personas y usuarios.  

La **persistencia de datos** se gestiona con **JPA + EclipseLink** en una base de datos **MySQL**.  
La **interfaz de usuario** está construida con **JSF (JavaServer Faces)** y **PrimeFaces**, proporcionando una experiencia rica y moderna.

---

## ⚙️ Tecnologías Principales
- **Backend:** Java, Jakarta EE, EJB, JPA, EclipseLink  
- **Frontend:** JSF, PrimeFaces  
- **Inyección de Dependencias:** CDI (Contexts and Dependency Injection)  
- **Base de Datos:** MySQL  
- **Servidor:** GlassFish Server  
- **Gestor de Dependencias:** Maven  

---

## 🚀 Procedimiento para iniciar desde cero este proyecto (`Personas-JEE-WEB`)

### 1. Requerimientos Técnicos y Prácticos
- Tener **Apache NetBeans IDE 26** instalado.  
- Tener instalado el **JDK 21**  
  ```bash
  java -version
  # output esperado: 21.0.7
  ```
- Tener instalado **GlassFish Server 8.0.0**  
  - En NetBeans:  
    `Propiedades > Java (Pestaña) >> Java Platform JDK => JDK 21`  

📄 Si no tienes GlassFish Server 8.0.0:  
[readmeInstallGlassfishServer8.0.0.md](Documentation/readmeInstallGlassfishServer8.0.0.md)

---

### 2. Procedimiento para Application Deploy (`Personas-JEE-WEB`)
1. Instalar **MySQL Workbench 8.0.42 (Community Version)**  
2. En MySQL Workbench crear un **Schema** llamado `test`.  
3. Importar la base de datos:  
   - `Server > Data Import`  
   - Seleccionar la carpeta `Documentation/importarBD_test` y darle a **Importar**.  
4. Configurar **GlassFish Server 8.0.0** si no está instalado.  
   - 📄 [readmeInstallGlassfishServer8.0.0.md](Documentation/readmeInstallGlassfishServer8.0.0.md)  
5. Configurar los **DataSource** en GlassFish:  
   - `PersonaPool / PersonaDB`  
   - `UsuarioPool / UsuarioDB`  

📄 Guía de configuración:  
[readmeConfigurateDataSourceGlassfish.md](Documentation/readmeConfigurateDataSourceGlassfish.md)  

---

✅ Con esto tendrás tu proyecto **listo para compilar y ejecutar** en **NetBeans + GlassFish + MySQL** 🚀
