Análisis Básico de Vulnerabilidades en Aplicación Web (OWASP Juice Shop)

Autor: Jennifer Gabriela Rodríguez Jiménez  
Entorno: Ubuntu 22.04 LTS | Docker | VMware  
Fecha: Septiembre 2026  



Documentación Completa
Puedes consultar e inspeccionar el informe técnico completo en formato PDF directamente aquí:
[Descargar / Ver Informe PDF Completo](./Proyecto%20Análisis%20básico%20de%20vulnerabilidades%20en%20una%20aplicación%20web%20vulnerable%20dentro%20de%20un%20entorno%20virtual%20controlado.pdf)



Resumen del Proyecto
Este laboratorio práctico tuvo como objetivo identificar, analizar y documentar vulnerabilidades web fundamentales en un entorno local y controlado utilizando OWASP Juice Shop ejecutado en un contenedor Docker.

Herramientas Utilizadas
- VMware / Ubuntu 22.04 LTS: Entorno de virtualización y sistema operativo base.
- Docker: Contenedorización de la aplicación vulnerable.
- OWASP Juice Shop: Aplicación web objetivo para pruebas éticas.
- DevTools (Navegador Web): Inspección de tráfico y comportamiento HTTP.



Vulnerabilidades Analizadas

| # | Vulnerabilidad / Reto | Categoría OWASP | Impacto / Riesgo Principal |
|---|-----------------------|------------------|----------------------------|
| 1 | Password Strength | Broken Authentication | Acceso no autorizado a cuenta administrativa debido a credenciales débiles (`admin123`). |
| 2 | SQL Injection | Injection | Bypassing / evadir el formulario de autenticación e ingresar como usuario administrador mediante entradas no saneadas. |
| 3 | Improper Error Handling | Security Misconfiguration | Exposición innecesaria de información técnica o comportamiento inconsistente ante errores. |



Principales Recomendaciones de Mitigación
- Autenticación: Implementar políticas de contraseñas fuertes, limitar intentos de inicio de sesión y requerir Autenticación Multifactor (MFA).
- Inyecciones SQL: Utilizar consultas SQL parametrizadas (Prepared Statements) y sanear/validar todas las entradas de usuario.
- Manejo de Errores: Configurar mensajes de error genéricos orientados al usuario e implementar registro (logging) interno controlado para depuración.



Conclusión y Valor Aprendido
El proyecto permitió llevar conceptos teóricos de ciberseguridad a la práctica real en un entorno seguro, fortaleciendo competencias en gestión de contenedores Docker, comandos de Linux, metodología de documentación técnica e identificación de riesgos organizacionales.
