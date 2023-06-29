# Manu-CNC
Programación para cnc (ejercicios de clase)
% O0001 
(Declarar variables)
#10 = 0 (Número de herramienta actual)
#20 = 1 (Número de herramienta deseado)

(Movimiento a la posición de cambio de herramienta)
G53 G0 Z0 (Mover a la posición segura)
G53 G0 X0 Y0 (Mover a la posición de cambio de herramienta)

(Cambio de herramienta)
M06 T#20 (Cargar la herramienta deseada)
#10 = #20 (Actualizar el número de herramienta actual)

(Volver a la posición segura)
G53 G0 Z0 (Mover a la posición segura)

(Fin del programa)
M30
%
