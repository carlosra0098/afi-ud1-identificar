# **Lista de comprobación para escena digital**

### **BLOQUE 1: AL LLEGAR — Antes de tocar nada**

1. ¿Realmente hay un incidente? Verifica que los hechos que justifican tu presencia encajan con un incidente de seguridad. No asumir: confirmarlo con quien ha llamado. ENFSI 8.2 (preservación inicial y acciones de control).
2. Registrar quién ha estado antes de mi. Anotar nombre, hora y motivo de toda persona que haya accedido a la escena antes de mi llegada. ENFSI 9.1 (evaluar la escena y determinar requisitos).
3. Hacer un análisis de riesgos de la escena. ¿Hay riesgo eléctrico, de incendio, biológico, de agresión? ¿Puedo trabajar con seguridad? ENFSI 8.2 (preservación inicial y acciones de control).
4. Restringir el acceso. Acordonar o limitar físicamente quién puede entrar y salir. El objetivo es que nada cambie mientras trabajo. ENFSI 8.2 (preservación inicial y acciones de control).
5. Documentar la integridad inicial. Fotografiar pantallas, cables conectados, luces encendidas, estado del equipo antes de cualquier manipulación. ENFSI 9.2 (preparativos para inspeccionar la escena).

### **BLOQUE 2: ANTES DE TOCAR NADA — Evaluación estratégica**

1. Pregunta: ¿debería estar yo aquí, o hay otra disciplina forense que deba actuar primero? Huellas, ADN, balística u otra evidencia física pueden condicionar mi entrada o secuencia. ENFSI 8.2 (identificar otras disciplinas antes de tocar nada).
2. ¿Qué fuentes de datos potenciales hay más allá del equipo que tengo delante? Un router, un switch, un punto de acceso inalámbrico, un teléfono móvil, una impresora en red. La evidencia no está solo en el PC. NIST SP 800-86 3.1.1 (identificación de fuentes de datos).
3. ¿Hay servicios remotos o en la nube implicados? Correo, almacenamiento, registros de proveedores. La escena digital incluye servidores que no están físicamente presentes. NIST SP 800-86 3.1.1 (identificación de fuentes de datos).
4. Formular el mandato. ¿Qué me piden exactamente? Buscar qué tipo de evidencia, para qué delito o incidente. Determina el alcance antes de recoger. ENFSI 9.1 (determinar requisitos de la investigación).
5. Decidir: ¿sistema encendido o apagado? Si está encendido y hay datos volátiles críticos (memoria, conexiones activas, cifrado en curso), no apagarlo. Si está apagado, no encenderlo sin justificación. RFC 3227 2.1 (no apagar hasta completar la recogida; no confiar en programas del sistema).
6. ¿Hay mecanismos de autodestrucción? Si sospecho que desconectar la red puede activar un borrado remoto o cifrado, documentar el estado antes de actuar. RFC 3227 2.3 (remove external avenues for change — deadman switches).

### **BLOQUE 3: DECIDIR QUÉ SE ADQUIERE Y EN QUÉ ORDEN**

1. Aplicar el orden de volatilidad estricto. De lo que desaparece en segundos a lo que persiste: registros y caché → memoria RAM y tablas de conexiones → sistemas de archivos temporales → datos de registro remoto y monitorización → configuración de red y topología → medios de almacenamiento. RFC 3227 2.1 (orden de volatilidad).
2. Priorizar también por relevancia potencial y admisibilidad. Si dos fuentes tienen volatilidad similar, ¿cuál tiene más valor probatorio? ¿Cuál es más admisible? NIST SP 800-86 3.1.2 (adquisición de datos).
3. Ejecutar las herramientas desde medios protegidos, no desde el sistema investigado. No confiar en los programas del equipo sospechoso: pueden haber sido alterados. RFC 3227 2.1 (orden de volatilidad).
4. No ejecutar programas que modifiquen fechas de acceso. tar, xcopy y similares alteran metadatos. Usar herramientas forenses. RFC 3227 2.1 (orden de volatilidad).
5. Documentar cada acción, cada herramienta y cada decisión. Si se modifica algo (aunque sea mínimo), quedará registrado. RFC 3227 3 (procedimiento de recogida) ; NIST SP 800-86 3.1
6. Si hay sistemas que no se pueden parar (producción crítica, servicios en vivo), obtener los datos volátiles y, si es necesario, solicitar los logs al administrador. NIST SP 800-86 3.1.3 (consideraciones de respuesta a incidentes).
7. Antes de irme: ¿me dejo alguna fuente atrás? Repasar la lista de dispositivos, servicios remotos, registros de proveedores y cualquier otro lugar donde pueda haber evidencia. NIST SP 800-86 3.1.1 (identificación de fuentes de datos).