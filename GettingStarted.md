# ¿Que hace ProcessaLoadFiles?
ProcessaLoadFiles se encarga de realizar el cargue de diferentes archivos sin estructura para realizar un proceso especifico determinado por la necesidad del cliente.

# ¿Que contiene la primera version de ProcessaLoadFiles?
La primera versión del módulo contiene funciones para el cargue de archivos que contengan numeros de bonos sin estructura especifica, para su posterior Activación, Bloqueo o Cancelación y notificacion por correo electronico sobre el proceso.  

## Funciones

| Fuinción  | Descripción  |
|:---|---|
| [Find-BonusLog](Scripting/Find-BonusLog.md)  | Encuentra la ruta completa del log enviado al cliente por un numero de bono especifico. |
| [Get-AdminLog](Scripting/Get-AdminLog)  | Obtiene y muestra el log del administrador por rango de fechas y un posible processId |
| [Get-Configuration](Scripting/GetConfig)  | Obtiene la configuracion del modulo. |
| [Get-ValuePattern](Scripting/RemoveConfig)  | Obtiene informacion del archivo indicado segun la expresion regular indicada. |
| [Invoke-BonusActivation](Scripting/InvokeReport)  | Realiza el proceso de cargue y activacion de los bonos enviados en el archivo indicado. |
| [Invoke-BonusCancellation](Scripting/InvokeReport)  | Realiza el proceso de cargue y cancelacion de los bonos enviados en el archivo indicado. |
| [Invoke-BonusLock](Scripting/InvokeReport)  | Realiza el proceso de cargue y bloqueo de los bonos enviados en el archivo indicado. |
| [Set-Configuration](Scripting/InvokeReport)  | Realiza la configuracion necesaria para el funcionamiento del modulo. |
| [Test-Configuration](Scripting/InvokeReport)  | Valida que la configuracion del modulo se encuentre correcta. |

# ¿ Como instalar el modulo ?
Abra una ventana de Powershell (En su preferencia como Administrador) y ejecute el siguiente comando.
```PowerShell
Install-Module -Name ProcessaLoadFiles -Repository (Nombre del Repositorio creado en su Ambiente)
```
**Nota:**
En caso de aparecer una ventana de confirmacion aceptar que el modulo se instale.

# ¿ Como utilizar el modulo ?
## Importar el modulo
Abra una ventana de Powershell y ejecute el siguiente comando.
```PowerShell
Import-Module -Name ProcessaLoadFiles 
```
En caso de tener cargado el modulo en Powershell pero desear importarlo utilice el parametro -Force (Este es un parametro Switch).
Una vez cargado el modulo lo recomendable es utilizar el siguiente comando.
```PowerShell
Get-Configuration
```
Con esto podremos ver toda la configuracion del modulo. mas informacion en el enlace del cuadro de funciones.

## Configurar el modulo
Ejecute el siguiente comando para realizar la configuracion del modulo.
```PowerShell
Set-Configuration
```
Esta funcion abrira un cuadro de dialogo en el cual debe ingresar los valores solicitados para la configuracion, una vez de click en el boton Aceptar la configuracion se validara e indicara si fue posible guardarla o no.  mas informacion en el enlace del cuadro de funciones.

## Validar la configuracion del modulo
Ejecute el siguiente comando para validar la configuracion
```PowerShell
Test-Configuration
```
Con esto se indicara si la configuracion se encuentra correcta o presenta algun error.  mas informacion en el enlace del cuadro de funciones.

## Finalizando 
Con la configuracion establecida y validada puede utilizar las demas funciones indicadas en el cuadro de funciones.
