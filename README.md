🧪 Proyecto Final – QA Manual & API Testing

Autora: Yuli Riveros

🎯 Objetivo del Proyecto

Evaluar la calidad funcional de la aplicación Instagram Lite y realizar pruebas de integración sobre la FakeStoreAPI, aplicando buenas prácticas de Testing Manual y Testing de API.
El propósito fue validar el comportamiento esperado de las principales funcionalidades, detectar defectos y documentar hallazgos de forma profesional.

🧭 Alcance del Testing
🔹 Qué se testeó

Funcionalidades principales: login, registro, dar “like”, navegación y publicación.

Flujo de usuario en entorno móvil real (Android – Samsung).

Endpoints clave de la API (GET, POST, PUT y validaciones de estructura JSON).

🔹 Qué no se testeó

Pruebas de rendimiento o carga.

Base de datos o notificaciones push.

Pruebas de seguridad o integración con redes externas.

⚙️ Entorno de Pruebas
Tipo	Detalle
Aplicación	Instagram Lite
Dispositivo	Samsung (Android)
Navegador / API Tool	Google Chrome / Postman
API utilizada	FakeStoreAPI

Metodología aplicada	Simulación de Sprints semanales (planificación, ejecución, retrospectiva)
Gestión de evidencias	Planillas y reportes en formato Excel y carpetas estructuradas dentro del repositorio
📊 Resultados Generales
✅ Funcional Testing (Instagram Lite)

Se validaron los flujos principales del usuario con resultados mayoritariamente exitosos.

Se detectaron fallas menores en carga de publicaciones y subida de imágenes.

Las funcionalidades críticas (login, navegación, “like”) funcionaron según lo esperado.

🌐 API Testing (FakeStoreAPI)

3 endpoints positivos: GET /products, POST /products, PUT /products/1 → todos respondieron 200 OK / 201 Created.

1 caso negativo: GET /products/9999 → body vacío, respuesta aceptada según la documentación.

1 validación de estructura JSON: exitosa.

🐞 Defectos Críticos Detectados
ID	Descripción	Severidad	Estado
BUG-01	Error “Función no disponible” al intentar subir video	Alta	Bloqueado
BUG-02	Lenta actualización del feed en red inestable	Media	Pendiente revisión
BUG-03	Fallo intermitente al cargar imágenes	Media	Abierto
📈 Conclusiones

El producto presenta un comportamiento estable y funcional.
Los casos críticos fueron gestionados y documentados, mostrando buena trazabilidad entre historias, pruebas y resultados.
El sistema está listo para pruebas de regresión y validaciones previas a su paso a producción.

💡 Recomendaciones

Mejorar la carga dinámica del contenido en Instagram Lite.

Optimizar manejo de red y mensajes de error en conexión inestable.

Continuar pruebas en distintos modelos Android.

Automatizar los casos de API críticos para próximos sprints.

📂 Estructura del Repositorio
/historias_usuario         → Historias y criterios de aceptación
/casos_de_prueba           → Matriz de pruebas funcionales
/bugs                      → Reporte de bugs con evidencias
/api_testing               → Casos y resultados de API Testing + capturas
/documentos                → Informe final y presentaciones
README.md                  → Descripción general del proyecto

🚀 Reflexión Final

Este proyecto me permitió aplicar habilidades en análisis funcional, documentación, gestión de defectos y comunicación de resultados, dentro de una dinámica de trabajo ágil simulada por sprints.
Refleja mi enfoque como QA: detallista, organizada y orientada a resultados medibles.
