# stack-android-free
### 📌 Objetivos del stack:

Framework multiplataforma que no dependa de Google ni de Meta.

Desarrollo y herramientas de código abierto.

Distribución privada fuera de Google Play y App Store, como alternativa a sus tiendas.

Seguridad y privacidad tanto para ti como para los usuarios.

## 🔧 1. Framework de desarrollo

### React Native (sin Expo)

React Native* es una de las mejores opciones para construir apps multiplataforma. Al usar React Native puro, evitas las dependencias pesadas de Expo, como el uso de Google Play Services y Firebase.
Ventajas*:
Permite escribir código nativo para iOS y Android.

Puedes optar por no integrar ninguna herramienta de Google/Meta.

Gran comunidad y ecosistema de librerías.

Desventajas*:
Necesitarás configurar ciertas funcionalidades manualmente, como las notificaciones push o servicios en segundo plano.
Alternativa a Expo*: Si no usas Expo, puedes prescindir de su ecosistema y tener control total sobre las dependencias que importas.
### Instalación básica (React Native sin Expo):

Instalar Node.js (LTS recomendado).

Instalar React Native CLI:

npm install -g react-native-cli
Crear un nuevo proyecto:
npx react-native init MiApp
### Librerías clave sin Google/Meta:

Notificaciones push*: usa librerías como react-native-push-notification o notifee (sin Google Firebase).
Base de datos*: en lugar de Firebase, puedes usar SQLite* o Realm*. Ambos son libres y locales, sin necesidad de servicios en la nube.
Geolocalización*: usa react-native-geolocation-service, sin necesidad de Google Play Services.
## 🏗️ 2. Desarrollo sin dependencias de Google/Meta

### Herramientas de desarrollo:

Android Studio (sin servicios de Google): Puedes usar Android Studio sin necesidad de integrar Google Play Services, pero ten en cuenta que algunas APIs de Android son inherentemente dependientes de Google (como Google Maps). Sin embargo, puedes omitir estas APIs y usar alternativas como OpenStreetMap para mapas.
Para trabajar sin Google Play Services, puedes deshabilitar la integración de Google en el archivo AndroidManifest.xml de tu proyecto.
Alternativa ligera a Android Studio*: Si prefieres algo más ligero, puedes usar VSCode* o IntelliJ IDEA* para escribir tu código y usar el terminal para construir el proyecto con el comando react-native run-android.
## 💻 3. Seguridad y privacidad

### Seguridad del entorno de desarrollo:

Contenedores o máquinas virtuales: Para minimizar riesgos, puedes trabajar en un entorno aislado, como una máquina virtual o contenedor Docker.

Revisar dependencias: Usa herramientas como npm audit para revisar vulnerabilidades en las dependencias de tu proyecto.

Uso de VPN o red segura: Si trabajas con datos sensibles o necesitas anonimizar tu tráfico, usa una VPN confiable durante el desarrollo.

### Auditoría de dependencias:

Usa herramientas como Snyk* o npm audit* para identificar vulnerabilidades en librerías y dependencias de tu proyecto.
## 🛠️ 4. Librerías alternativas (sin Google/Meta)

Aquí tienes algunas alternativas open-source que puedes usar para reemplazar servicios como los de Google y Meta:

Notificaciones Push:
react-native-push-notification: Alternativa a Firebase Cloud Messaging.

Notifee: Framework independiente para notificaciones push.

Autenticación:
Si necesitas autenticación, usa OAuth2 con un proveedor como Keycloak (open-source), o implementa una solución propia basada en JWT.
Base de datos:
SQLite: Base de datos local para almacenamiento en tu dispositivo, sin necesidad de servicios en la nube.

Realm: Base de datos local y autónoma, también sin necesidad de conectividad externa.

Mapas:
OpenStreetMap: Alternativa libre a Google Maps. Usa bibliotecas como react-native-maps para integrarlo en tu app.
Analítica y métricas:
Si necesitas analítica, usa herramientas como PostHog o Matomo, que son open-source y no recopilan datos de forma intrusiva.
## 📦 5. Distribución fuera de Google Play/Apple Store

Puedes distribuir tu app sin necesidad de usar las tiendas oficiales de Google y Apple. Aquí tienes algunas opciones:

F-Droid (Android):
F-Droid es una tienda de aplicaciones para Android que solo incluye software libre y abierto.

Proceso: Puedes enviar tu APK a F-Droid para que los usuarios lo descarguen de allí.

Distribución directa:
Puedes ofrecer tu APK directamente a los usuarios a través de tu propia web. Usar un CDN o una solución como IPFS para asegurar que el archivo sea distribuido de manera descentralizada.
Aurora Store:
Si deseas que los usuarios puedan descargar tu app sin usar Google Play, puedes usar Aurora Store, que es una alternativa de código abierto para acceder a las apps de Google Play sin necesidad de una cuenta de Google.
Alternativas a la App Store (iOS):
Para iOS, las opciones son más limitadas, pero puedes optar por distribuir tus apps mediante un perfil de Enterprise o TestFlight (en caso de que solo quieras que un grupo de usuarios acceda a tu app).
## 📜 6. Licencias y código abierto

Es importante que las herramientas y librerías que utilices tengan licencias claras y transparentes. Algunas buenas prácticas:

Licencias permisivas*: Como MIT, Apache 2.0 o BSD.
Evita software privativo*: Asegúrate de que todo el código que utilices sea de código abierto, y revisa las licencias para asegurarte de que se ajustan a tu visión.
## 🌱 Resumen del stack sugerido:

Framework*: React Native (sin Expo).
IDE*: Android Studio o VSCode.
Notificaciones*: react-native-push-notification o Notifee.
Base de datos*: SQLite o Realm.
Mapas*: OpenStreetMap.
Autenticación*: Keycloak (OAuth2).
Distribución*: F-Droid, distribución directa, Aurora Store.
