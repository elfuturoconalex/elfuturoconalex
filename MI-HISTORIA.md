# Mi historia

🇺🇸 [Read in English](MY-STORY.md)

Me llamo Alejandro. Tengo 45 años y soy un profesional de tecnología cuya carrera se ha construido principalmente alrededor de redes, infraestructura y soluciones Cisco.

A lo largo de mi carrera he trabajado como arquitecto de preventa en un partner de Cisco (un integrador que diseña y vende soluciones Cisco a empresas), un rol que me ha colocado entre dos mundos: el técnico y el humano. No se trata solo de conocer equipos, protocolos o arquitecturas, sino de entender lo que un cliente necesita, traducir esa necesidad en una solución tecnológica y ayudar a distintas personas a entenderla y a tomar decisiones sobre ella.

Mi experiencia me ha permitido desarrollar habilidades tanto técnicas como de comunicación. He trabajado con equipos Cisco, diseñado soluciones, capacitado a otros y compartido conocimiento técnico, participado en proyectos de tecnología y acompañado a clientes en decisiones que muchas veces involucran tecnologías complejas.

En los últimos años me he expandido hacia la **arquitectura de data center**. Hoy trabajo con soluciones de fabricantes como **Dell, Lenovo y Everpure Storage**, y conozco herramientas de respaldo y protección de datos como **Veeam y Commvault**, así como plataformas de virtualización como **VMware y Red Hat**. Este paso me dio una visión más completa de la infraestructura: no solo cómo se conectan las cosas, sino dónde viven los datos, cómo se protegen y cómo corren las aplicaciones.

Una gran parte de mi vida profesional ha sido enfrentar esa complejidad. He tenido que seguir aprendiendo, mantenerme actualizado y adaptarme a tecnologías que evolucionan todo el tiempo. En tecnología, quedarse quieto prácticamente significa quedarse atrás, así que aprender se ha vuelto una parte natural de mi trabajo.

También descubrí que una de mis fortalezas es explicar cosas complejas de forma que otros las entiendan. Puedo pasar de una conversación muy técnica a una con alguien que necesita entender el impacto de una solución sin conocer cada detalle.

Hoy estoy en una etapa en la que veo mi carrera con perspectiva. Tengo experiencia, conocimiento técnico y una visión mucho más amplia de lo que significa trabajar en tecnología que la que tenía cuando empecé.

No soy solo el profesional que sabe de Cisco o que diseña arquitecturas de redes y data center. Soy alguien que ha aprendido a resolver problemas, a trabajar con todo tipo de personas, a asumir proyectos complejos y a seguir aprendiendo aunque cambien las circunstancias.

## Un nuevo capítulo: de las redes a los agentes de IA

Hoy estoy dando un paso que hace unos meses no me hubiera imaginado: estoy construyendo agentes de inteligencia artificial y desplegándolos en AWS.

Empecé con un curso de AWS. Cuando llegué al proyecto final, una arquitectura bancaria completa con varias regiones, redes, bases de datos y alta disponibilidad, me di cuenta de que primero necesitaba bases más sólidas. Así que decidí empezar con algo concreto: un agente investigador que recibe un tema, busca en internet, resume la información y guarda un informe, sin interfaz y sin intervención humana.

Lo interesante es que empecé prácticamente desde cero en programación. No sabía Python, nunca había usado en serio la terminal y no sabía qué era Git. En pocos días configuré mi computadora con herramientas de desarrollo, aprendí Git y GitHub, manejé mis propias llaves de API de forma segura y escribí mis primeros programas.

En el camino también aprendí algo que va más allá del código. Cometí errores reales, como exponer por accidente una llave de API en una captura de pantalla, y aprendí a corregirlos de inmediato y a no repetirlos. Documento cada paso en una bitácora de aprendizaje: no solo lo que hago, sino lo que aprendo y los problemas que resuelvo, porque creo que la forma en que piensas y resuelves problemas importa tanto como el resultado.

### Lo que he construido hasta ahora

**1. Agente Investigador.** Decide por sí mismo qué buscar, hace varias búsquedas y escribe un informe con sus fuentes. Empezó en mi computadora y hoy corre en AWS con Lambda, API Gateway y S3. Revisar sus informes me dejó una gran lección: si no obligas a una IA a citar cada dato y a decir "no encontré esto", rellena los huecos con información irrelevante. Esa es su siguiente mejora.

