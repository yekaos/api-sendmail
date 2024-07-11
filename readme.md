# API SEND-MAIL

## NOMBRE
API SendMail

## DESCRIPCIÓN

Se trata de una API simple para enviar correos electrónicos al webmaster utilizando PHP. 
Este README proporciona una guía básica para entender y utilizar la API. Asegúrate de personalizar los detalles como la URL del endpoint y la configuración del correo del webmaster según tu entorno específico.

## INSTALACIÓN

1. Clona el repositorio o descarga los archivos en tu servidor web.
2. Asegúrate de tener PHP instalado y configurado correctamente.
3. (OPCIONAL) - Se recomienda instalar PaperCut SMTP.

## USO

- En cuanto a parámetros, deberemos rellenar lo siguiente en **sendmail.http** para que la API funcione correctamente:

1. name (string): Nombre del remitente del correo.
2. email (string): Dirección de correo electrónico del remitente.
3. message (string): Mensaje que el remitente desea enviar.

- En **index.php**, configurar la URL del endpoint a tu servidor correspondiente.
- En **index.php**, configurar la dirección de correo del webmaster para que llegue al destinatario correspondiente.

## EJEMPLO DE SOLICITUD

POST http://localhost/api/v1/endpoint-webservice/

{
  "name":"Lamine",

  "email":"lamine@example.com",

  "message":"Buenos días, ¿qué tal?"
}

**Este ejemplo muestra cómo puedes enviar una solicitud POST a tu API usando cualquier cliente HTTP compatible con JSON, como cURL, Postman, o incluso desde tu propio código en PHP, Python, JavaScript, etc. Asegúrate de ajustar la URL y los datos según tus necesidades específicas.**