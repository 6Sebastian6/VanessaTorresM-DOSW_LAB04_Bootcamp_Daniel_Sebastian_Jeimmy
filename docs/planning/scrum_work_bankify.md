# DOSW-Lab4
# planeación
___
## Desglose de trabajo: Epica, Historias  de Usuario y Tareas
___
## 1.Epica
| Campo        | Descripción                                                                                                      |
|--------------|------------------------------------------------------------------------------------------------------------------|
| ID           | DLBDSJ-1                                                                                                           |
| Título       | Deposito                                                                                                         |
| Descripción  | Para que los usuarios realicen depositos de dinero en distintas cuentas y tener un comprobante de la transacción |
| Stalkeholder | Gerente de Operaciones y Cliente o Usuario                                                                       |

### 2.Historias de usuario
| Campo      | Descripción                     |
|------------|---------------------------------|
| ID         | DLBDSJ-2                        |
| Título     | Autenticar usuario              |
| Prioridad  | Alta                            |
| Estimación | Se define en el Planning Poker  |

https://youtu.be/m8TP2ZEYkbg


| Campo      | Descripción                     |
|------------|---------------------------------|
| ID         | DLBDSJ-3                        |
| Título     | Validar datos de la transacción |
| Prioridad  | Media                           |
| Estimación | Se define en el Planning Poker  |

| Campo      | Descripción                     |
|------------|---------------------------------|
| ID         | DLBDSJ-4                        |
| Título     | Realizar el movimiento          |
| Prioridad  | Alta                            |
| Estimación | Se define en el Planning Poker  |

| Campo      | Descripción                     |
|------------|---------------------------------|
| ID         | DLBDSJ-5                        |  
| Título     | Registrar movimiento            |
| Prioridad  | Media                           |
| Estimación | Se define en el Planning Poker  |


### 3.Tareas
| Campo                             | Descripción                                                                    |
|-----------------------------------|--------------------------------------------------------------------------------|
| ID                                | DLBDSJ-6                                                                       |
| Título                            | Iniciar sesión en el sistema                                                   |
| ID de la Historia de Uso asociada | DLBDSJ-2                                                                          |
| Descripción                       | Implementar el login para que el usuario pueda ingresar  hacer el deposito | 
| Tareas requisito                  | Niguna                                                                         | 

| Campo                             | Descripción                                                                                    |
|-----------------------------------|------------------------------------------------------------------------------------------------|
| ID                                | DLBDSJ-7                                                                                       |
| Titulo                            | Ir al deposito                                                                                 |
| ID de la Historia de Uso asociada | DLBDSJ-3                                                                                          |
| Descripción                       | Agregar la función que permitir al usuario  ir a la pantalla donde se realiza el deposito | 
| Tareas requisito                  | DLBDSJ-6                                                                                          | 

| Campo                             | Descripción                                                                                       |
|-----------------------------------|---------------------------------------------------------------------------------------------------|
| ID                                | DLBDSJ-8                                                                                             |
| Título                            | Diligenciar datos de transacción                                                                  |
| ID de la Historia de Uso asociada | DLBDSJ-2                                                                                             |
| Descripción                       | Crear la pantalla en la cual  el  usuario escribe el numero de la cuenta al que va a enviar la transacción y su respectivo monto.  | 
| Tareas requisito                  | DLBDSJ-7                                                                                            | 

| Campo                             | Descripción                                                                                            |
|-----------------------------------|--------------------------------------------------------------------------------------------------------|
| ID                                | DLBDSJ-9                                                                                                  |
| Título                            | Validar que existe la cuenta de destino                                                                |
| ID de la Historia de Uso asociada | DLBDSJ-3                                                                                                  |
| Descripción                       | Verificar que la cuenta a la que se le enviará el dinero exista y este activa antes de enviar el monto | 
| Tareas requisito                  | DLBDSJ-8                                                                                                  | 

