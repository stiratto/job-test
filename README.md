# RESPUESTAS:

## A) Verdadero / Falso
1. Next.js 14 introduce nuevos Server Actions que permiten ejecutar lógica del lado
del servidor sin necesidad de un endpoint API adicional: Verdadero

3. En React 18, la función useEffect se ejecuta antes de renderizar el componente en
la pantalla: Falso

5. El tipado en TypeScript elimina por completo los errores en tiempo de ejecución al
compilar el proyecto: Falso

7. TanStack Query permite manejar la caché de datos y revalidación de manera
automática, optimizando solicitudes HTTP: Verdadero

9. ShadCN está enfocado únicamente en la creación de dashboards empresariales
sin posibilidad de uso general: Falso

11. Los Route Handlers en Next.js 14 (app/api/.../route.ts) permiten crear un BFF que
unifique múltiples fuentes de datos bajo contratos propios: Verdadero

13. CORS y CSRF resuelven exactamente el mismo problema de seguridad en
aplicaciones web: Falso

15. En React Native, el DOM no existe; la UI se renderiza con vistas nativas, por lo que
ciertos estilos o APIs del navegador no aplican: Verdadero

17. El almacenamiento offline en React Native puede resolverse con AsyncStorage,
pero también es común usar React Query con persistencia: Verdadero

19. Un índice apropiado en base de datos puede reducir tiempos de lectura en
órdenes de magnitud; sin embargo, puede penalizar las escrituras: Verdadero


## B) Opción Múltiple (una sola respuesta correcta)


11. Respecto a las Server Components de Next.js 14, ¿cuál es su principal ventaja? A.
Generar el HTML en el cliente para mejorar el SEO.
B. Renderizar componentes en el servidor, reduciendo el JavaScript que se envía al
cliente. (X)
C. Reemplazar por completo la necesidad de TypeScript en el proyecto.
D. Aumentar el tamaño de los bundles finales del cliente.

13. Para implementar Incremental Static Regeneration (ISR) con Next.js, ¿qué se
requiere?
A. Llamar a un hook especial useISR() dentro de nuestro componente.
B. Configurar la opción revalidate al usar getStaticProps(). (X)
C. Implementar únicamente getServerSideProps() con un parámetro adicional.
D. Deshabilitar la funcionalidad de SSR en su totalidad.

15. ¿Cuál de estas ventajas describe mejor el uso de TypeScript en un proyecto
React/Next?
A. Evita que el código JavaScript sea accesible para navegadores antiguos.
B. Permite crear interfaces y tipos para ayudar a detectar errores de forma anticipad (X).
C. Anula la necesidad de usar librerías para validación en tiempo de ejecución.
D. Genera automáticamente la documentación del proyecto.

17. Si utilizamos TanStack Query en lugar de un estado global manual para manejar
datos (por ej. fetch de usuarios), ¿qué mejora principal obtenemos?
A. Carga forzada de datos en cada renderizado sin caché.
B. Cacheo y revalidación automática de datos, reduciendo llamadas innecesarias a la
API. (X)
C. Reemplazo automático de Next.js enrutamiento.
D. Un framework de pruebas integrado para testear endpoints.

18. ¿Cuál de estas afirmaciones sobre ShadCN es cierta?
A. Es una colección de componentes (como botones, modales, etc.) creada para
React, con énfasis en accesibilidad y personalización. (X)
B. No permite modificar ni un solo estilo en sus componentes, son totalmente
cerrados.
C. Se usa únicamente en proyectos Angular.
D. Hace render del lado del servidor sin necesidad de Next.js.

20. ¿Qué patrón es más apropiado para un BFF en Next.js 14?
 A. Conectar el cliente directamente a todas las APIs externas.
 B. Implementar route handlers con esquemas Zod que hagan fetch a APIs externas y
devuelvan DTOs propio. (X)
 C. Poner toda la lógica en useEffect y hacer fetch desde el cliente.
 D. Servir JSON estático embebido en el bundle.

22. ¿Cuál es la mejor estrategia para validar inputs en endpoints de escritura (POST)
del BFF?
 A. Validar solo en el cliente.
 B. Validar en el servidor usando esquemas (p. ej. Zod) y devolver errores tipados. (X)
 C. No validar: JSONPlaceholder no lo exige.
 D. Rechazar todo POST.

24. En React Native, ¿cuál es una forma común de navegación entre pantallas?
 A. next/link
 B. React Navigation (stack/tab) (X)
 C. Anclas (<a href="#id">)
 D. window.history.pushState

25. ¿Qué encabezado HTTP permite una política de caché que sirva contenido
guardado mientras se revalida en background?
 A. Cache-Control: no-store
 B. Cache-Control: private
 C. Cache-Control: stale-while-revalidate=... (X)
 D. ETag: *

26. ¿Qué opción describe mejor una optimización de performance en web y mobile
para listas largas?
 A. Renderizar toda la lista de una vez.
 B. Virtualización (p. ej. FlatList/SectionList en RN, virtual scroll en web). (X)
 C. Poner overflow: hidden.
 D. Deshabilitar el JS minificado.

## Desafios Tecnicos

Ejercicio 1: https://github.com/stiratto/app-1-next
Ejercicio 2: https://github.com/stiratto/app-2-native
