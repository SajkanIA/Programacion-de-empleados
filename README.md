# Programacion-de-empleados


Documentación del Proyecto
Clase Departamento
La clase Departamento se utiliza para crear departamentos con nombre y habilidades requeridas. Cada departamento puede tener un nombre y una lista de habilidades requeridas.

Métodos:

__init__(self, nombre, habilidades_requeridas): El constructor de la clase que recibe el nombre del departamento y las habilidades requeridas.
cambia_nombre(self, nuevo_nombre): Cambia el nombre del departamento.
cambia_habilidades(self, nueva_habilidad): Cambia las habilidades requeridas del departamento.
ver_habilidades(self): Devuelve la lista de habilidades requeridas.
ver_nombre(self): Devuelve el nombre del departamento.
Clase Turno
La clase Turno se utiliza para crear turnos de trabajo. Cada turno de trabajo tiene un empleado asignado, un horario de inicio y finalización, un departamento al que pertenece y los días en los que está disponible.

Métodos:

__init__(self, inicio_del_turno, final_del_turno, departamento, dias, empleado=None): El constructor de la clase que recibe el horario de inicio, el horario de finalización, el departamento al que pertenece, los días en los que está disponible y un empleado opcional.
cambio_de_empleado(self, nuevo_empleado): Cambia el empleado asignado al turno.
ver_empleado(self): Devuelve el empleado asignado al turno.
ver_inicio_del_turno(self): Devuelve el horario de inicio del turno.
ver_final_del_turno(self): Devuelve el horario de finalización del turno.
ver_departamento(self): Devuelve el departamento al que pertenece el turno.
ver_dias(self): Devuelve los días en los que está disponible el turno.
Funciones de creación de departamentos y turnos
agregar_dep(nombre, habilidades_requeridas): Crea un objeto que referencia un departamento.
crea_dep(): Crea los departamentos que se utilizarán y devuelve una lista de objetos Departamento.
crea_turno(departamentos): Crea los turnos de trabajo para los departamentos especificados y devuelve una lista de objetos Turno.
Clase Empleados
La clase Empleados se utiliza para crear empleados con nombre, habilidades, hora de inicio, hora de salida y disponibilidad. Cada empleado puede tener un nombre, habilidades, horario de inicio, horario de salida y disponibilidad.

Métodos:

__init__(self, nombre, habilidades, hora_de_inicio, hora_de_salida, disponibilidad): El constructor de la clase que recibe el nombre del empleado, habilidades, horario de inicio, horario de salida y disponibilidad.
cambia_cualidades(self, nombre=None, habilidades=None, disponibilidad=None): Cambia las cualidades del empleado, incluyendo nombre, habilidades y disponibilidad.
ver_nombre(self): Devuelve el nombre del empleado.
ver_habilidades(self): Devuelve las habilidades del empleado.
ver_hora_de_inicio(self): Devuelve la hora de inicio del empleado.
ver_hora_de_salida(self): Devuelve la hora de salida del empleado.
ver_disponibilidad(self): Devuelve la disponibilidad del empleado.
Función de creación de empleados
crear_empleados(): Crea una lista de objetos Empleados con información proporcionada por el usuario.
Función de asignación de turnos a empleados
backtrack(turnos, empleados): Busca una solución al problema de asignar turnos a empleados utilizando recursión.
Función de restricciones para la asignación de turnos
solo_puede_cubrir_un_turno_al_día(turnos): Verifica si un empleado solo puede cubrir un turno al día.
hab_persona_vs_hab_dep(hab_persona, hab_departamento): Compara las habilidades de una persona con las habilidades requeridas por un departamento.
respeta_disponibilidad(dips_emp, dip_tur): Verifica si un empleado respeta la disponibilidad de horario de un turno.
Algoritmo AC-3
AC3(): Implementa el algoritmo de consistencia arc3 (AC-3) para resolver el problema de asignación de turnos a empleados.
Es importante tener en cuenta que este es un esqueleto de código y puede requerir más desarrollo y ajustes para funcionar correctamente según los requisitos específicos del proyecto. El código proporcionado aquí se centra en la estructura de las clases y funciones para abordar el problema de asignación de turnos a empleados.
