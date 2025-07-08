# comandos-CHKDSK
Cómo utilizar los comandos CHKDSK para analizar y reparar discos duros en Windows
Los problemas de disco duro en Windows pueden ser una experiencia, cuanto menos, desagradable. Afortunadamente, Windows dispone de herramientas integradas como CHKDSK que pueden ayudar a resolver los errores del disco duro con rapidez.

¿Qué es CHKDSK?
CHKDSK (Check Disk) es una utilidad de Windows diseñada para analizar y reparar los errores del sistema. Comprueba si el tamaño de un archivo, la ubicación y otra información del sistema coinciden con los datos que están realmente en el disco. CHKDSK también busca partes del disco duro que podrían dañar sus datos.

CHKDSK permite comprobar si hay errores en un disco duro en Windows 10 u 11. En concreto, el tipo de errores que se producen cuando los archivos no están donde se supone que deben estar. Los problemas en el disco duro son una de las razones por las que los PC funcionan con más lentitud con el paso del tiempo.

Si considera que el rendimiento de su equipo se está ralentizando, compruebe la duración de la batería. Asimismo, deshágase de las aplicaciones innecesarias del PC para que funcione más rápido, sin problemas y durante más tiempo.

¿Cuánto tarda CHKDSK?
CHKDSK puede tardar entre 20 minutos y varias horas en completarse, según la antigüedad y la capacidad del hardware. Mientras se ejecute CHKDSK, el equipo funcionará con lentitud. Si es posible, deje que el análisis CHKDSK finalice antes de reanudar otros procesos.

Si no se completa, pruebe a cancelar el análisis y a ejecutar CHKDSK de nuevo. Ahora bien, la imposibilidad de completarlo de forma repetida, significa que el problema puede ser grave. Si es así, es probable que tenga que seguir los pasos para reparar una unidad en Windows 10 o de la solución de problemas CHKDSK.

Comandos de CHKDSK
Puede seleccionar diferentes parámetros CHKDSK para identificar problemas concretos. El comando chkdsk buscará errores en la unidad de disco, pero no los reparará. Si los resultados le indican que no se requiere ninguna otra acción, no tendrá que utilizar ningún otro comando.

Este es un resumen de los comandos CHKDSK:

chkdsk compara los datos del directorio de archivos con los del sistema de archivos para verificar que coinciden. Es solo un diagnóstico y no intenta solucionar nada.

chkdsk /f repara cualquier problema estructural que surja con el sistema de archivos y el directorio de archivos, corrigiendo inconsistencias entre ambos.

chkdsk /r busca partes dañadas del disco duro físico (a la vez que se ejecuta chkdsk /f) e intenta recuperar los datos que contiene para trasladarlos a una parte del disco que no esté dañada.

chkdsk /x desmonta una unidad para que se pueda comprobar y reparar. Ejecutar este comando también ejecuta /f.

chkdsk /v muestra la ruta y el nombre de todos los archivos, a la vez que se ejecuta una comprobación.

Estos comandos se ejecutarán automáticamente en la unidad activa que se muestra junto al cursor. Para ejecutar CHKDSK en una unidad diferente, escriba chkdsk [letra de unidad]: /f, sustituyendo la [letra de unidad] por la letra de la unidad que quiera analizar. Por ejemplo, para reparar la unidad D, escriba chkdsk D: /f.

La unidad donde se aloja Windows (normalmente C) le pedirá que reinicie antes de que CHKDSK pueda ejecutarse. Para continuar, seleccione Y. Windows ejecutará CHKDSK justo después de reiniciarse.

