<p align="center">
  <img src="public/assets/images-doc/Logo-Upc.png" alt="Logo UPC" width="300">
</p>
# UNIVERSIDAD PERUANA DE CIENCIAS APLICADAS
## Ingeniería de Software

**Período:** 2026-1  
**Curso:** 1ASI0730 | Aplicaciones Web  
**NRC:** 12190  
**Docente:** Hugo Allan Mori Paiva  

---

# INFORME DE TRABAJO FINAL

## Relación de integrantes

| Código | Apellidos y nombres |
| :--- | :--- |
| U201924127 | Alberca Saavedra, Victor Manuel |
| U201724692 | Komatsu Dueñas, David |
| [Completar] | [Completar] |

---

## Registro de Versiones del Informe

| Versión | Fecha | Autor | Descripción de modificación |
| :--- | :--- | :--- | :--- |
| **v.01.Tb1** | 19/04/2026 | Meza Soza, Alexandra Yamile<br>Alberca Saavedra, Víctor Manuel<br>Komatsu Dueñas, David | Se agregaron los tópicos correspondientes a los Capítulos I, II, III, IV y V, abarcando desde el Startup Profile y Requirements Elicitation, hasta la arquitectura, diseño UI/UX (Landing Page y Mobile) y el Sprint 1. |
| **v.01.Tp1** | [Fecha] | [Autor] | Se agregaron los siguientes tópicos: [Completar] |
| **v.01.Tb2** | [Fecha] | [Autor] | Se agregaron los siguientes tópicos: [Completar] |
| **v.01.Tf** | [Fecha] | [Autor] | Se agregaron los siguientes tópicos: [Completar] |

*(Nota: En la versión v.01.Tb1 he resumido la lista de capítulos para que la tabla sea legible en GitHub. Si necesitas el listado exhaustivo de cada subcapítulo, te recomiendo ponerlo fuera de la tabla).*

---

## Student Outcome

| Criterio específico | Acciones realizadas | Conclusiones |
| :--- | :--- | :--- |
| **Trabaja en equipo para proporcionar liderazgo en forma conjunta** | **Victor Alberca:**<br>TB1: Participé en todo el proceso de desarrollo del proyecto, desde la investigación hasta la validación final...<br><br>**David Komatsu:**<br>TB1: Realicé entrevistas para obtener información de la problemática...<br>TP1: Encontré requerimientos de las funcionalidades...<br>TB2: Realicé entrevistas de validación y analicé detalladamente...<br>TF: Identifique partes del código con errores y duplicados...<br><br>**Alexandra Meza:**<br>TB1: Realicé y registré entrevistas para conocer mejor las perspectivas...<br>TP1: Diseñe los Wireframes y los mockups de los Landing Pages...<br>TB2: A través de la elaboración de la landing page...<br>TF: Durante la culminación del landing page e implementación... | En la TB1, el equipo realizó diversas actividades clave: análisis competitivo, entrevistas, diseño de User Personas y validación del documento...<br><br>En el TP1, el equipo se enfocó en analizar y estructurar de manera más profunda los problemas mediante To-Be Scenario Mapping, Impact Mapping, Historias de Usuario, Wireframes y Mockups...<br><br>En la TB2, el equipo realizó entrevistas de validación, detectó oportunidades de mejora en navegación y aplicó evaluaciones heurísticas...<br><br>En el TF, el equipo identificó y resolvió problemas complejos en navegación, consistencia visual, estructura de clases y código. |
| **Crea un entorno colaborativo e inclusivo, establece metas, planifica tareas y cumple objetivos** | **Victor Alberca:**<br>TB1: Organicé y analicé la información de entrevistas...<br><br>**David Komatsu:**<br>TB1: Con la información obtenida diseñe el empathy map...<br>TP1: Alineamos las historias de usuario acorde a las necesidades...<br>TB2: Con la información obtenida, precisé los requerimientos...<br>TF: Registré el avance grupal de las nuevas funcionalidades...<br><br>**Alexandra Meza:**<br>TB1: Tras analizar los datos, reconocí los comportamientos y lo agregué al User task Matrix...<br>TP1: Para realizar el diseño de los wireframes, pensé en cómo incluir correctamente el tipo de diseño...<br>TB2: Formulé los problemas encontrados estructurando los hallazgos...<br>TF: Formulé patrones complejos de diseño para adaptar la interfaz... | En esta etapa, el equipo organizó la información para nutrir el User Task Matrix, el Empathy Map y los User Personas, y definió la problemática y el modelo de negocio...<br><br>Durante esta etapa, se formularon criterios de aceptación, el Product Backlog y flujos de navegación lógicos...<br><br>En la TB2, el equipo profundizó en la definición técnica mediante entrevistas y mejoró la arquitectura de la landing page...<br><br>En esta etapa final, se convirtieron problemas detectados en requisitos claros y se corrigieron fallas en diseño responsive y código. |

