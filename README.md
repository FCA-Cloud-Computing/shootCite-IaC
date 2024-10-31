
# Proyecto Terraform: Infraestructura como Código

Este proyecto utiliza **Terraform** para gestionar y aprovisionar infraestructura de forma automatizada. Se compone de tres archivos principales: `main.tf`, `variables.tf` y `output.tf`, donde se definen los recursos, las variables de configuración, y los outputs relevantes del despliegue.

## Estructura del Proyecto

- **`main.tf`**: Define los recursos y proveedores de infraestructura.  
- **`variables.tf`**: Declara las variables usadas para parametrizar el despliegue.  
- **`output.tf`**: Define las salidas (outputs) importantes que se mostrarán al finalizar el despliegue.

---

## Requisitos

- **Terraform** >= 1.0  
- Proveedor cloud configurado (por ejemplo: AWS, Azure, GCP).  
- Acceso a credenciales válidas en tu entorno.  

---

## Instalación

1. **Clonar el repositorio**  
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   cd <NOMBRE_DEL_PROYECTO>
   ```

2. **Inicializar Terraform**  
   Ejecuta este comando para inicializar los proveedores necesarios:  
   ```bash
   terraform init
   ```

---

## Uso

1. **Planificar el despliegue**  
   Revisa los cambios que Terraform aplicará con:  
   ```bash
   terraform plan
   ```

2. **Aplicar la configuración**  
   Para desplegar los recursos, usa:  
   ```bash
   terraform apply
   ```

3. **Ver los outputs**  
   Una vez completado el despliegue, puedes revisar las salidas con:  
   ```bash
   terraform output
   ```

4. **Destruir la infraestructura**  
   Si necesitas eliminar todos los recursos:  
   ```bash
   terraform destroy
   ```

---

## Variables

Define tus variables en el archivo `variables.tf`. Aquí tienes un ejemplo de cómo pasar valores mediante la línea de comandos:  
```bash
terraform apply -var="nombre_variable=valor"
```

También puedes usar un archivo `terraform.tfvars` para definir las variables por defecto.

---

## Contribuciones

1. Realiza un **fork** del proyecto.
2. Crea una nueva **rama** para tus cambios:  
   ```bash
   git checkout -b feature/nueva-funcionalidad
   ```
3. Haz un **commit** con tus cambios y súbelos:  
   ```bash
   git commit -m "Agrega nueva funcionalidad"
   git push origin feature/nueva-funcionalidad
   ```
4. Abre un **pull request**.

---

## Licencia

Este proyecto está disponible bajo la licencia [MIT](https://opensource.org/licenses/MIT). 

---

## Contacto

Si tienes alguna duda o sugerencia, no dudes en abrir un **issue** o contactarme directamente.
