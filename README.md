# Ejercicio Práctico: Integración Completa del Sistema del Hospital con ReactJS
## Descripción 
En esta actividad, todas las vistas del sistema del hospital (Home, Servicios, Equipo Médico, Citas) deberán integrar componentes avanzados y técnicas de optimización de ReactJS.Ademas, se manejarán interacciones complejas con datos a través de APIs.

### Estructura principal de carpetas
- **assets:** carpeta que contiene los elementos graficos del sitio web, en este caso, imagenes.
- **components:** carpeta que contiene todos los componentes creados y utilizados en el sitio web, como header y footer.
- **public:** contiene los archivos JSON con los cuales se trabaja.
  - appointment.json: archivo que contiene toda la información asociada las citas medicas registradas
  - doctors.json: archivo que contiene toda la información respecto a cada doctor de la clinica.
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
git clone https://github.com/lorenasotosanmartin/M4_EP1.git
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
