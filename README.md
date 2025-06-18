XTREET 
Descripción del Desarrollo
Realicé una landing page minimalista donde los usuarios pueden ver un poco de lo que es la empresa, ver sus productos y enviar sus datos de contacto mediante un formulario con un mensaje que comunique su necesidad. El sistema almacena la información en una base de datos MongoDB Atlas, a través de una API REST construida con el objetivo de que esas peticiones sean mostradas en alguna pantalla para que esas consultas o dudas sean atendidas y poder convertir a esas personas en potenciales clientes.
Herramientas que utilicé:
-	Frontend: React, TailwindCSS y Axios.
-	Backend: Node.js, Express, MongoDB Atlas, Zod y CORS / Morgan.
-	Deploy: Frontend en Vercel y Backend en Render
-	Base de datos: Mongo DB Atlas 

Instrucciones para Ejecutar el Proyecto
Para correr el deploy solo se debe ingresar al siguiente link https://xtreet.vercel.app/ . La base de datos se encuentra en la nube por lo que no se puede usar mediante este link sin correr el backend.

Backend
1.	Clona el repositorio:
-	git clone https://github.com/Fernando0312/XTREET_Back
-	cd XTREET_Back
2.	Instala dependencias:
-	npm install
3.	Crea archivo .env:
-	MONGO_URI=mongodb+srv://<usuario>:<clave>@cluster0.mongodb.net/ClientXtreet?retryWrites=true&w=majority
-	PORT=3001
4.	Ejecuta localmente:
-	npm run dev 
Frontend 
1.	Clona el repo:
-	git clone https://github.com/Fernando0312/XTREET_Front
-	cd XTREET_Front
2.	Instala dependencias:
-	npm install
3.	Archivo .env:
-	VITE_API_URL=https://xtreetback.onrender.com/api
4.	Ejecuta localmente:
-	npm run dev

Decisiones Técnicas
-	Separé el backend y el frontend para permitir escalabilidad.
-	Utilicé Zod para validaciones por su legibilidad y robustez.
-	MongoDB Atlas fue el elegido por ser gratuito, flexible, con compatibilidad cloud y es el entorno con el que estoy más familiarizado de bases NoSql.
-	Render y Vercel se usaron por su facilidad de deploy gratuito.
-	React Hook Form se implementó para el manejo limpio y validado de formularios.
-	TailwindCSS para dar un diseño responsivo, ligero y personalizable.
-	Utilicé React ya que es el framework que conozco más y que tengo un poco de experiencia.

Enlaces en Producción subidos a la nube
•	Backend: https://xtreetback.onrender.com
•	Frontend: https://xtreet-5qsc81mak-fernandos-projects-87ccc41a.vercel.app 
