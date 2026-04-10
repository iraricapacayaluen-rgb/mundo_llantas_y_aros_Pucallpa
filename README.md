# Sistema de Gestión "Mundo Llantas & Aros"
Sistema web integral para el control de asistencia biométrica, gestión de inventarios y facturación electrónica.
Desarrollado como solución tecnológica para modernizar la operatividad del sector automotriz en Pucallpa

## Descripción del Negocio
Nombre: Mundo Llantas & Aros Pucallpa.
Giro: Comercialización de neumáticos y aros, con servicios técnicos de balanceo, alineamiento y reparación.
Tamaño: Empresa con personal técnico especializado en diversas áreas operativas.
Contexto: Actualmente operan con registros manuales en papel, lo que genera errores, pérdida de datos y riesgos de suplantación.
Justificación: Se requiere digitalizar el control de personal y el stock para evitar retrasos por medidas incorrectas de llantas y falta de veracidad en la asistencia

## Identificar el Problema y Solución

Problema: Gestión manual de entradas/salidas, errores en el conteo de inventario y
lentitud en el despacho de productos hacia los clientes
Solución Tecnológica: Implementación de un Software ERP integrado con un lector
biométrico ZKTeco y dispositivos PDA para el escaneo de códigos de barras/QR

## Requerimientos Funcionales

| Codigo | Descripcion |
|---|---|
| RF01 |El sistema debe capturar la huella dactilar (ZKTeco) para marcar entrada, salida y refrigerio|
| RF02 | Cada venta realizada debe descontar automáticamente el stock del inventario  |
| RF03 | Generación de boletas y facturas electrónicas (PDF/XML) vinculadas a SUNAT|
| RF04 | El administrador debe poder justificar tardanzas o faltas de forma manual|
| RF05 |Emisión de reportes: ventas diarias, ranking de productos y récord de asistencia|


## Requerimientos No Funcionales

| Codigo | Tipo | Descripcion |
|---|---|---|
| RNF01 | Seguridad | Impedir acceso no autorizado mediante roles (Vendedor, Almacenero, AdminImpedir acceso no autorizado mediante roles (Vendedor, Almacenero, Admin)|
| RNF02 | Disponibilidad  | Sistema basado en la nube (Cloud) accesible 24/7 vía web o móvil |
| RNF03 |Integridad | Los registros de huellas no deben ser alterables por los trabajadores |
| RNF04 |Rendimiento | La validación de huella y emisión de boletas debe tardar entre 3 a 5 segundos |


## Stack completo
1.  Gestión        = Trello (Kanban).
2 . Diseño         = Figma (UI/UX) y Draw.io (Diagramas).
3.  Base de Datos  = MySQL Workbench y MySQL 8.
4.  esarrollo      = IntelliJ IDEA (Java Spring Boot 3).
5.  Servidor       =XAMPP (Tomcat) o Despliegue en la Nube (Cloud)



## Tecnologias utilizadas 
- Java 17
- Spring Boot 3
- MySQL 8
- HTML5, CSS3, JavaScript
- IntelliJ IDEA
- XAMPP (Tomcat)
- MySQL Workbench
- Figma (diseño UI/UX)
- Draw.io (diagramas)
---


## Estructura del proyecto

```
Sistema-MundoLlantas/
├── backend/          → Spring Boot (Java)
│   ├── src/
│   ├── pom.xml
│   └── ...
├── frontend/         → HTML, CSS, JS|
│   ├── css/
│   ├── js/
│   └── index.html
```
----

## Base de datos
El sistema cuenta con 3 tablas principales identificadas 

|Tabla |Descripción |
|---|---|
|ASISTENCIA | Registro de marcas biométricas (entrada/salida) de los trabajadores |
|INVENTARIO_VENTAS | Control de stock de llantas/aros y registro de transacciones comerciales |
|USUARIO_TURNO | Gestión de accesos, roles de usuario y horarios asignados | 


https://github.com/ojitoslanda/JavaWeb-GotaGota/tree/main?tab=readme-ov-file#modelo-relacional-mr











