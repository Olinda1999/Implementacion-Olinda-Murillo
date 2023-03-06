# Implementacion-Olinda-Murillo 
## Amazon CloudFront con carga de contenidos mediante Amazon S3
Paso 1: Buscar el servicio Amazon S3 luego elegir crear bucket.
![image](https://user-images.githubusercontent.com/126735151/223227950-6febe38e-e6d8-4926-afaa-cbfd29557dec.png)
Paso 2: Le ponemos un nombre, elegimos la región el resto lo dejamos todo por defecto por último hacer click en crear bucket.
![image](https://user-images.githubusercontent.com/126735151/223228156-b49cc014-2c5d-47b6-a160-2ec56ef4016b.png)
![image](https://user-images.githubusercontent.com/126735151/223228185-88d02b5c-666f-4f08-9d29-f6f51b0b3753.png)
Paso 3: Cargamos los archivos de la página para finalizar hacemos click en cargar. El archivo index.html (Archivo de un deber anterior).
![image](https://user-images.githubusercontent.com/126735151/223228252-775ea37c-7771-4301-82ef-7058ad669f47.png)
Paso 4: Buscamos el servicio Amazon CloudFront y hacemos click en “Create a Cloudfront Distribution”.
![image](https://user-images.githubusercontent.com/126735151/223228317-aab9842b-05d5-40d3-bf7f-aa36d289ec86.png)
Paso 5: En Origin Domain Name, introduce el nombre de dominio de tu bucket. Es importante que uses el dominio regional, el resto lo dejamos todo por defecto. 
![image](https://user-images.githubusercontent.com/126735151/223228360-51bf0248-bf5a-428a-bc08-8b3cf0b31b8b.png)
Paso 6: En Viewer Protocol Policy escoge Redirect HTTP to HTTPS. Por último, en Default Root Object introduce index.html. Haz click en Create Distribution.
![image](https://user-images.githubusercontent.com/126735151/223228430-0bb2f12d-6fbf-43ff-96b4-865fbaecc857.png)
Paso 7: Seleccionamos la distribución creada en “Origins” se edita el “Origin Access”, se escoge la secunda opción luego aparece un recuadro para crear una configuración de control.
![image](https://user-images.githubusercontent.com/126735151/223228512-154b1574-1dc3-42ae-b5fd-b3c830149211.png)
Paso 8: Se crea la configuración de control 
![image](https://user-images.githubusercontent.com/126735151/223228618-b5fb6940-d379-4c83-9361-c29849c843cd.png)
Paso 9: Luego de creado se copia la política.
![image](https://user-images.githubusercontent.com/126735151/223228690-c15eea4f-bed7-44f7-a5fc-97994417c831.png)
Paso 10: En el servicio de Amazon S3 en los permisos editamos la política de bucket y pegamos lo antes copiado.
![image](https://user-images.githubusercontent.com/126735151/223228753-285da044-c34f-40ff-a648-6bca50f35c9a.png)
Paso 11: Esperamos un momento y copiamos el “Domain name” de Amazon Cloudfront.
![image](https://user-images.githubusercontent.com/126735151/223228852-151d2db0-2c75-40cc-b339-27f7fdf04343.png)
Paso 12: Pegamos el enlace antes mencionado, aparecerá la pagina del archivo antes cargado.
![image](https://user-images.githubusercontent.com/126735151/223228904-cc32a79e-27cc-45c2-8767-9ed4dae3b292.png)
Luego usaremos la herramienta PingDom Tools para medir la velocidad de la página.
![image](https://user-images.githubusercontent.com/126735151/223228988-fac80fe9-36d1-4c0a-9140-5540b3c50dad.png)