![image](https://github.com/user-attachments/assets/2aa5126c-945f-42f5-9f7f-291aebe28844)
Imagen del símbolo del sistema con el comando adecuado para ejecutar CHKDSK en la unidad D. «chkdsk D: /f»

¿Qué hace chkdsk /r?
Chkdsk /r busca e intenta reparar las partes dañadas del disco duro. También ejecuta automáticamente chkdsk /f como parte de este proceso para corregir errores en el disco. Esto significa que no tendrá que ejecutar el comando chkdsk /f /r.

Chkdsk /r es uno de los comandos de CHKDSK más valiosos porque puede avisar de partes del disco duro que empiezan a funcionar mal. Puede servir como recordatorio para hacer copias de seguridad de los archivos importantes y no perderlos por un fallo del disco duro.

Antes de ejecutar chkdsk /r, es aconsejable hacer una copia de seguridad de los archivos importantes en otra unidad de almacenamiento, ya que podrían eliminarse una vez finalizado el proceso. Existe una pequeña posibilidad de que, si estos archivos se encuentran cerca de un sector defectuoso, chkdsk /r los identifique como dañados y se deshaga de ellos.

Chkdsk /r no es una herramienta de recuperación de datos y a veces no recupera correctamente los archivos dañados. El método más seguro para recuperar datos es usar una copia de seguridad creada anteriormente o consultar a un experto antes de ejecutar chkdsk /r.

Si no sabe si optar por chkdsk /f o /r, mediante /r encontrará mucha más información.

Si tiene problemas con el funcionamiento del análisis, una alternativa válida es abrir el símbolo del sistema como administrador y ejecutar chkdsk /f /r /x.

¿Qué hace chkdsk /f?
Chkdsk /f comprueba todo el disco y reescribe el directorio de carpetas para que coincida con el contenido real de la unidad. Esto debe tenerse en cuenta, porque si Windows intenta acceder a un archivo importante del sistema y no está allí, puede provocar una pantalla azul o negra de la muerte, o causar otros fallos y bloqueos.

El disco duro de un equipo es, en cierta manera, como un libro, con la diferencia de que la información almacenada en él se añade, se actualiza, se mueve y se elimina constantemente. Así, la función chkdsk /f aseguraa que el «índice» del disco enumere todos los «capítulos» correctos, que cada «capítulo» tenga una entrada y que todas las entradas apunten a los «números de página» correctos.

Glosario de comandos de CHKDSK
¿Quiere saber otras formas de ejecutar CHKDSK? A continuación, se enumeran algunos comandos diferentes que puede utilizar al ejecutar CHKDSK en el símbolo del sistema:

chkdsk: comprueba si hay problemas en la unidad predeterminada y el sistema de archivos sin solucionar o reparar.

chkdsk [letra de unidad]: ejecuta la misma tarea, pero para la unidad especificada.

/f: la «f» significa «solucionar». Aquí se refiere a solucionar la información del sistema de archivos para que le dirija a los archivos correctos.

/r: la «r» significa «reparación». /r encuentra las partes dañadas del disco duro e intenta recuperar los archivos que se almacenan allí.

/x: desmonta la unidad antes de ejecutar CHKDSK, cosa que puede ser necesaria para que se ejecute.

/f /r /x : ejecuta los comandos /f y /r en una unidad desmontada.

/scan: analiza el disco sin desmontarlo (solo es posible con NTFS).

/b: restablece la lista de clústeres incorrectos (partes dañadas del disco) y vuelve a analizar para detectar su presencia.

/v: comprueba el disco, pero muestra los nombres de los archivos mientras lo hace.

/i: un análisis más rápido y menos exhaustivo. Las entradas del índice se revisan por encima en lugar de comprobarse en profundidad.

/c: otro tipo de análisis superficial. No comprueba los ciclos de las carpetas.

Cómo ejecutar CHKDSK en Windows 10
Hay muchas maneras de ejecutar CHKDSK en Windows 10, incluso cuando el PC parece no funcionar. Si tiene que reparar su disco duro de Windows 10 en una emergencia, CHKDSK podría ser la respuesta.

Hay varias formas de comprobar si hay errores en el disco duro en Windows 10. A continuación, se indican tres opciones de CHKDSK para Windows 10 que puede probar:

Ejecute CHKDSK en su equipo
Puede usar la utilidad CHKDSK desde Windows y la unidad se analizará para detectar errores. Este es el procedimiento para ejecutar CHKDSK en Windows 10:

Escriba chkdsk en el cuadro de búsqueda de la barra de tareas.

Imagen de una barra de tareas con «check disk» escrito, y el usuario ha hecho clic en la aplicación de check disk y está resaltando la opción «Ejecutar como administrador».
Haga clic con el botón derecho en chkdsk y seleccione Ejecutar como administrador.

Este método puede provocar que CHKDSK se ejecute sin mostrarle los resultados. Para obtener resultados más detallados y personalizados, intente ejecutar CHKDSK desde el símbolo del sistema. Los comandos de CHKDSK en Windows 10 son los mismos que en el resto de las versiones de Windows.

Ejecute CHKDSK desde el Símbolo del sistema
El símbolo del sistema es una herramienta útil. Permite ejecutar comandos en Windows e indicar a Windows lo que debe hacer. Si no se va con cuidado, puede causar complicaciones adicionales; por lo tanto, asegúrese de seguir estos pasos al pie de la letra.

Este es el procedimiento para usar el Símbolo del sistema para comprobar el disco:

Escriba cmd (o símbolo del sistema) en el cuadro de búsqueda de la barra de tareas.

Imagen de una barra de tareas con «símbolo del sistema» escrito, y el usuario ha hecho clic en la aplicación de símbolo del sistema y está resaltando la opción «Ejecutar como administrador».
Haga clic con el botón derecho en Símbolo del sistema y seleccione Ejecutar como administrador.

Imagen del símbolo del sistema, con «chkdsk» escrito en la entrada.
Escriba chkdsk y pulse la tecla Entrar. Este comando hará que la utilidad CHKDSK busque problemas sin realizar cambios.

Escriba chkdsk y pulse Intro para que CHKDSK analice el disco para detectar problemas sin realizar cambios.
Para ejecutar CHKDSK en otra unidad diferente de C, especifique el volumen justo después de chkdsk. Por ejemplo, compruebe su unidad D escribiendo chkdsk D: /f.

Escriba chkdsk /r para que CHKDSK repare los archivos dañados, pero solo si se ha detectado un problema. Si en esta fase no hay problemas, no tiene que hacer nada más.

Ejemplo de resultados tras la ejecución de chkdsk. Los resultados indican que no se han encontrado problemas.
Lo mejor del Símbolo del sistema es que se utiliza de forma consistente en todos los sistemas operativos Windows. Tanto si su equipo es nuevo como si tiene 20 años, puede utilizar los mismos comandos, ya que es útil para aprender a ejecutar CHKDSK en Windows 10 o Windows 11.
