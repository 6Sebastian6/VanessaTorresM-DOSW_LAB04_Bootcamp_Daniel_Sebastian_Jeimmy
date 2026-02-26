# DOSW-Lab4
# planeacion
___
## Desglose de trabajo: Epica, Historias  de Usuario y Tareas
___
## 1.Epica
| Campo        | Descripcion                                                                                                      |
|--------------|------------------------------------------------------------------------------------------------------------------|
| ID           | EP-01                                                                                                            |
| Titulo       | Deposito                                                                                                         |
| Descripcion  | Para que los usuarios realizar depositos de dinero en distintas cuentas y tener un comprobante de la transaccion |
| Stalkeholder | Gerente de Operaciones y Cliente o Usuario                                                                       |

### 2.Historias de usuario
| Campo      | Descripcion                     |
|------------|---------------------------------|
| ID         | HU-01                           |
| Titulo     | Autenticar usuario              |
| Prioridad  | Alta                            |
| Estimacion | Se define en el Planning Poker  |

| Campo      | Descripcion                     |
|------------|---------------------------------|
| ID         | HU-02                           |
| Titulo     | Validar datos de la transaccion |
| Prioridad  | Media                           |
| Estimacion | Se define en el Planning Poker  |

| Campo      | Descripcion                     |
|------------|---------------------------------|
| ID         | HU-03                           |
| Titulo     | Realizar el movimiento          |
| Prioridad  | Alta                            |
| Estimacion | Se define en el Planning Poker  |

| Campo      | Descripcion                     |
|------------|---------------------------------|
| ID         | HU-04                           |
| Titulo     | Registrar movimiento            |
| Prioridad  | Media                           |
| Estimacion | Se define en el Planning Poker  |


### 3.Tareas
| Campo                             | Descripcion                                                                    |
|-----------------------------------|--------------------------------------------------------------------------------|
| ID                                | TR-01                                                                          |
| Titulo                            | Iniciar sesión en el sistema                                                   |
| ID de la Historia de Uso asociada | HU-01                                                                          |
| Descripcion                       | Implementar el login para que el usuario pueda ingresar para hacer el deposito | 
| Tareas requisito                  | Niguna                                                                         | 

| Campo                             | Descripcion                                                                                    |
|-----------------------------------|------------------------------------------------------------------------------------------------|
| ID                                | TR-02                                                                                          |
| Titulo                            | Ir al deposito                                                                                 |
| ID de la Historia de Uso asociada | HU-02                                                                                          |
| Descripcion                       | Agregar la funcion para permitir que el usuario pueda ir a la pantalla de realizar el deposito | 
| Tareas requisito                  | TR-01                                                                                          | 

| Campo                             | Descripcion                                                                                       |
|-----------------------------------|---------------------------------------------------------------------------------------------------|
| ID                                | TR-03                                                                                             |
| Titulo                            | Diligenciar datos de transaccion                                                                  |
| ID de la Historia de Uso asociada | HU-01                                                                                             |
| Descripcion                       | Crear la pantalla para que el  usuario ponga el numero de la cuenta al que va a enviar y el monto | 
| Tareas requisito                  | TR-02                                                                                             | 

| Campo                             | Descripcion                                                                                            |
|-----------------------------------|--------------------------------------------------------------------------------------------------------|
| ID                                | TR-04                                                                                                  |
| Titulo                            | Validar que existe la cuenta de destino                                                                |
| ID de la Historia de Uso asociada | HU-02                                                                                                  |
| Descripcion                       | Verificar que la cuenta a la que se le enviara el dinero exista y este activa antes de enviar el monto | 
| Tareas requisito                  | TR-03                                                                                                  | 

| Campo                             | Descripcion                                                                                                          |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------|
| ID                                | TR-05                                                                                                                |
| Titulo                            | Validar monto                                                                                                        |
| ID de la Historia de Uso asociada | HU-02                                                                                                                |
| Descripcion                       | Ver que el monto sea un numero positivo y que no sea mayor a la cantidad de dinero que tenga el usuario en la cuenta | 
| Tareas requisito                  | TR-04                                                                                                                | 

| Campo                             | Descripcion                                                                           |
|-----------------------------------|---------------------------------------------------------------------------------------|
| ID                                | TR-06                                                                                 |
| Titulo                            | Mostrar mensaje de error                                                              |
| ID de la Historia de Uso asociada | HU-02                                                                                 |
| Descripcion                       | Crear un mensaje que muestre al usuario cualquier error que pueda pasar en el proceso | 
| Tareas requisito                  | TR-03,TR-04,TR-05                                                                     | 

| Campo                             | Descripcion                                                                                       |
|-----------------------------------|---------------------------------------------------------------------------------------------------|
| ID                                | TR-07                                                                                             |
| Titulo                            | Ejecutar transaccion                                                                              |
| ID de la Historia de Uso asociada | HU-03                                                                                             |
| Descripcion                       | Crear la logica para que se realize el proceso de realizar la transaccion desde una cuenta a otra | 
| Tareas requisito                  | TR-04,TR-05                                                                                       | 

| Campo                             | Descripcion                                                                                                                          |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|
| ID                                | TR-08                                                                                                                                |
| Titulo                            | Integridad de la transaccion                                                                                                         |
| ID de la Historia de Uso asociada | HU-03                                                                                                                                |
| Descripcion                       | Asegurarse de que si falla no se realize ningun cambio en las cuentas o que se revierta cualquier cambio para mantener la integridad | 
| Tareas requisito                  | TR-07                                                                                                                                | 

| Campo                             | Descripcion                                                                 |
|-----------------------------------|-----------------------------------------------------------------------------|
| ID                                | TR-09                                                                       |
| Titulo                            | Registrar movimiento                                                        |
| ID de la Historia de Uso asociada | HU-03                                                                       |
| Descripcion                       | Crear un registro, como un historial del movimiento con informacion de esta | 
| Tareas requisito                  | TR-07                                                                       | 

| Campo                             | Descripcion                                                                              |
|-----------------------------------|------------------------------------------------------------------------------------------|
| ID                                | TR-10                                                                                    |
| Titulo                            | Crear comprobante                                                                        |
| ID de la Historia de Uso asociada | HU-04                                                                                    |
| Descripcion                       | Crear un formato que tenga los datos de la transaccion y esta se le entregara al usuario | 
| Tareas requisito                  | TR-09                                                                                    | 

| Campo                             | Descripcion                                                               |
|-----------------------------------|---------------------------------------------------------------------------|
| ID                                | TR-11                                                                     |
| Titulo                            | Obtener datos del comprobante                                             |
| ID de la Historia de Uso asociada | HU-04                                                                     |
| Descripcion                       | Con el movimiento se obtendra la informacion que estara en el comprobante | 
| Tareas requisito                  | TR-10                                                                     | 

| Campo                             | Descripcion                                                                                                  |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------|
| ID                                | TR-12                                                                                                        |
| Titulo                            | Generar y descargar comprobante                                                                              |
| ID de la Historia de Uso asociada | HU-04                                                                                                        |
| Descripcion                       | Crear la logica para que el usuario pueda generar y descargar el comprobante, cuando se finalize el deposito | 
| Tareas requisito                  | TR-10,TR-09                                                                                                  | 
