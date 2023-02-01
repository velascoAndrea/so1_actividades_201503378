## Tipos de Kernel y sus Diferencias
- Kernel monolítico: Un kernel grande para todas las tareas. Es el único responsable de la gestión de la memoria y de los procesos, de la comunicación entre procesos y proporciona funciones de soporte de drivers y hardware. Los sistemas operativos que usan el kernel monolítico son Linux, OS X y Windows.
- Microkernel: El microkernel se ha diseñado intencionadamente de un tamaño pequeño para que en caso de fallo no paralice todo el sistema operativo. No obstante, para que pueda asumir las mismas funciones que un kernel grande, está dividido en varios módulos. Como ejemplo de aplicación solo existe el componente Mach de OS X, ya que hasta ahora no hay ningún sistema operativo con microkernel.
- Kernel híbrido: La combinación del kernel monolítico y el microkernel se denomina kernel híbrido. En este caso, el kernel grande se hace más compacto y modulable. Otras partes del kernel pueden cargar dinámicamente. Esto ya ocurre en cierta medida en Linux y OS X.

Las diferencias radican en cómo se dividen y organizan las funciones del kernel. Los monolíticos son más eficientes, pero menos flexibles y escalables. Los microkernels son más flexibles y escalables, pero pueden ser menos eficientes debido a la necesidad de delegar tareas a componentes externos. Los híbridos buscan equilibrar ambos aspectos. La elección del tipo de kernel adecuado dependerá de los requisitos específicos de un sistema operativo en particular.

## User vs Kernel Mode
El modo de usuario y el modo de kernel son dos modos de operación diferentes de un sistema operativo.

- Modo de usuario: en este modo, el procesador ejecuta aplicaciones y programas que son accesibles para el usuario. El modo de usuario no tiene acceso directo a los recursos del sistema, como la memoria y los dispositivos de entrada/salida.
  
- Modo de kernel: en este modo, el procesador tiene acceso total a los recursos del sistema. El modo de kernel se utiliza para realizar tareas críticas para el funcionamiento del sistema, como gestionar memoria y manejar interrupciones de dispositivos.


La diferencia fundamental es el nivel de acceso que tienen los procesos a los recursos del sistema. El modo de usuario es más limitado para prevenir errores o fallos en el sistema, mientras que el modo de kernel tiene control total sobre el sistema. La transición entre modos se realiza mediante interrupciones o llamadas al sistema.