| Campo                             | Descripción                                                                                                          |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------|
| ID                                | DLBDSJ-10                                                                                                             |
| Título                            | Validar monto                                                                                                        |
| ID de la Historia de Uso asociada | DLBDSJ-3                                                                                                                |
| Descripción                       | Asegurar que el monto sea un número positivo y que no sea mayor a la cantidad de dinero que tenga el usuario en la cuenta | 
| Tareas requisito                  | DLBDSJ-9                                                                                                                | 

| Campo                             | Descripción                                                                           |
|-----------------------------------|---------------------------------------------------------------------------------------|
| ID                                | DLBDSJ-11                                                                               |
| Título                            | Mostrar mensaje de error                                                              |
| ID de la Historia de Uso asociada | DLBDSJ-3                                                                                 |
| Descripción                       | Crear un mensaje que muestre al usuario cualquier error que pueda pasar en el proceso | 
| Tareas requisito                  | DLBDSJ-8,DLBDSJ-9, DLBDSJ-10                                                                     | 

| Campo                             | Descripción                                                                                       |
|-----------------------------------|---------------------------------------------------------------------------------------------------|
| ID                                | DLBDSJ-12                                                                                             |
| Título                            | Ejecutar transacción                                                                              |
| ID de la Historia de Uso asociada | DLBDSJ-4                                                                                             |
| Descripción                       | Crear la lógica en la cual se realiza el proceso de transaccion entre cuentas, asegurandose la integridad de los datos. | 
| Tareas requisito                  | DLBDSJ-9,DLBDSJ-10                                                                                       | 

| Campo                             | Descripción                                                                                                                          |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|
| ID                                | DLBDSJ-13                                                                                                                                |
| Título                            | Integridad de la transacción                                                                                                         |
| ID de la Historia de Uso asociada | DLBDSJ-4                                                                                                                                |
| Descripción                       | Asegurar que, en caso de que la transacción falle, no se realice ningún cambio en las cuentas y se garantice su integridad. | 
| Tareas requisito                  | DLBDSJ-12                                                                                                                                | 

| Campo                             | Descripcion                                                                 |
|-----------------------------------|-----------------------------------------------------------------------------|
| ID                                | DLBDSJ-14                                                                       |
| Título                            | Registrar movimiento                                                        |
| ID de la Historia de Uso asociada | DLBDSJ-4                                                                       |
| Descripción                       | Crear un registro en el historial de transacciones, específicamente para este movimiento.| 
| Tareas requisito                  | DLBDSJ-12                                                                       | 

| Campo                             | Descripcion                                                                              |
|-----------------------------------|------------------------------------------------------------------------------------------|
| ID                                | DLBDSJ-15                                                                                    |
| Título                            | Crear comprobante                                                                        |
| ID de la Historia de Uso asociada | DLBDSJ-5                                                                                    |
| Descripción                       | Crear un formato que tenga los datos de la transacción y esta se le entregará al usuario | 
| Tareas requisito                  | DLBDSJ-14                                                                                    | 

| Campo                             | Descripcion                                                               |
|-----------------------------------|---------------------------------------------------------------------------|
| ID                                | DLBDSJ-16                                                                     |
| Título                            | Obtener datos del comprobante                                             |
| ID de la Historia de Uso asociada | DLBDSJ-5                                                                     |
| Descripción                       | Con el movimiento se obtendrá la información que estará en el comprobante | 
| Tareas requisito                  | DLBDSJ-15                                                                     | 

| Campo                             | Descripcion                                                                                                  |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------|
| ID                                | DLBDSJ-17                                                                                                        |
| Título                            | Generar y descargar comprobante                                                                              |
| ID de la Historia de Uso asociada | DLBDSJ-5                                                                                                        |
| Descripción                       | Crear la lógica que permite al usuario generar y descargar el comprobante, cuando se finalice el deposito. | 
| Tareas requisito                  | DLBDSJ-15,DLBDSJ-14                                                                                                  | 