---

# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup

**Innovify** es una startup cuyo propósito es reducir la deserción académica conectando a estudiantes universitarios para que compartan conocimientos a través de sesiones de tutoría. Esta iniciativa resuelve de manera ágil las dudas específicas de los alumnos mediante dos modalidades integradas: un aprendizaje sincrónico, llevado a cabo en tiempo real a través de videollamadas incrustadas en la misma plataforma (mediante el consumo de APIs de video externas), y un aprendizaje asincrónico, que facilita el intercambio de materiales y recursos de estudio directamente en el entorno de la reserva.

A diferencia de los modelos tradicionales, nuestra plataforma se sostiene bajo un modelo de negocio mixto (B2C y B2B). Por el lado del estudiante (B2C), operamos bajo un sistema colaborativo de donaciones voluntarias; al finalizar una tutoría, el aprendiz puede realizar un aporte económico al tutor como agradecimiento, procesado mediante una pasarela de pagos segura, de la cual Innovify retiene una comisión del 5% para garantizar su sostenibilidad. Por el lado institucional (B2B), Innovify ofrece alianzas estratégicas a las universidades, brindándoles acceso a un Dashboard Analítico ("Termómetro Académico") que les permite visualizar estadísticas en tiempo real sobre los cursos con mayor demanda de tutorías, ayudándolas a prevenir la deserción estudiantil.

Todo este ecosistema se mantiene seguro y escalable gracias a un proceso de validación automatizada que exige el uso de correos institucionales (`.edu.pe` o `upc.edu.pe`, `pupc.edu.pe`) para garantizar que los usuarios sean estudiantes reales. Asimismo, la calidad académica está respaldada por la participación de los Profesores Universitarios, quienes actúan como garantes de excelencia al crear el banco oficial de quizzes y retos que los tutores utilizan para evaluar a sus aprendices, fomentando un entorno confiable, profesional y altamente colaborativo.

Asimismo, pensando en la escalabilidad y el aseguramiento de la calidad a futuro, Innovify contempla la integración de tecnología IoT en su ecosistema. El roadmap tecnológico incluye el desarrollo de un **'Sensor de Calidad de Entorno'**: un dispositivo miniatura basado en un microcontrolador (ej. ESP32) equipado con sensores de luz y ruido, diseñado para ubicarse en el área de estudio del tutor. Durante el aprendizaje sincrónico, este hardware enviará métricas ambientales en tiempo real al backend. Si el entorno presenta contaminación auditiva o iluminación deficiente, la plataforma alertará al tutor para que mejore sus condiciones. Por el contrario, parámetros óptimos otorgarán automáticamente un 'Badge de Excelencia Técnica' a la sesión. Esta proyección IoT asegura que el servicio por el cual el aprendiz realiza su donación económica mantenga siempre un estándar de alta calidad profesional.

### Visión
Ser la plataforma líder en educación colaborativa universitaria a nivel nacional, reconocida por ser el principal aliado estratégico de las instituciones en la prevención de la deserción académica, potenciando el aprendizaje mediante tecnología escalable, entornos validados por IoT y un ecosistema económicamente sostenible.

### Misión
Facilitar el aprendizaje sincrónico y asincrónico entre estudiantes universitarios proporcionando herramientas digitales integradas, seguras y automatizadas. Promovemos la excelencia académica, la mejora de habilidades blandas y la recompensa justa al esfuerzo del tutor mediante donaciones voluntarias, operando bajo un entorno validado institucionalmente que brinda data de valor a las universidades para optimizar sus planes de estudio.
### 1.1.2. Perfiles de integrantes del equipo

