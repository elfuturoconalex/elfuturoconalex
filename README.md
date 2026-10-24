# Hola, soy Alejandro

**Arquitecto de Soluciones en Redes y Data Center → Construyendo Agentes de IA en AWS**

🇺🇸 [Read in English](README-EN.md)

Soy profesional de tecnología con años de experiencia como **arquitecto de preventa** en un **partner de Cisco**, diseñando soluciones de **redes** e infraestructura de **data center**. Mi trabajo está entre dos mundos: el técnico y el humano. Entiendo lo que un cliente necesita y lo convierto en una solución que la gente pueda entender y decidir.

Ahora llevo ese mismo enfoque a la IA: construyo agentes en los que un pequeño negocio pueda confiar, que funcionan 24/7 en AWS y cuestan centavos por conversación.

### Lo que aporto
- **Redes:** arquitecturas y diseño de soluciones Cisco
- **Data center:** Dell, Lenovo, Everpure Storage
- **Respaldo y protección de datos:** Veeam, Commvault
- **Virtualización:** VMware, Red Hat
- **Comunicación:** explicar tecnología compleja para que la gente pueda tomar decisiones

### Lo que estoy construyendo
Estoy aprendiendo a **construir agentes de IA y desplegarlos en AWS**, empezando desde cero en programación. Mi meta: **5 agentes de IA**, cada uno más complejo que el anterior.

| # | Proyecto | Estado |
|---|---|---|
| 1 | [**Agente Investigador**](https://github.com/elfuturoconalex/agente-investigador): busca en la web y escribe un informe con sus fuentes. Con trazas bajé su costo por informe un 22% | ✅ Local · ✅ AWS (Bedrock) |
| 2 | [**Agente de Soporte Interno**](https://github.com/elfuturoconalex/agente-soporte-interno): responde preguntas de empleados con los documentos de la empresa (RAG en Bedrock + Lambda + API Gateway). Cita el documento y dice "no lo sé" en lugar de inventar | ✅ Terminado · **25/25** en examen automático |
| 3 | [**Agente de Pedidos por Telegram**](https://github.com/elfuturoconalex/agente-pedidos-telegram): toma pedidos como habla el cliente, consulta un catálogo real, confirma dirección y pago, y guarda cada pedido con folio | 🔄 Fase 1 de 3 · **8/8** en examen automático |
| 4–5 | Próximamente | ⏳ |

*Todas las demos usan empresas y datos ficticios.*

### Lo que me enseñó construirlos
- **La IA no falla por falta de inteligencia, falla por falta de datos y de controles.** El dinero y las reglas del negocio los decide el código, no el modelo.
- **Una regla en el prompt no basta.** Mi agente de pedidos decía "tu pedido está confirmado" sin haber guardado nada. Una guardia en el código lo corrigió.
- **La IA recuerda lo que dijo, no lo que hizo.** Olvidó que ya había agregado un producto y lo agregó otra vez. Ahora el código lleva el pedido y se lo muestra al modelo en cada mensaje.
- **Sin examen no hay confianza.** Una conversación que se veía perfecta guardaba pedidos al doble del precio. Solo las pruebas automáticas lo encontraron.
- **Un agente bien hecho cuesta centavos por conversación.**

**Stack:** Python · Claude API · Amazon Bedrock · RAG · AWS Lambda · API Gateway · S3 · CloudWatch · Tavily · Telegram Bot API · Git/GitHub · Terraform (en progreso)

### Hacia dónde voy
Construyo un perfil en forma de "T": bases amplias en nube, redes, data center, seguridad y costos, con especialización profunda en **agentes de IA en AWS**. A largo plazo: **Arquitecto de Soluciones especializado en IA**, ayudando a pequeños negocios de México y Latinoamérica a poner agentes a trabajar.

### Platiquemos
¿Quieres llevar agentes de IA a tu negocio o buscas un arquitecto de IA en AWS?
👉 [LinkedIn](https://www.linkedin.com/in/yosoyalexpadilla/) · Comparto el proceso en español como **El Futuro con Alex**

📖 [Lee mi historia completa](MI-HISTORIA.md)

> A los 45 años no estoy empezando de cero: le estoy agregando una nueva capa a todo lo que ya construí.
