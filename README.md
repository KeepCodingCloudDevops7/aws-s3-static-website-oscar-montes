# Despliegue Website Estático en AWS S3 Bucket - Óscar Montes

Este proyecto utiliza Terraform para el despliegue en la región de Irlanda de un bucket S3 en el cual se aloja un sitio web estático compuesto por dos ficheros HTML (index.html y error.html). Al final del despligue, mostrará el acceso web al mismo mediante el endpoint de conexión.

## Requisitos previos

- Cuenta de AWS.
- AWS CLI y Terraform instalado en su sistema

## Despliegue

1. Clone el repositorio en local.
2. Acceda a la carpeta www e inicialice Terraform:

   ```
   terraform init
   ```
3. Planificar el despliegue mediante el siguiente comando:

   ```
   terraform plan
    ```
4. Finalmente, realice el despligue:

    ```
    terraform apply
    ```
5. Al final del mismo, aparecerán los outputs configurados. Copiar el enlace del website_endpoint en el navegador para acceder al sitio Web:

   ```
   Outputs:

   s3_first_bucket_arn = "arn:aws:s3:::kc-bucket-om"
   s3_first_bucket_name = "kc-bucket-om"
   website_endpoint = "kc-bucket-om.s3-website-eu-west-1.amazonaws.com"  <<<<
   ```

6. Una vez realizada la actividad, recomendamos la eliminación de los recursos generados:

   ```
   terraform destroy
    ```