| Foto | Integrante | Carrera | Descripción |
| :---: | :--- | :--- | :--- |
| <img src="public/assets/images/image-perfil-victor.png" width="100"> | **Alberca Saavedra, Victor Manuel**<br>(U201924127) | Ingeniería de Software | Puedo aportar mis conocimientos básicos de investigación para los temas y tengo experiencia en el leguaje C++. También puedo aportar al grupo con el aspecto comunicativo y organizativo para si poder realizar un mejor trabajo. |
| <img src="public/assets/images/image-david.png" width="100"> | **Komatsu Dueñas, David**<br>(U201724692) | Ingeniería de Software | Me gustaría aportar a este proyecto con mis conocimientos adquiridos en investigación y sus respectivas metodologías, y la experiencia universitaria adquirida en el lenguaje C++ y JavaScript. También, aportare con mis habilidades de comunicación asertiva y buen trabajo en equipo. |
| <img src="images/foto-integrante3.jpg" width="100"> | **[Nombre Integrante 3]**<br>([Código]) | Ingeniería de Sistemas de Información | Estudiante de Ingeniería de Sistemas de Información con enfoque en análisis de datos y desarrollo básico en Python/C++. Me caracterizo por aprendizaje rápido, criterio para filtrar información relevante y trabajo colaborativo. En el equipo aporto investigación aplicada y prototipos técnicos que conectan los hallazgos con funcionalidades del producto. |
| <img src="images/foto-integrante4.jpg" width="100"> | **[Nombre Integrante 4]**<br>([Código]) | Ingeniería de Sistemas de Información | Estudiante de la carrera de ingeniería de sistemas en la UPC. Domino C#, Java, C++ y me gusta trabajar en equipo para lograr un objetivo. Tengo habilidades además de programar con el diseño. En el equipo aportaré a nuestra landing page con mis conocimientos, un diseño limpio y agradable para el usuario. |
| <img src="images/foto-integrante5.jpg" width="100"> | **[Nombre Integrante 5]**<br>([Código]) | Ingeniería de Sistemas de Información | Puedo aportar mis conocimientos en C++ y Python. Además de la generación de tablas y gráficos estadísticos desde la depuración de un mismo código y el acceso a una base de datos desde las hojas de cálculo de Excel en sus diferentes formatos hasta base de datos en SQL Server. |
| <img src="images/foto-integrante6.jpg" width="100"> | **[Nombre Integrante 6]**<br>([Código]) | Ingeniería de Software | Me gustaría aportar a este proyecto con mis conocimientos en programación en los lenguajes C++, Python, HTML y CSS. Asimismo, puedo contribuir al equipo con habilidades en trabajo colaborativo, organización y resolución de problemas. |

*(Tabla 1. Perfiles integrantes de equipo - Elaboración propia. Nota: En esta tabla se aprecia los perfiles de los integrantes de equipo).*

---

## 1.2. Solution Profile

### 1.2.1. Antecedentes y problemática

En el Perú, el fracaso académico, manifestado mediante un bajo rendimiento académico, la reprobación de cursos y la deserción, es un problema que afecta a varios estudiantes de diversas universidades, tanto públicas como privadas. De acuerdo con el Minedu (2021), la tasa de interrupción de estudios en universidades licenciadas llegó a 11,5% en el ciclo 2021-1, siendo Lima una de las regiones con tasas de deserción más altas, con un 12,4%.

Diversos estudios asocian un ambiente de aprendizaje inadecuado y una enseñanza poco satisfactoria como parte de las causas de este problema, así como factores mentales y emocionales como la falta de apoyo social, bajos niveles de motivación intrínseca y falta de autoestima (Escalante et al., 2023).

Si bien estas causas son multifactoriales, nuestra investigación identifica un problema subyacente y desatendido: **el aislamiento del conocimiento**. Cada universidad, con sus fortalezas y debilidades, funciona como una isla académica. El talento y la pericia de sus estudiantes permanecen encapsulados dentro de sus propios campus, desaprovechando una vasta red de conocimiento distribuido a nivel nacional. Actualmente, no existe un puente formal, seguro y confiable que permita a un estudiante de una universidad A, que necesita ayuda en un tema específico, conectar con un par de la universidad B que domine esa área. Los estudiantes se ven limitados a su círculo inmediato o a grupos informales en redes sociales que carecen de seguridad y verificación.

