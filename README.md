# Ejercicio Práctico: Consumo de API en el Sistema del Hospital
## Descripción 
En esta actividad, se implementa el consumo de una API para obtener y mostrar datos del sistema del hospital utilizando useEffect y useState mediante peticiones asíncronas,ademas, se gestiona el estado y manejen los errores de manera eficiente.

### Implementación de Peticiones con useEffect y useState
Se simula el consumo de una APi (archivos json) mediante el uso de useEffect y useState para obtener todos los datos del sitio web del hospital.
### Uso de Fetch API o Axios para el Consumo de la API
Para consumir las APis simuladas a lo largo de la aplicación, se implementa el usi de Axios, su elección se debe, a que al ser una aplicación escalable a futuro, se pueden requerir necesidades mas avanzadas para manejar la información que fetch no proporciona, algunas de las ventajas de axios en lo cual se basa su elección de uso para este proyecto, son las siguientes:
 - Manejo automatico de errores
 - Sintaxis mas amigable, facilitando su implementación a lo largo del codigo.
 - Permite establecer un tiempo de espera de la respuesta y también la capacidad de cancelar peticiones.
 - Proporciona un conjunto completo de opciones de configuración para las solicitudes, como la incorporación de encabezados.
 - Automáticamente transforma las respuestas en JSON.
### Peticiones Basadas en Eventos del Usuario
Se permite que el usuario realice una petición a una API, al presionar el boton "Cargar lista completa" en la sección servicios(equipo medico). al seleccionar, esta opción se llama a la APi doctorsComplete que entrega información de mas doctores del hospital, la cual, se visualiza en pantalla.
### Manejo de Errores en Peticiones Asíncronas
Para que el usuario conozca si existe un error al consumir una API se implementa el uso de sweetalerts que envian un mensaje informativo en caso de existir un error, ademas, se pregunta al usuario si desea intentarlo nuevamente (llamando nuevamente a la API) o cancelar la acción.

### Estructura principal de carpetas
- **assets:** carpeta que contiene los elementos graficos del sitio web, en este caso, imagenes.
- **components:** carpeta que contiene todos los componentes creados y utilizados en el sitio web, como header y footer.
- **public:** contiene los archivos JSON con los cuales se trabaja.
  - appointment.json: archivo que contiene toda la información asociada las citas medicas registradas
  - doctors.json: archivo que contiene toda la información respecto a cada doctor de la clinica.
  - doctorsComplete.json: archivo que contiene un segundo arreglo con información de doctores. esta información es la que se muestra al presionar el boton "Cargar lista completa" en la seccion de servicios (equipo medico).
  - services.json: archivo que contiene toda la información respecto a cada servicio medico ofrecido por la clinica a sus pacientes.
- **views:** contienen la estructura basica de las 5 pantallas principales del sitio web, desde ellas se llaman y utilizan los componentes.
  - contact: contiene la pantalla asociada al formulario de contacto.
  - home: pantalla principal del sitio, aqui, se listan los servicios ofrecidos por la clinica, llamando al componente ServiceList.
  - services: presenta información asociada al equipo medico de la clinica, llamando al componente DoctorCard.
  - RegisterAppointment: presenta un listado con todas las citas medicas registradas.
  - Appointment: contiene el formulario que permite agendar una cita medica, llamando al componente AppointmentForm.
 
 ### Visualización del proyecto
Para visualizar este proyecto se necesita que previamente cuentes con la instalación de:
- **Git**: [sitio de descarga] (https://git-scm.com/downloads)
- **Node.js**: [sitio de descarga] (https://nodejs.org/en/download/package-manager)
- **Visual Studio Code**: [sitio de descarga] (https://code.visualstudio.com/download)
  
Una vez que ya cuentes con lo descrito anteriormente, debes clonar este repositorio en una carpeta local, mediante el siguiente comando:
```bash
git clone https://github.com/lorenasotosanmartin/M5_EP1.git
```
cuando ya este clonado, escribir el siguiente comando en la consola: 
```bash
npm  i
```
y ejecutar el comando, para inicializar el proyecto: 
```bash
npm run dev
```
Finalmente, para visualizar el proyecto en tu navegador debes abrir la url http://localhost:3000/ 
