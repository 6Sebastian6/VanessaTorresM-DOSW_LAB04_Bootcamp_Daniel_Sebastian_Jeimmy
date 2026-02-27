# DOSW-Lab4
# planeacion
___
## Desglose de trabajo: Epica, Historias  de Usuario y Tareas
___
## 1.Epica
| Campo        | Descripción                                                                                                      |
|--------------|------------------------------------------------------------------------------------------------------------------|
| ID           | EP-01                                                                                                            |
| Título       | Deposito                                                                                                         |
| Descripción  | Para que los usuarios realicen depositos de dinero en distintas cuentas y tener un comprobante de la transacción |
| Stalkeholder | Gerente de Operaciones y Cliente o Usuario                                                                       |

### 2.Historias de usuario
| Campo      | Descripción                     |
|------------|---------------------------------|
| ID         | HU-01                           |
| Título     | Autenticar usuario              |
| Prioridad  | Alta                            |
| Estimación | Se define en el Planning Poker  |

| Campo      | Descripción                     |
|------------|---------------------------------|
| ID         | HU-02                           |
| Título     | Validar datos de la transacción |
| Prioridad  | Media                           |
| Estimación | Se define en el Planning Poker  |

| Campo      | Descripción                     |
|------------|---------------------------------|
| ID         | HU-03                           |
| Título     | Realizar el movimiento          |
| Prioridad  | Alta                            |
| Estimación | Se define en el Planning Poker  |

| Campo      | Descripción                     |
|------------|---------------------------------|
| ID         | HU-04                           |
| Título     | Registrar movimiento            |
| Prioridad  | Media                           |
| Estimación | Se define en el Planning Poker  |


### 3.Tareas
| Campo                             | Descripción                                                                    |
|-----------------------------------|--------------------------------------------------------------------------------|
| ID                                | TR-01                                                                          |
| Título                            | Iniciar sesión en el sistema                                                   |
| ID de la Historia de Uso asociada | HU-01                                                                          |
| Descripción                       | Implementar el login para que el usuario pueda ingresar  hacer el deposito | 
| Tareas requisito                  | Niguna                                                                         | 

| Campo                             | Descripción                                                                                    |
|-----------------------------------|------------------------------------------------------------------------------------------------|
| ID                                | TR-02                                                                                          |
| Titulo                            | Ir al deposito                                                                                 |
| ID de la Historia de Uso asociada | HU-02                                                                                          |
| Descripción                       | Agregar la función que permitir al usuario  ir a la pantalla donde se realiza el deposito | 
| Tareas requisito                  | TR-01                                                                                          | 

| Campo                             | Descripción                                                                                       |
|-----------------------------------|---------------------------------------------------------------------------------------------------|
| ID                                | TR-03                                                                                             |
| Título                            | Diligenciar datos de transacción                                                                  |
| ID de la Historia de Uso asociada | HU-01                                                                                             |
| Descripción                       | Crear la pantalla en la cual  el  usuario escribe el numero de la cuenta al que va a enviar la transacción y su respectivo monto.  | 
| Tareas requisito                  | TR-02                                                                                             | 

| Campo                             | Descripción                                                                                            |
|-----------------------------------|--------------------------------------------------------------------------------------------------------|
| ID                                | TR-04                                                                                                  |
| Título                            | Validar que existe la cuenta de destino                                                                |
| ID de la Historia de Uso asociada | HU-02                                                                                                  |
| Descripción                       | Verificar que la cuenta a la que se le enviará el dinero exista y este activa antes de enviar el monto | 
| Tareas requisito                  | TR-03                                                                                                  | 

| Campo                             | Descripción                                                                                                          |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------|
| ID                                | TR-05                                                                                                                |
| Título                            | Validar monto                                                                                                        |
| ID de la Historia de Uso asociada | HU-02                                                                                                                |
| Descripción                       | Asegurar que el monto sea un número positivo y que no sea mayor a la cantidad de dinero que tenga el usuario en la cuenta | 
| Tareas requisito                  | TR-04                                                                                                                | 

| Campo                             | Descripción                                                                           |
|-----------------------------------|---------------------------------------------------------------------------------------|
| ID                                | TR-06                                                                                 |
| Título                            | Mostrar mensaje de error                                                              |
| ID de la Historia de Uso asociada | HU-02                                                                                 |
| Descripción                       | Crear un mensaje que muestre al usuario cualquier error que pueda pasar en el proceso | 
| Tareas requisito                  | TR-03,TR-04,TR-05                                                                     | 

| Campo                             | Descripción                                                                                       |
|-----------------------------------|---------------------------------------------------------------------------------------------------|
| ID                                | TR-07                                                                                             |
| Título                            | Ejecutar transacción                                                                              |
| ID de la Historia de Uso asociada | HU-03                                                                                             |
| Descripción                       | Crear la lógica en la cual se realiza el proceso de transaccion entre cuentas, asegurandose la integridad de los datos. | 
| Tareas requisito                  | TR-04,TR-05                                                                                       | 

| Campo                             | Descripción                                                                                                                          |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|
| ID                                | TR-08                                                                                                                                |
| Título                            | Integridad de la transacción                                                                                                         |
| ID de la Historia de Uso asociada | HU-03                                                                                                                                |
| Descripción                       | Asegurar que, en caso de que la transacción falle, no se realice ningún cambio en las cuentas y se garantice su integridad. | 
| Tareas requisito                  | TR-07                                                                                                                                | 

| Campo                             | Descripcion                                                                 |
|-----------------------------------|-----------------------------------------------------------------------------|
| ID                                | TR-09                                                                       |
| Título                            | Registrar movimiento                                                        |
| ID de la Historia de Uso asociada | HU-03                                                                       |
| Descripción                       | Crear un registro en el historial de transacciones, específicamente para este movimiento.| 
| Tareas requisito                  | TR-07                                                                       | 

| Campo                             | Descripcion                                                                              |
|-----------------------------------|------------------------------------------------------------------------------------------|
| ID                                | TR-10                                                                                    |
| Título                            | Crear comprobante                                                                        |
| ID de la Historia de Uso asociada | HU-04                                                                                    |
| Descripción                       | Crear un formato que tenga los datos de la transacción y esta se le entregará al usuario | 
| Tareas requisito                  | TR-09                                                                                    | 

| Campo                             | Descripcion                                                               |
|-----------------------------------|---------------------------------------------------------------------------|
| ID                                | TR-11                                                                     |
| Título                            | Obtener datos del comprobante                                             |
| ID de la Historia de Uso asociada | HU-04                                                                     |
| Descripción                       | Con el movimiento se obtendrá la información que estará en el comprobante | 
| Tareas requisito                  | TR-10                                                                     | 

| Campo                             | Descripcion                                                                                                  |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------|
| ID                                | TR-12                                                                                                        |
| Título                            | Generar y descargar comprobante                                                                              |
| ID de la Historia de Uso asociada | HU-04                                                                                                        |
| Descripción                       | Crear la lógica que permite al usuario generar y descargar el comprobante, cuando se finalice el deposito. | 
| Tareas requisito                  | TR-10,TR-09                                                                                                  | 