Esto no solo impacta negativamente en el bienestar social y económico de los mismos estudiantes sino también en la capacidad productiva del país por falta de mano de obra calificada, agravando problemas socioeconómicos como los niveles de vida deficientes, las altas tasas de desempleo y el incremento de comportamientos disruptivos en la sociedad (Escalante et al., 2023).

Para conocer aún más la problemática usaremos la técnica de las **5W y 2H**:

#### What (¿Qué? / ¿Cuál?)
* **¿Cuál es el problema?** El problema es la deserción universitaria ocasionada por diversos factores tales como falta de aprendizaje, estrés académico, bajos niveles económicos, etc. Por consecuencia, muchos estudiantes terminan suspendiendo sus estudios universitarios y, en el peor de los casos, muchos de ellos nunca llegan a terminarlos.
* **¿Qué soluciones existen actualmente?** Actualmente existen plataformas académicas como *[Colocar las empresas aquí]*. Sin embargo, en el país no han alcanzado gran popularidad debido al limitado impacto que han tenido en la comunidad universitaria peruana. Con nuestra propuesta de valor buscamos generar ese impacto a través de un sistema de conexión entre estudiantes, facilitando un aprendizaje sincrónico mediante videollamadas integradas y asincrónico a través de recursos compartidos, todo esto bajo un modelo sostenible de donaciones voluntarias.
* **¿Cuál es la relación con el usuario?** El usuario es el eje central de nuestra plataforma, ya que es quien le da vida mediante la realización de consultas y el intercambio de conocimientos. En caso de asumir el rol de tutor, también tendrá la responsabilidad de guiar al aprendiz, recibiendo donaciones monetarias por su tiempo invertido, lo que aporta mayor seguridad y confianza al ecosistema.

#### Why (¿Por qué?)
* **¿Cuál es la causa principal del problema?** Consideramos que, si bien en la primera pregunta del segmento "What" se mencionaron diversas causas, todas confluyen en un mismo problema principal: no todos los estudiantes logran comprender completamente los temas en clase. Con frecuencia, el tiempo resulta insuficiente y varios de ellos quedan con dudas sin resolver debido a distintos factores. Por esta razón, muchos recurren a estrategias de aprendizaje que no siempre se adaptan a ellos.

#### Who (¿Quién?)
* **¿Quiénes están involucrados?** Está involucrada toda la comunidad universitaria, incluidos estudiantes y profesores, así como los rectores.
* **¿A quiénes les sucede el problema?** Estudiantes universitarios hispanohablantes que necesiten ayuda para resolver dudas inconclusas de sus clases, así como tutores que deseen ayudar a otros alumnos a concluir sus estudios de manera satisfactoria.

#### When (¿Cuándo?)
* **¿Cuándo sucede el problema?** Constantemente, en el Perú las cifras de deserción universitaria son inmensas y más en estos últimos años en que los trabajos y las empresas en general se mueven más por contactos y experiencia, dejando en un segundo plano e infravalorando a los estudios universitarios.
* **¿Cuándo el cliente usa el producto?** Cuando uno de los muchos estudiantes universitarios tiene dudas que no fueron resueltas en clase y no disponen de mucho tiempo para leerse libros inmensos con toda la teoría o necesitan ejemplos que se adaptan más a su velocidad de aprendizaje.

#### Where (¿Dónde?)
* **¿Dónde está el usuario cuando usa la plataforma?** En su lugar favorito dedicado al estudio, no es un lugar en específico y en su mayoría depende mucho de las preferencias y disponibilidad del estudiante. Comúnmente son espacios universitarios dedicados al estudio, salas de estudio dentro de las casas o habitaciones en silencio para la concentración del estudiante o tutor.
* **¿Dónde surge el problema?** En las universidades y sus sistemas que muchas veces no terminan de complementarse bien con el estudiante.

