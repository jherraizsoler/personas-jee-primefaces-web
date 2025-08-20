
**                 Readme y proyecto realizado por Jorge Herraiz Soler tiene todos derechos reservados, prohibido sin autorización del autor @jherraizsoler        **
---
# Procedimiento para iniciar desde cero este proyecto (Personas-JEE-WEB)                          
---

---
## 1. REQUERIMIENTOS TECNICOS  Y  PRACTICOS

1. Tener Apache Netbeans IDE 26  
 
2. Tener instalado el jdk-21  
   | java -version 21.0.7 | 

3. Tener instalado GassFish Server 8.0.0  
   | Propiedades > Java (Pestaña) >> Java Platform JDK =>  JDK 21  | 

   Vinculo (revisar en caso de no tener instalado GassFish Server 8.0.0 )
        - Archivo  / url  --  Documentation/readmeInstallGlassfishServer8.0.0.md
---

---
## 2. PROCEDIMIENTO   APPLICATION   DEPLOY Personas-JEE-WEB

1. Tener instalado MySQL Workbench 8.0.42  (Community Version)

2. Dentro de MySQL Workbench crear Schema con el nombre test 

3. Dentro de MySQL Workbench en Server > Data Import  seleccionar la carpeta que esta en Documentation que se llama importarBD_test y darle a importar

4. Tener instalado Glassfish Server 8.0.0 en caso de no tenerlo instalado 
    - Archivo  / url  --  Documentation/readmeInstallGlassfishServer8.0.0.md

5. Configurar el DataSource  PersonaPool / PersonaDB  dentro de Glassfish 
    - Archivo / url  --  Documentation/readmeConfigurateDataSourceGlassfish.md

6. Configurar el DataSource  UsuarioPool / UsuarioDB  dentro de Glassfish 
    - Archivo / url  --  Documentation/readmeConfigurateDataSourceGlassfish.md


7. Dentro del paquete cliente.ciclovidajpa tenemos 5 archivos .java que nos 
   permitiran poder gestionar y testear operaciones CRUD con Personas y Usuarios

        > EncontrarObjetoJPA.java
        > PersistirObjetoJPA.java
        > ActualizarObjetoJPA.java
        > ActualizarObjetoSesionLarga.java
        > EliminarObjetoJPA.java
---