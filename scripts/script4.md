### Requerimientos No Funcionales (RNF) Asociados

#### Seguridad

1. **Encriptación de Datos:**
   - **Descripción:** Todos los datos de autenticación deben ser encriptados.
   - **Relevancia:** Asegura que la información sensible (credenciales de usuario) esté protegida.

2. **Autenticación Multifactor (MFA):**
   - **Descripción:** El sistema debe soportar autenticación multifactor para garantizar una seguridad adicional más allá de la contraseña.
   - **Relevancia:** Proporciona una capa adicional de seguridad, reduciendo el riesgo de accesos no autorizados incluso si las credenciales son comprometidas.

3. **Política de Contraseñas:**
   - **Descripción:** Las contraseñas deben tener al menos 8 caracteres, incluyendo letras mayúsculas y minúsculas, números y caracteres especiales. Deben cambiarse cada 90 días.
   - **Relevancia:** Mejora la robustez de las contraseñas, disminuyendo la probabilidad de ataques de fuerza bruta o de adivinanza.

#### Rendimiento

4. **Tiempo de Respuesta:**
   - **Descripción:** El sistema debe procesar el inicio de sesión en menos de 2 segundos bajo condiciones normales de carga.
   - **Relevancia:** Garantiza una experiencia de usuario fluida y eficiente, esencial para mantener la satisfacción y productividad del usuario.

#### Disponibilidad

5. **Tiempo de Uptime:**
   - **Descripción:** El sistema de autenticación debe estar disponible el 99.9% del tiempo.
   - **Relevancia:** Asegura que los usuarios puedan acceder al sistema de manera continua, minimizando tiempos de inactividad que podrían afectar la operatividad del servicio.

#### Usabilidad

6. **Facilidad de Uso:**
   - **Descripción:** La interfaz de inicio de sesión debe ser intuitiva y cumplir con las pautas de accesibilidad web (WCAG 2.1).
   - **Relevancia:** Facilita el uso del sistema para todos los usuarios, incluyendo aquellos con discapacidades, mejorando la accesibilidad y la adopción del sistema.

#### Compatibilidad

7. **Compatibilidad con Navegadores:**
   - **Descripción:** El sistema debe ser compatible con los principales navegadores (Chrome, Firefox, Safari, Edge).
   - **Relevancia:** Asegura que el sistema pueda ser utilizado por una amplia gama de usuarios sin problemas de compatibilidad.

### Reflejo de los RNF en la Fase de Diseño

- **Encriptación de Datos:** Durante la fase de diseño, se deben seleccionar y configurar bibliotecas y protocolos de encriptación (como SSL/TLS) para asegurar que toda la comunicación entre el cliente y el servidor esté protegida.
- **Autenticación Multifactor:** Se diseñará un flujo de usuario que incluya la opción de autenticación multifactor, integrando mecanismos como la verificación por SMS, aplicaciones de autenticación, o correos electrónicos.
- **Política de Contraseñas:** Se implementarán restricciones de complejidad de contraseñas en la lógica de backend y se establecerá un sistema para recordar a los usuarios el cambio de contraseñas cada 90 días.
- **Tiempo de Respuesta:** Se optimizará la arquitectura del sistema, incluyendo la base de datos y los servicios de backend, para asegurar tiempos de respuesta rápidos. Esto podría incluir el uso de caché y optimización de consultas.
- **Tiempo de Uptime:** Se diseñará la infraestructura del sistema con redundancia y escalabilidad en mente, utilizando servicios en la nube que ofrezcan altos niveles de disponibilidad.
- **Facilidad de Uso:** Se realizará un diseño centrado en el usuario (UX) que sea intuitivo y accesible, cumpliendo con las pautas de accesibilidad web (WCAG 2.1).
- **Compatibilidad con Navegadores:** Se utilizarán tecnologías web estándares y se realizarán pruebas de compatibilidad en múltiples navegadores para asegurar el funcionamiento correcto en todos ellos.

### Verificación de los Requerimientos en la Fase de Pruebas

- **Encriptación de Datos:** Se realizarán pruebas de penetración y auditorías de seguridad para asegurar que todas las comunicaciones estén encriptadas adecuadamente.
- **Autenticación Multifactor:** Se realizarán pruebas funcionales para verificar que el flujo de MFA esté implementado correctamente y funcione bajo diferentes escenarios.
- **Política de Contraseñas:** Se realizarán pruebas unitarias y de integración para asegurar que las restricciones de complejidad de contraseñas y las políticas de cambio estén aplicadas.
- **Tiempo de Respuesta:** Se realizarán pruebas de rendimiento y carga para asegurar que el tiempo de respuesta del sistema de inicio de sesión sea menor a 2 segundos bajo condiciones normales de carga.
- **Tiempo de Uptime:** Se monitorizará el sistema utilizando herramientas de monitoreo en tiempo real para asegurar el cumplimiento del 99.9% de disponibilidad.
- **Facilidad de Uso:** Se realizarán pruebas de usabilidad y se recolectará feedback de usuarios para asegurar que la interfaz sea intuitiva y cumpla con las pautas de accesibilidad.
- **Compatibilidad con Navegadores:** Se realizarán pruebas de compatibilidad en los principales navegadores (Chrome, Firefox, Safari, Edge) para asegurar que el sistema funcione correctamente en todos ellos.

Estos métodos de verificación aseguran que tanto los requerimientos funcionales como los no funcionales sean cumplidos, proporcionando un sistema robusto, seguro y eficiente para la autenticación de usuarios.