#### How (¿Cómo?)
* **¿En qué condiciones los clientes usan nuestro producto?** Los clientes usan nuestro producto cuando tienen dudas que necesiten resolver, cuando deseen estudiar para un examen o simplemente tengan tiempo libre y quieran ayudar a otros universitarios, ya que de todas maneras serán recompensados.
* **¿Cómo se enteran de la aplicación?** A través de redes sociales, pruebas piloto dentro de nuestra universidad y la recomendación de su uso por parte de contactos o profesores.

#### How much (¿Cuánto?)
* **¿Cuánto le cuesta este problema a la economía, sociedad o institución del Perú actualmente?** Actualmente la educación universitaria está siendo respaldada en gran parte por el gobierno, ya que se conoce que se realizó un incremento de presupuesto del 24% respecto al año 2023, lo que significan unos S/8 416 millones en total (Gobierno del Perú, 2024).
* **¿Cuánto costaría implementar la solución propuesta?**
  * Desarrollo web MVP: S/ 19,000 - S/38,000
  * Aplicación móvil (híbrida): S/19,000 - S/30,400
  * Integración de APIs, videollamada y pasarela de pagos: S/ 3,000 - S/6,000
  * Diseño UI/UX: S/ 3,040 - S/7,600
  * Dominio + hosting: S/570 - S/1,900
  * Seguridad y soporte: S/ 2,280 - S/6,080

---

### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements
Nuestra plataforma se enfoca en crear una red de aprendizaje colaborativo e intercambio de conocimientos exclusivamente entre estudiantes de distintas universidades peruanas. Buscamos romper los silos académicos tradicionales para que los estudiantes puedan complementar su formación, resolver dudas y desarrollar nuevas competencias con pares que de otra manera no conocerían. La plataforma facilitará un entorno de apoyo mutuo: los estudiantes podrán recibir ayuda sincrónica (videollamadas) o asincrónica (materiales compartidos), y los tutores serán recompensados con donaciones voluntarias de las cuales la plataforma retendrá un 5% de comisión para asegurar su sostenibilidad.

La problemática que abordamos es el fracaso y la deserción académica en el sistema universitario peruano, un fenómeno agravado por el aislamiento estudiantil y la falta de acceso a perspectivas académicas. Según datos del MINEDU (2021), la tasa de interrupción de estudios alcanzó el 11.5%, siendo Lima una de las regiones más afectadas (12.4%). Este fenómeno se relaciona con bajos niveles de motivación y entornos de aprendizaje poco satisfactorios, donde muchos estudiantes no encuentran el soporte necesario para superar cursos o desarrollar habilidades específicas.

Hemos observado que, si bien cada universidad cuenta con talento y fortalezas específicas, este conocimiento permanece encapsulado dentro de sus propios campus. Un estudiante de la UNI puede tener una habilidad en cálculo que un estudiante de la UPC necesita, y viceversa, este último puede dominar una herramienta de diseño crucial para el primero. El problema central es la inexistencia de un puente formal y seguro que conecte a estos estudiantes, lo que genera una brecha de oportunidad y desaprovecha un valioso capital de conocimiento distribuido en el país. Las soluciones informales actuales, como los grupos en redes sociales, carecen de sistemas de verificación y confianza, exponiendo a los alumnos a riesgos e interacciones de baja calidad.

A raíz de esta problemática, nuestra propuesta busca responder a la siguiente pregunta: **¿Cómo podríamos crear un ecosistema digital que conecte a estudiantes de distintas universidades peruanas para que enseñen y aprendan de forma segura, fomentando el apoyo mutuo de forma sincrónica y asincrónica, bajo un modelo de negocio sostenible de donaciones voluntarias?**

#### 1.2.2.2. Lean UX Assumptions
Para abordar de manera efectiva la problemática del fracaso académico y la deserción universitaria, es fundamental partir de una serie de supuestos sobre nuestros usuarios y su contexto. El éxito de Innovify depende de qué tan acertadas sean estas hipótesis centradas en el usuario tecnológico y en nuestro modelo de negocio sostenible.

Nuestro análisis del entorno universitario peruano revela que los estudiantes enfrentan barreras académicas que limitan su progreso. Suponemos que existe un vacío en su experiencia de aprendizaje, y que muchos buscan activamente apoyo personalizado. Creemos que los estudiantes valoran recibir clases de pares de otras universidades, siempre que el entorno cuente con herramientas integradas que faciliten un aprendizaje sincrónico (en vivo) y asincrónico (intercambio de materiales).