**2. Agente de Soporte Interno.** Responde preguntas de empleados usando los documentos de una empresa ficticia (vacaciones, viáticos, políticas) con RAG en Amazon Bedrock. Cita de qué documento sacó la respuesta y, cuando la respuesta no está ahí, dice "no lo sé" en lugar de inventar. Le hice un examen automático de 25 preguntas, incluidas preguntas trampa, y sacó 25/25. Para llegar ahí tuve que calibrar un umbral de confianza con datos reales, atrapar una pregunta trampa sobre sueldos que la IA casi contesta y encontrar una sola letra fuera de lugar en mi código que tiró todo el examen a cero.

**3. Agente de Pedidos por Telegram.** Una tiendita de barrio ficticia recibe pedidos por chat. El cliente escribe como habla ("dame 2 kilos de tortilla y un refresco") y el agente consulta el catálogo real, arma el pedido, pide dirección y forma de pago, y lo guarda con un folio. Este fue el que más me enseñó:

- Sin catálogo, la IA inventaba productos que la tienda no vendía.
- Le decía al cliente "tu pedido está confirmado" sin haber guardado nada. Puse una guardia en el código que lo revisa.
- Una prueba automática encontró que el cliente veía un total de $84, pero el pedido se guardaba por $168. A ojo, la conversación se veía perfecta.
- Olvidaba que ya había agregado un producto y lo volvía a agregar: la IA recuerda lo que dijo, no lo que hizo. Ahora el código lleva el pedido y se lo muestra en cada mensaje.
- Aunque el producto decía "AGOTADO", lo seguía ofreciendo. Solo dejó de hacerlo cuando lo saqué por completo de la lista.

Después de cuatro intentos, pasó 8 de 8 conversaciones de prueba.

### Lo que me enseñaron estos agentes

La IA no falla por falta de inteligencia. Falla por falta de datos y de controles. Una regla escrita en el prompt no basta: el dinero y las reglas del negocio los decide y los verifica el código, no el modelo. Sin pruebas automáticas no hay confianza, porque "se ve bien" no es lo mismo que "funciona". Y un agente bien hecho cuesta solo centavos por conversación.

Me di cuenta de que mi experiencia anterior no se queda atrás. Al contrario: entender redes, data centers, almacenamiento, respaldo, virtualización y seguridad me ayuda a ver cómo se conectan las piezas en la nube. Y mi experiencia en preventa me da algo que muchos perfiles técnicos no tienen: la capacidad de explicar para qué sirve una solución, cuánto cuesta y qué valor le aporta a un cliente.

## Hacia dónde voy

Mi meta es construir cinco agentes de IA, cada uno más complejo que el anterior. Dos están terminados y el tercero va en progreso. Lo siguiente es desplegar el agente de pedidos en AWS con Terraform y una fila de mensajes, para que ningún pedido se pierda aunque algo falle. Para los últimos dos estoy explorando un equipo de preventa con IA que redacte propuestas técnicas, y pequeñas herramientas para tareas del día a día de un negocio.

Elegí casos de pequeños negocios a propósito: me obligan a resolver problemas reales, como mensajes humanos desordenados, dinero que tiene que cuadrar exacto, reglas que no se pueden romper y costos que deben mantenerse bajos. Cada agente lo diseño con las mismas preguntas que siempre me he hecho como arquitecto: ¿es confiable?, ¿es seguro?, ¿cuánto cuesta? y ¿lo puedo medir?

También comparto el proceso en público, en español, como **El Futuro con Alex**: lo que construyo, lo que se rompe y lo que aprendo. Explicárselo a otros es mi forma de asegurarme de que de verdad lo entiendo.

Quiero construir un perfil en forma de "T": bases amplias en nube, redes, data center, seguridad y costos, con especialización profunda en agentes de IA en AWS. Mi objetivo es que mi GitHub muestre proyectos reales, funcionando y bien documentados, y poder explicar cada decisión que tomé.

A largo plazo, me veo como Arquitecto de Soluciones especializado en IA, combinando lo que siempre he hecho bien (entender necesidades y convertirlas en soluciones) con una de las tecnologías que más está transformando el mundo hoy.

A los 45 años no estoy empezando de cero: le estoy agregando una nueva capa a todo lo que ya construí.

Y sobre todo, soy Alejandro: un hombre de 45 años que sigue aprendiendo, cuestionando lo que sabe y tratando de entender mejor quién es y qué quiere hacer con todo lo que ha construido hasta ahora.