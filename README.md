# Brain-Computer-Interface-Development
The objective of this repositorie is to build a Brain Computer Interface that sends EEG signals by Wi-Fi connection and save them in a Data Base

# Descripción
Proyecto enfocado en el desarrollo de una Interfaz Cerebro Computadora (BCI) para el Laboratorio de Procesamiento Digital de Señales en el Centro de Investigación en Computación del Instituto Politécnico Nacional (CIC-IPN). 

El dispositivo busca capturar 16 canales de EEG y enviarlos inalámbricamente mediante un ESP32 a una base de datos gestionada por un sitio Web propio del laboratorio para su posterior procesamiento mediante algoritmos de Procesamiento Digital de Señales y de Inteligencia Artificial para la clasificación en tareas de movimientos musculares (motor imagery).

# Protocolo
## Procedimiento
El procedimiento consiste en medir mediante electrodos la actividad eléctrica de la corteza cerebral. La señal es tan pequeña que debe ser amplificada y filtrada de manera analógica a través del componente electrónico de Texas Instruments; ADS1299. Este componente recoge por canal y de forma diferencial dos señales, dando como salida la resta entre ellas y su respectivo tratamiento analógico.

La colocación de los electrodos sobre el cuero cabelludo está sujeta a un sistema de estandarización internacional 10-20, el cuál fue llamado así por la separación porcentual entre los electrodos en puntos reconocibles del cráneo. Estos puntos clave, a partir de los que se toma la distancia son:
- Nasión identación entre frente y nariz.
- Inión; protuberancia occipital.
- Puntos preauriculares; frente del trago de cada pabellón de la oreja.

Sin embargo, por las facilidades y reducciones de tiempo y recursos que involucra estar midiendo constantemente estos puntos, se optó por utilizar un gorro de electroencefalografía de tamaño mediano de adulto. Éste gorro cuenta con 20 puntos de medición, de los cuáles usaremos 16 por la cantidad de electrodos que actualmente se cuentan. 

Los pasos a seguir para preparar la captura de EEG a un paciente son los siguientes:

1. El gorro se coloca directamente a la cabeza del paciente y se introduce cada electrodo dentro de los espacios del gorro.
2. Se cubre cada copa de oro del electrodo con una pasta que facilite la recepción de la señal a través del cuero cabelludo.
3. Del otro extremo de los electrodos se conecta a un adaptador que entrará a la tarjeta ADS1299.

## Tipos de montajes
Algunos conceptos clave que se deben saber son los siguientes:
- Electrodo: Elemento situado en el punto de registro y que conecta al dispositivo amplificador.
- Derivación: Los dos electrodos que son conectados a un canal del amplificador.
- Montaje: Conjunto de derivaciones, pueden ser monopolares o bipolares.
  - Montaje monopolar: Los electrodos exploradores ocupan la posición 1 del amplifiador mientras que la posición 2 se fija a un electrodo relativamente inactivo o común para todos los canales.
  - Montaje bipolar: Se toma la resta entre dos electrodos, pueden ser antero-posteriores (sagitales) o transversos (coronales).

# Desarrollo de la prueba
En este proyecto, el dispositivo está siendo desarrollado para aplicaciones de intención de movimiento o mejor conocido como motor imargery, en el cuál se evalúa la relación de señales electroencefalográficas con las contracciones musuclares.



# Horario de miembros del equipo
+ Lunes
  - Mari (13:00-16:00)
  - Alexis (14:00-19:00)
+ Martes
  - Mari (13:00-16:00)
  - Alexis (13:00-16:00)
+ Miércoles
  - Mari (10:00-16:00)
  - Alexis (15:00-19:00)
+ Jueves
  - Mari (13:00-16:00)
  - Alexis (13:00-16:00)
+ Viernes
  - Mari (11:00-16:00)
  - Alexis (12:00-17:00)