Asimismo, identificamos que la falta de incentivos reales frena la colaboración continua. En cuanto a la motivación, creemos que los estudiantes con buen rendimiento académico (Tutores) están dispuestos a invertir su tiempo si pueden reforzar su propio aprendizaje y, a la vez, ser recompensados mediante un sistema de donaciones voluntarias por su esfuerzo.

Nuestra propuesta se distinguirá al ofrecer una plataforma centralizada y verificada. Innovify integrará funcionalidades clave mediante servicios de terceros (APIs de videollamada y pasarelas de pago) para que los estudiantes no tengan que salir de la aplicación, generando así un ecosistema seguro, estructurado y económicamente sostenible gracias a la retención de una pequeña comisión (5%) por cada donación procesada.

##### Assumptions Worksheet

| Pregunta | Respuesta |
| :--- | :--- |
| **¿Quién es el usuario?** | Nuestros usuarios son estudiantes universitarios peruanos de diversas carreras que se dividen en dos roles principales:<br>1. **El Aprendiz:** Estudiante universitario que se siente estancado en ciertos temas y valora la ayuda en tiempo real (sincrónica) o mediante materiales compartidos (asincrónica).<br>2. **El Tutor:** Estudiante que domina una materia, motivado por ayudar a otros, consolidar sus conocimientos y recibir donaciones económicas voluntarias por su tiempo. |
| **¿Dónde encaja nuestro producto en su trabajo o vida?** | Creemos que los estudiantes buscarán apoyo fuera de su horario de clases regular, prefiriendo organizar videollamadas en horarios flexibles sin tener que depender de aplicaciones externas inseguras. |
| **¿Qué problemas tiene nuestro producto a resolver?** | • **Problema de Herramientas Fragmentadas:** Asumimos que los estudiantes se frustran al tener que usar WhatsApp para coordinar, Drive para materiales y Zoom para la clase. Todo debe estar integrado.<br>• **Problema de Sostenibilidad e Incentivo:** Asumimos que los tutores se desmotivan si no ven un beneficio tangible. El sistema de donaciones resuelve esto, y la comisión del 5% resuelve la sostenibilidad del negocio.<br>• **Problema de Seguridad:** Asumimos que interactuar con estudiantes de otras universidades genera fricción si no hay un Administrador/Verificador validando las cuentas y moderando reportes. |
| **¿Cuándo y cómo es nuestro producto usado?** | El uso se intensificará en picos de estrés académico (semanas de parciales/finales). Los alumnos agendarán sesiones en vivo (sincrónicas) o enviarán documentos para revisión (asincrónico) de manera centralizada. |
| **¿Qué características son importantes?** | • **Videollamada Integrada:** Es fundamental que la clase ocurra dentro de la plataforma usando una API externa.<br>• **Pasarela de Pagos Confiable:** Para procesar las donaciones de forma rápida y segura.<br>• **Seguridad y Moderación:** Un panel donde el Verificador pueda atender reportes y asegurar la calidad. |
| **¿Cómo debe verse nuestro producto y cómo comportarse?** | Creemos que la experiencia debe sentirse segura, confiable y colaborativa. El usuario debe percibir la plataforma como un entorno académico serio, pero a la vez solidario y de apoyo mutuo, no como una red social informal. |

##### Definición de Objetivos

**Business outcomes**
* Fomentar la colaboración y reducir el aislamiento académico entre universidades.
* Contribuir a la disminución de la tasa de deserción estudiantil por fracaso académico.
* Posicionar la plataforma como la red de apoyo estudiantil interuniversitaria líder en el Perú.
* Establecer alianzas estratégicas con universidades para facilitar los procesos de validación.
* Lograr un modelo de negocio sostenible captando el 5% de comisión de las donaciones.
* Fomentar el aprendizaje interuniversitario sincrónico y asincrónico.

**User outcomes**
* Mejorar el rendimiento académico y la comprensión de temas complejos.
* Reducir el estrés y la ansiedad asociados a los desafíos académicos.
* Adquirir nuevas habilidades prácticas y teóricas de forma accesible.
* Ampliar su red de contactos con pares de otras disciplinas y universidades.
* Aumentar su confianza al poder enseñar y validar sus propios conocimientos.
* Generar ingresos económicos extra para los tutores a través de su esfuerzo.

