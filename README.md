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

5. Una vez realizada la actividad, recomendamos la eliminación de los recursos generados:

   ```
   terraform destroy
    ```

