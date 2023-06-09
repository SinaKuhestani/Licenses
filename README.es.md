# How to Choose a License for Your Own Work
[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/sinabek/licences/blob/main/README.md)
[![pt-br](https://img.shields.io/badge/lang-pt--br-green.svg)](https://github.com/sinabek/licences/blob/main/README.pt.md)
[![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/sinabek/licences/blob/main/README.es.md)
[![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/sinabek/licences/blob/main/README.fr.md)
[![es](https://img.shields.io/badge/lang-es-yellow.svg)](https://github.com/sinabek/licences/blob/main/README.de.md)


La gente a menudo nos pregunta qué licencia recomendamos que usen para su proyecto. Hemos escrito sobre esto públicamente antes, pero la información se ha dispersado entre diferentes ensayos, entradas de preguntas frecuentes y comentarios de licencia. Este artículo recopila toda esa información en una sola fuente, para que sea más fácil para las personas seguirla y consultarla.


Estas recomendaciones son para trabajos diseñados para realizar trabajos prácticos. Estos incluyen software, documentación y algunas otras cosas. Las obras de arte y las obras que expresan un punto de vista son cuestiones diferentes; el Proyecto GNU no tiene una posición general sobre cómo deberían publicarse, excepto que todos deberían poder utilizarse sin software no libre (en particular, sin DRM). Sin embargo, es posible que desee seguir estas recomendaciones para las obras de arte que acompañan a un programa en particular.


Las recomendaciones se aplican a la licencia de un trabajo que usted crea, ya sea una modificación de un trabajo existente o un nuevo trabajo original. No abordan el tema de combinar material existente bajo diferentes licencias. Si está buscando ayuda con eso, consulte nuestras Preguntas frecuentes sobre GPL.

Después de ver lo que recomendamos aquí, si desea asesoramiento, puede escribir a <licensing@gnu.org>. Tenga en cuenta que es probable que el equipo de licencias tarde algunas semanas en comunicarse con usted; si no obtiene respuesta en un mes, por favor vuelva a escribir.


## Contribuir a un proyecto existente


Cuando contribuye a un proyecto existente, generalmente debe publicar sus versiones modificadas bajo la misma licencia que el trabajo original. Es bueno cooperar con los mantenedores del proyecto, y el uso de una licencia diferente para sus modificaciones a menudo hace que la cooperación sea muy difícil. Solo debe hacer eso cuando haya una razón poderosa que lo justifique.


Un caso en el que se puede justificar el uso de una licencia diferente es cuando realiza cambios importantes en un trabajo bajo una licencia sin copyleft. Si la versión que ha creado es considerablemente más útil que la original, entonces vale la pena copiar su trabajo con copyleft, por las mismas razones que normalmente recomendamos copyleft. Si se encuentra en esta situación, siga las recomendaciones a continuación para obtener la licencia de un nuevo proyecto.


Si elige publicar sus contribuciones bajo una licencia diferente por cualquier motivo, debe asegurarse de que la licencia original permita el uso del material bajo la licencia elegida. En aras de la honestidad, muestre explícitamente qué partes del trabajo están bajo qué licencia.


### Software


Recomendamos diferentes licencias para diferentes proyectos, dependiendo principalmente del propósito del software. En general, recomendamos usar la licencia copyleft más sólida que no interfiera con ese propósito. Nuestro ensayo “¿Qué es Copyleft?” explica el concepto de copyleft con más detalle y por qué generalmente es la mejor estrategia de licenciamiento.


Para la mayoría de los programas, le recomendamos que utilice la versión más reciente de la Licencia pública general de GNU (GPL) para su proyecto. Su fuerte copyleft es apropiado para todo tipo de software e incluye numerosas protecciones para la libertad de los usuarios. Para permitir futuras actualizaciones de la licencia, especifique "versión 3 o cualquier versión posterior" para que su programa sea compatible con la licencia con el código que puede publicarse, en el futuro, bajo versiones posteriores de GPL.


### Pequeños programas


No vale la pena usar copyleft para la mayoría de los programas pequeños. Usamos 300 líneas como punto de referencia: cuando el código fuente de un paquete de software es más corto que eso, los beneficios proporcionados por el copyleft suelen ser demasiado pequeños para justificar la inconveniencia de asegurarse de que una copia de la licencia siempre acompañe al software.


Para esos programas, recomendamos la Licencia Apache 2.0. Se trata de una licencia de software débil, laxa, "pushover" (sin copyleft) que tiene términos para evitar que los contribuyentes y distribuidores demanden por infracción de patente. Esto no hace que el software sea inmune a las amenazas de las patentes (ninguna licencia de software puede lograrlo), pero evita que los titulares de patentes configuren un "cebo y cambio" en el que lanzan el software en términos gratuitos y luego requieren que los destinatarios acepten términos no libres en una licencia de patente.


Entre las licencias débiles (pushover), Apache 2.0 es la mejor; por lo tanto, si va a utilizar una licencia débil, sea cual sea el motivo, le recomendamos que utilice esa.

### Bibliotecas


Para las bibliotecas, distinguimos tres tipos de casos.


Algunas bibliotecas implementan formatos de datos gratuitos que compiten con formatos de datos restringidos, como Ogg Vorbis (que compite con audio MP3) y WebM (que compite con video MPEG-4). El éxito del formato libre requiere permitir que muchos programas de aplicación patentados se vinculen en el código para manejar el formato. Por ejemplo, queríamos que los reproductores de medios no libres, especialmente los electrodomésticos, incluyeran el código para Ogg Vorbis además de MP3.


En estas situaciones especiales, si su objetivo es convencer a los desarrolladores de aplicaciones propietarias para que utilicen la biblioteca para el formato libre, deberá facilitarlo otorgando una licencia de la biblioteca con una licencia débil, como Apache License 2.0.


Sin embargo, debemos reconocer que esta estrategia no funcionó para Ogg Vorbis. Incluso después de cambiar la licencia de derechos de autor para permitir la fácil inclusión de ese código de biblioteca en aplicaciones propietarias, los desarrolladores propietarios generalmente no lo incluyeron. El sacrificio hecho en la elección de la licencia finalmente nos ganó poco.


Para todas las demás bibliotecas, recomendamos algún tipo de copyleft. Si los desarrolladores ya están usando una biblioteca alternativa establecida publicada bajo una licencia no libre o una licencia laxa, entonces recomendamos usar la Licencia Pública General Menor de GNU (LGPL).


A diferencia del primer caso, donde la biblioteca implementa un estándar éticamente superior, aquí la adopción por sí misma no logrará ningún objetivo especial, por lo que no hay razón para evitar el copyleft por completo. Sin embargo, si requiere que los desarrolladores que usan su biblioteca publiquen sus programas completos bajo copyleft, simplemente usarán una de las alternativas disponibles, y eso tampoco ayudará a nuestra causa. La Lesser GPL fue diseñada para llenar el término medio entre estos casos, permitiendo a los desarrolladores de software propietario usar la biblioteca cubierta, pero brindando un copyleft débil que brinda a los usuarios libertad con respecto al código de la biblioteca en sí.


Para las bibliotecas que brindan instalaciones especializadas y que no se enfrentan a una competencia arraigada sin copyleft o no libre, recomendamos utilizar la GPL de GNU simple. Para conocer las razones, lea "Por qué no debería usar la GPL menor para su próxima biblioteca".


### Software de servidor


Si es probable que otros hagan versiones mejoradas de su programa para que se ejecuten en servidores y no distribuyan sus versiones a nadie más, y le preocupa que esto ponga en desventaja a su versión lanzada, le recomendamos la Licencia Pública General GNU Affero (AGPL). Los términos de la AGPL son casi idénticos a los de la GPL; la única diferencia sustantiva es que tiene una condición adicional para garantizar que las personas que usan el software en una red puedan obtener el código fuente.


El requisito de la AGPL no aborda los problemas que pueden surgir para los usuarios cuando confían su computación o sus datos al servidor de otra persona. Por ejemplo, no impedirá que el Servicio como sustituto del software (SaaSS) niegue la libertad de los usuarios, pero la mayoría de los servidores no utilizan SaaSS. Para obtener más información sobre estos temas, lea “Por qué Affero GPL”.


### Documentación


Recomendamos la Licencia de documentación libre de GNU (GFDL) para tutoriales, manuales de referencia y otros trabajos extensos de documentación. Es una licencia fuerte con copyleft para obras educativas, escrita inicialmente para manuales de software, e incluye términos que abordan específicamente problemas comunes que surgen cuando esas obras se distribuyen o modifican.


Para trabajos breves de documentación secundaria, como una tarjeta de referencia, es mejor usar la licencia GNU all-permissive, ya que una copia de la GFDL difícilmente cabría en una tarjeta de referencia. No uses CC BY, ya que es incompatible con GFDL.


Para las páginas man, recomendamos la GFDL si la página es larga y la licencia GNU all-permissive si es corta.


Parte de la documentación incluye el código fuente del software. Por ejemplo, un manual para un lenguaje de programación podría incluir ejemplos para que los lectores los sigan. Debe incluirlos en el manual según los términos de la FDL y publicarlos bajo otra licencia que sea apropiada para el software. Hacerlo ayuda a facilitar el uso del código en otros proyectos. Le recomendamos que dedique pequeños fragmentos de código al dominio público mediante CC0 y que distribuya fragmentos más grandes con la misma licencia que utiliza el proyecto de software asociado.

### Otros datos para programas


Esta sección analiza todos los demás trabajos para uso práctico que puede incluir con el software. Para darle algunos ejemplos, esto incluye íconos y otros gráficos, fuentes y datos geográficos funcionales o útiles. También puede seguirlos por arte, aunque no lo criticaríamos si no lo hace.


Si está creando estos trabajos específicamente para usarlos con un proyecto de software, generalmente recomendamos que publique su trabajo bajo la misma licencia que el software. No hay problema en hacerlo con las licencias que hemos recomendado: GPLv3, LGPLv3, AGPLv3 y GPLv2 se pueden aplicar a cualquier tipo de trabajo, no solo software, que tenga derechos de autor y tenga una forma preferida clara de modificación. El uso de la misma licencia que el software ayudará a que el cumplimiento sea más fácil para los distribuidores y evitará cualquier duda sobre posibles problemas de compatibilidad. El uso de una licencia gratuita diferente puede ser apropiado si proporciona algún beneficio práctico específico, como una mejor cooperación con otros proyectos gratuitos.


Si su trabajo no se está creando para usar con un proyecto de software en particular, o si no sería apropiado usar la misma licencia que el proyecto, solo le recomendamos que elija una licencia copyleft que sea apropiada para su trabajo. Tenemos algunos de estos listados en nuestra lista de licencias. Si ninguna licencia parece especialmente apropiada, la licencia Creative Commons Attribution-ShareAlike es un copyleft que se puede utilizar para muchos tipos diferentes de obras.