**Features**
* Sistema de registro y verificación de identidad gestionado por un Coordinador.
* Creación de perfiles de estudiante con secciones diferenciadas para "Habilidades para Enseñar" y "Habilidades para Aprender".
* Motor de búsqueda con filtros por habilidad y universidad, con bloqueo de emparejamiento para la misma institución.
* Sistema de solicitudes de intercambio con mensajería personalizada.
* Chat integrado para la coordinación segura entre los estudiantes emparejados.
* Sistema de calificación mutua y reseñas visibles en los perfiles de usuario.
* Integración de API de videollamadas (ej. Agora o Zoom SDK) para el aprendizaje sincrónico.
* Chat interno con soporte para subir archivos (aprendizaje asincrónico).
* Integración de API de pasarela de pagos (ej. Stripe o MercadoPago) para procesar las donaciones voluntarias y retener automáticamente el 5% de comisión.

#### 1.2.2.3. Lean UX Hypothesis Statements

**Hipótesis de Negocio**
* Creemos que al implementar un sistema de registro y verificación automática exclusiva con correos institucionales (".edu.pe") para todos los estudiantes, resultará en una superación de la barrera de desconfianza inicial y un ingreso más ágil sin validación manual, lo que facilitará la adopción de la plataforma; sabremos que esto es cierto cuando el 90% de los nuevos usuarios complete su registro en las primeras 24 horas y la tasa de reportes por cuentas falsas o suplantación sea cercana a 0%. 
* Creemos que al diseñar un modelo de donaciones voluntarias mediante una pasarela de pagos con una comisión del 5%, resultará en un modelo de negocio sostenible y en una comunidad donde los tutores se mantengan motivados, evidenciándose cuando al menos el 60% de las sesiones incluyan una donación y los ingresos cubran los costos operativos al finalizar el primer año. 
* Finalmente, creemos que al implementar un sistema de calificaciones y reseñas mutuas tras cada sesión, resultará en una comunidad basada en la reputación y la meritocracia, incentivando la calidad de las tutorías; sabremos que esto es cierto cuando más del 75% de las sesiones reciban calificaciones de ambas partes y los tutores con promedio superior a 4.5 estrellas obtengan un 30% más de solicitudes y donaciones.

**Hipótesis de Usuario**
* Creemos que al ofrecer un motor de búsqueda con filtros por habilidad y universidad para los estudiantes "aprendices", resultará en la capacidad de encontrar apoyo específico que no hallan en su entorno inmediato, facilitando conexiones más precisas dentro de la plataforma; sabremos que esto es cierto cuando el 70% de las búsquedas con filtros conduzcan a una solicitud de ayuda y el 60% de los nuevos aprendices completen una sesión exitosa en sus primeras dos semanas.
* Creemos que al integrar un sistema de aprendizaje sincrónico (videollamadas incrustadas vía API) y asincrónico (chat para intercambio de materiales), resultará en una mayor retención, comodidad y percepción de seguridad al no depender de enlaces externos vulnerables; sabremos que esto es cierto cuando más del 90% de las tutorías programadas se realicen exclusivamente dentro de la sala virtual y la satisfacción técnica de la llamada alcance una calificación promedio de 4.5/5.
* Creemos que al facilitar conexiones de tutoría interuniversitarias, los estudiantes "aprendices" lograrán mejorar su rendimiento académico en cursos de alta dificultad, fortaleciendo su confianza y comprensión; sabremos que esto es cierto cuando el 75% de los aprendices reporte en encuestas posteriores un aumento significativo en su confianza y dominio del tema. 
* Finalmente, creemos que al ofrecer una plataforma estructurada y monetizable para enseñar, los estudiantes "tutores" podrán desarrollar competencias académicas y blandas mientras generan ingresos extra, lo que incentivará su participación continua; sabremos que esto es cierto cuando el 80% de los tutores activos reporte que enseñar les ayudó a consolidar su conocimiento y cuando el 50% de los tutores recurrentes logre generar al menos una donación mensual.