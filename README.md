# Sistema de Verificación de Ingreso - Condominio "Las Flores del Maizal"

Este proyecto fue desarrollado como parte del curso de **Fundamentos de Programación**. Su objetivo es digitalizar y automatizar el control de ingreso de personas y vehículos en el condominio "Las Flores del Maizal", reemplazando los registros manuales tradicionales por un sistema funcional en Python.
Actualmente, el control de ingreso al condominio “Las Flores del Maizal” se realiza de manera manual, lo cual genera múltiples problemas relacionados con la seguridad, la eficiencia operativa y la trazabilidad de la información. Esta metodología expone al condominio a riesgos como el acceso no autorizado, pérdida de registros y demoras en los procesos de verificación. Además, el registro manual aumenta la carga de trabajo para el personal de seguridad, lo que puede afectar la precisión y consistencia en el registro de datos.
Este proyecto propone una solución innovadora mediante el desarrollo de un sistema automatizado utilizando el lenguaje de programación Python. El sistema permitirá registrar, validar y analizar el ingreso de personas y vehículos en tiempo real. Para ello, se emplearán estructuras de control como bucles, condicionales y estructuras secuenciales que darán forma a un algoritmo lógico y eficiente. 
El enfoque del proyecto también contempla la posibilidad de generar reportes detallados de los accesos registrados, lo que permitirá una mejor toma de decisiones administrativas en el condominio. La implementación de módulos adicionales para la gestión de datos históricos contribuirá a evaluar patrones de ingreso, identificando posibles riesgos y optimizando el manejo de información.
Complementariamente, se integrará una plataforma de gestión de tareas como Trello, permitiendo una organización clara del proyecto bajo metodologías ágiles. Esto facilitará la asignación de responsabilidades, el seguimiento de avances y la documentación del proceso. La solución busca no solo mejorar la seguridad del condominio, sino también optimizar el tiempo del personal de vigilancia y ofrecer reportes detallados que contribuyan a una mejor toma de decisiones.


## Objetivo General
Desarrollar un sistema automatizado de control de ingreso para el condominio “Las Flores del Maizal” utilizando el lenguaje de programación Python, con el fin de mejorar la seguridad, eficiencia y trazabilidad de los registros.

## Objetivos especificos
Implementar un módulo de ingreso automatizado utilizando Python.
Desarrollar interfaces gráficas intuitivas para el registro de personas y vehículos.
Integrar una base de datos segura para el almacenamiento y consulta de información.
Generar reportes periódicos de ingreso/salida para la administración del condominio.

## Situacion actual 

Actualmente, el proceso de control de ingreso en el condominio “Las flores del maizal”, se realiza de manera manual, ya sea mediante registros escritos en papel o a través de aplicaciones básicas (excel), sin integración ni control riguroso. Este método presenta varias limitaciones que afectan directamente la seguridad y eficiencia operativa del lugar:
- Falta de trazabilidad: No se tiene un registro digital fiable y consultable de quién ingresó, a qué hora, con qué vehículo y con qué propósito. 
Cuando el administrador del condominio quería recabar más información sobre la entrada de personas y vehículos se encontraba con que tenía que hacer un proceso manual más largo para obtener la información de solo una persona ingresante. 
- Errores humanos: Al depender del registro manual, es común que se cometan errores en la identificación de personas o en los horarios registrados.
En una audiencia que se hizo en el condominio, se vio que en los registros se habían cometido errores de escritura, las fechas no coinciden, y hubo una pérdida promedio del 22% de registros diarios de forma mensual.
- Ausencia de alertas o filtros de seguridad: No se detectan automáticamente visitas no autorizadas o personas que intenten ingresar de forma indebida.
Se ha tenido informe que desde el mes de Enero hasta el mes de Abril, hubo un total de 9 personas que ingresaron sin una autorización previa. Puesto que en las horas pico de la tarde se registró un total de 25 personas que ingresan al condominio 
- Tiempo de ingreso lento: El proceso de ingreso puede volverse lento en horas pico debido a la necesidad de verificar identidades de manera informal.
Se registró el tiempo de cuando se toman los datos de manera manual y este es de 3 minutos, lo cual parece poco, pero cuando son varias personas, más las actividades  por hacer, el uso de un programa agiliza más el procedimiento.   
Considerando que la seguridad y la trazabilidad de las visitas son factores fundamentales en la administración de un condominio, se hace evidente la necesidad de migrar hacia un sistema digital automatizado. Este nuevo enfoque debe permitir registrar de manera segura, eficiente y organizada el ingreso de residentes, visitantes y vehículos, incorporando mecanismos de control horario y validación de autorizaciones, con el fin de mejorar tanto la gestión como la protección del entorno residencial.

## Propuesta de innovación

Capítulo 2: Propuesta de innovación
a) Entradas 
Datos personales:
Nombre completo
Documento de identidad
Tipo de persona: propietario, visitante, trabajador, proveedor, etc.*
*(entrada opcional, por si no se encuentra registro.)
Datos del vehículo (si aplica):
Placa
Marca y modelo**
**(datos adicionales, opcional*)
Color**
**(datos adicionales, opcional*)
Motivo del ingreso:
Visita, trabajo, entrega, mantenimiento, etc.
Horario y fecha del ingreso
Registro de hora y fecha de ingreso a todo el que ingrese 
b) Procesos

Ingreso de datos por parte del personal seguridad:
A través del programa digitando manualmente el DNI y  placa del vehículo.
Verificación de identidad y validación del vehículo:
Si el DNI corresponde a una persona autorizada (“verificado mediante una base de datos internas del condominio”) se registra directamente el ingreso.
Si la persona no está registrada o no tiene autorización***, se notificará al personal de seguridad.
Registro del ingreso:
Una vez validado los datos, se registra el ingreso en la base de datos del condominio:
Nombre completo de la persona
DNI de la persona
Placa del vehículo
Hora del ingreso
Motivo del ingreso
Alerta:
Si la persona o vehículo no está autorizada se generará una alerta al personal de seguridad.
El ingreso será bloqueado hasta que se resuelva la situación (“requiere intervención de un responsable de seguridad”)
Actualización en tiempo real:
El registro del ingreso se actualizará en tiempo real en la base de datos accesibles por los administradores del condominio, permitiendo una consulta rápida y trazabilidad.
Salidas
Registro seguro y digital de ingreso con marca de tiempo
Historial de entradas consultable por persona, vehículo o fecha.
Reportes periódicos sobre el tráfico de ingreso/salida por hora, dia, tipo de ingreso (propietario, visitante, trabajador, etc.)


