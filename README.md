Integrantes del Equipo
Rafael Cano Pérez — A01804697
Jordan Adrián Bustamante Luna — A01805057

1- Definición del Proyecto
El objetivo central es desarrollar un dispositivo de monitoreo médico portable de bajo costo, pensado para adultos mayores y personas vulnerables que viven solas o pasan largos periodos sin supervisión continua.

Para asegurar la viabilidad del prototipo, el sistema opera bajo una idea fundamental la cual refiere a una automatización en la que no sea necesaria la intervención humana. El paciente únicamente porta el accesorio y este realiza lecturas continuas, transmitiendo los datos a la nube y alertando a sus familiares ante cualquier anomalía.

2- Ubicación del Dispositivo en el Cuerpo
Se seleccionó la cara anterior de la muñeca (formato reloj) por las siguientes razones:
  1. Aceptación y costumbre: Los adultos mayores están familiarizados con relojes; colocarlo evita que se lo retiren al dormir.
  2. Contacto con la piel: Ofrece contacto firme, indispensable para el sensor térmico y óptico.
  3. Punto Estratégico para Caídas: La ubicación del mismo nos permite tener un buen desempeño de este en el análisis del impacto.

3- Variables Biomédicas Seleccionadas
  1. Saturación de Oxígeno en Sangre: Para detectar fallas respiratorias o hipoxia silenciosa.
  2. Frecuencia Cardíaca (Pulso): Latidos por minuto para supervisar taquicardias o reposo anormal.
  3. Temperatura Corporal:Grados Celsius mediante contacto físico para alertar cuadros febriles o hipotermia.
  4. Variable Extra (Detección de Caídas): Control de impactos.

4. Diagrama de Arquitectura del Sistema
Capa 1 (Percepción): Microcontrolador ESP-32 DevKit V1, Sensor MAX30102, Sensor MPU6050 (Caídas) y Sensor DS18B20 (Temperatura)
Capa 2 (Red y Comunicación): Conexión WiFi doméstica estándar y protocolo MQTT para enviar mensajes.
Capa 3 (Procesamiento y Almacenamiento): Broker MQTT y Base de Datos relacional MySQL para organizar las lecturas cronológicamente.
Capa 4 (Visualización): Módulo de notificaciones de emergencia mediante un Bot de Telegram.
Capa 5 (Negocio e Impacto Social): Garantizar tranquilidad familiar con un costo de prototipo menor a $600 MXN, alineado al ODS 3 y ODS 10.
