Sponzy v6.8
Bienvenido al repositorio oficial de Sponzy, una plataforma social enfocada en creadores de contenido que integra monetización, streaming y experiencias de comunidad en un solo lugar. Aquí encontrarás todo lo necesario para desplegar, personalizar y evolucionar la aplicación.

¿Qué incluye este repositorio?
Documentation/
Manuales HTML con la guía oficial del producto: instalación, configuración, novedades por versión y buenas prácticas para upgrades.

MySQL/
Un volcado completo (sponzy.sql) con el esquema de base de datos tal como se usa en producción. Ideal para levantar entornos locales o analizar la estructura real de datos.

Script/
El corazón de la app: un proyecto Laravel con todo el código fuente (controladores, modelos, vistas, jobs, colas, assets front-end, etc.), listo para compilarse con Vite y correr en cualquier stack PHP moderno.

Upgrades/
Paquetes y notas HTML para actualizar desde versiones anteriores. Si vienes de una release distinta, aquí tienes los pasos y parches necesarios para migrar sin sorpresas.

¿Qué hace única a Sponzy?
Monetización avanzada
Compatible con múltiples pasarelas (Stripe, PayPal, Paystack, MercadoPago, CCBill, etc.), cálculos de comisiones flexibles y soporte para Stripe Tax. Ideal para construir negocios basados en suscripciones y propinas.

Procesamiento multimedia robusto
Jobs en cola con FFmpeg para codificar videos, generar miniaturas, aplicar marcas de agua y moderar automáticamente antes de publicar.

Experiencia social completa
Feeds, historias, mensajería, streaming en vivo, recomendaciones y verificación de cuentas, todo orquestado desde controladores y traits reutilizables.

Internacionalización y cumplimiento
Interfaces totalmente traducibles, banderas para contenidos adultos, avisos legales y personalización de temas.

Automatización lista para producción
Cron jobs para limpieza, rebilling, expiraciones y moderación, más eventos/notificaciones que mantienen informados a usuarios y administradores.

¿Cómo empezar?
Revisa la documentación en Documentation/ para entender requisitos y configuración recomendada.

Importa el esquema desde MySQL/sponzy.sql para tener la base de datos lista.

Instala dependencias PHP (Composer) y front-end (NPM/Vite) dentro de Script/.

Configura tus credenciales de pagos, storage y correo siguiendo los ejemplos .env.

Lanza las colas y el scheduler para manejar encoding, rebilling y notificaciones.

Hoja de ruta de aprendizaje
Si eres nuevo en Laravel o en el dominio de Sponzy, te recomendamos:

Dominar rutas, middleware y controladores de Laravel.

Profundizar en Eloquent y relaciones (suscripciones, transacciones, planes).

Entender colas, jobs y scheduler para mantener procesos críticos.

Revisar integraciones externas (pagos, OAuth, storage) y eventos/notificaciones.

Familiarizarte con Blade, Bootstrap 5, Axios y Vite para los ajustes front-end.

Leer la documentación y scripts de actualización antes de desplegar.

¿Quieres contribuir?
¡Nos encanta la colaboración! Te sugerimos:

Crea una nueva rama desde main para tu feature o fix.

Asegúrate de que las pruebas y los jobs relevantes se ejecuten correctamente.

Abre un Pull Request explicando tu cambio y enlazando cualquier issue asociado.

Ideas para aportar:

Mejorar la experiencia de onboarding o la documentación.

Añadir cobertura de tests en áreas críticas (pagos, multimedia, eventos).

Optimizar jobs y pipelines de encoding.

Extender integraciones con nuevas pasarelas o herramientas de streaming.

Diseñar nuevos componentes front-end o experiencias de usuario.

Licencia & soporte
Consulta el archivo LICENSE (si está disponible) o la documentación incluida para conocer los términos de uso. Para soporte comercial o preguntas específicas, revisa las guías en Documentation/.

