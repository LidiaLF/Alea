# FASE DE PLANIFICACIÓN DO PROXECTO

## Obxectivos do proxecto

## Guía de planificación do proxecto

### Metodoloxía
Adaptación de metodoloxías áxiles a unha persoa.

### Fases planificadas

Descríbense as fases en que se divide o proxecto e as tarefas que se han levar a cabo en cada unha destas fases.
Pódense indicar os recursos materiais e humanos asociados a cada tarefa ou, se son os mesmos, de maneira máis xeral.

En este caso centrarase na planificación do proxecto, tendo en conta que o desenvolvemento foi realizado por unha única persoa, polo que os **Recursos Humanos** en todos os apartados serei eu mesma.

#### Fase 1: Estudo de necesidades e modelo de negocio
##### Tarefa 1: Idea do proxecto

Descrición: Definición da idea do proxecto e necesidades a cubrir, mediante unha reunión con algún responsable da empresa, que nos describa que é o que demandan.

Estudaremos tamén, se hai aplicacións que cubran as necesidades demandadas, o sector ao que nos vamos a dirixir, comportamento, etc. establecendo así o valor engadido que pode ofrecer a nosa aplicación, utilidade e obxetivos que pretendemos alcanzar con esta.

Recursos hardware/software: Blog de notas para tomar apuntes sobre o que quere e necesita a empresa e internet para buscar a información necesaria.

Duración: 5 días.

##### Tarefa 2: Definición e diseño do proxecto

Descrición: Definición da idea do proxecto e necesidades a cubrir (Que vamos a realizar e como o vamos a realizar).
Aquí realizaremos ideas e xustificacións de posibles deseños front-End, estudos sobre a linguaxe a utilizar, base de datos e recursos necesarios para a realización e futura posta en marcha.

Debemos definir ao detalle todas as características e funcionalidades que a aplicación debe poseer para alcanzar a meta desexada, e dicir, establecer un primeiro diseño tanto da parte funcional como visual, dos que partiremos nas fases posteriores.

Neste caso seleccionamos un IDE (Android Studio), linguaxe de programación Android integrando ferramentas multiplataforma proporcionadas por Firebase, entre outras.
Definimos que os dispositivos nos que correrá a aplicación teñen que ter unha versión Nougat ou superior, abarcando así a máis da metade dos dispositivos actualmente utilizados en Android.


![Api](/doc/img/apiAndroid.png)


Recursos hardware/software: Dispositivo con conexión a internet para a busqueda de ideas e creacións de diseños (neste caso, os deseños foron realizados co programa [*Proto.io*](https://proto.io/)) e software de ofimática para describir as funcionalidades da aplicación.

Duración: 2 semanas.


##### Tarefa 3: Definición do modelo de negocio e presuposto

Descrición: Calcularemos un custo estimado do que pode custar a realización do proxecto, partindo do estudo realizado nas tarefas anteriores, e dicir, o presuposto dependerá do alcance definido anteriormente, a elección dos recursos hardware e software necesarios, viabilidade, etc.

Recursos hardware/software: Internet para estudar os posibles custos do requerido para a realización do proxecto e Excel para plasmar os custos que poden supoñer, o custo que vai supoñer para o programador e o custo que vai supoñer para a empresa demandante, así como todo o orzamento necesario.

Duración: 3 días.



#### Fase 2: Desenvolvemento da aplicación
##### Tarefa 1: Programación da aplicación con fases de testeo

Descrición: Unha vez rematadas todas as tarefas anteriores, debemos comezar creando o proxecto en Android Studio seguindo os deseños creados anteriormente.

Primeiro crearemos un proxecto Firebase, que nos proporcionará un JSON, librerías e dependencias necesarias para enlazalo co noso proxecto e poder utilizar as ferramentas que nos ofrece. Configuraremos tamén as reglas de acceso de seguridade aos datos pertencentes a Alea App que almacenaremos.

Unha vez configurado Firebase, podemos comezar a programar tanto o front-end como o back-end da aplicación, base de datos, esquemas e diagramas, etc. Todo isto debe alternarse con varias fases de testeo, o que nos permite detectar erros mais fácilmente e correxilos antes de continuar programando, o que nos permitirá obter un código de calidade.   

Aqui tamén nos reuniremos periódicamente co cliente, para mostrarlle o avance da aplicación, funcionalidades e que nos dea o visto bó para seguir adiante segundo o planificado, ou se prefire que corrixamos ou modifiquemos algunha característica que non sexa completamente do seu agrado.

Recursos hardware/software: Ordenador, Android Studio para o desenvolvemento, Firebase xunto coas funcionalidades que nos proporciona e un dispositivo móbil ou emulador para as probas.

Duración: 3-4 meses.

##### Tarefa 1: Proba de erros

Descrición: Unha vez rematada completamente a tarefa anterior, debemos someter á aplicación a unha proba de erros xeral, levandoa a un análisis extremo.

Instalaremos a aplicación en diferentes dispositivos de persoas alleas ao proxecto, con versións Android distintas, que forzarán todas as posibilidades que ofrece a aplicación, cubrindo un documento de reporte donde indiquen que dispositivo utilizaron, versión Android, acción realizada donde xorde o problema e descrición do problema.

Correxiremos os erros reportados e voltaremos a facer unha nova proba de erros, ata que non se detecte ningún. 

Recursos hardware/software: Android Studio e varios dispositivos móbiles.

Recursos humanos: A maiores, podemos considerar diferentes usuarios axenos á aplicación que a proben e nos reporten os posibles erros, bugs ou suxerencias.

Duración: 2-3 semanas (Dependendo da cantidades de reportes xurdidos)


#### Fase 2: Implantación
##### Tarefa 1: Instalación da aplicación

Descrición: Unha vez obtido unha aplicación completa e limpa de erros é o momento de instalala.
Instalaremos a aplicación nos distintos dispositivos da empresa, xunto cos manuais de uso e unha explicación xeral.
Debemos darlle un contacto para que nos comuniquen calquer dúbida, suxerencia ou erro que poidan ter no futuro.

Recursos hardware/software: AleaApp.apk, AleaScanner.apk, documetos de manual de uso, dispositivos nos que será instalada a aplicación.

Recursos humanos: podemos considerar como recursos humanos (non remunerados), os usuarios que usarán e instalarán a aplicación.

Duración: 1 día.

##### Tarefa 2: Promoción

Descrición: Publicitaremos a implantación de esta nova aplicación a través dos canles seleccionados, para darnos a coñecer como programadores de aplicacións a medida para contornos empresariais.

Recursos hardware/software: Redes sociais, creación de páxina web, etc.

Duración: 2-3 días.

##### Tarefa 3: Soporte e mantemento

Descrición: Esta tarefa extenderase ao largo do tempo, dando soporte a todo o necesario por parte da empresa, por exemplo, en caso de que a empresa cambie de administrador, deberá comunicárnolo para que o editemos, xa que en aspectos internos dos datos da aplicación, só terá acceso o programador.

A empresa terá unha contínua comunicación con nos, xa que nos debe reportar calquer erro, bug ou suxerencia para que nos o melloremos, ao mesmo tempo que debemos revisar periódicamente que todo funcione correctamente.
Co tempo poderá darse que a mesma empresa necesite engadir novas funcionalidades, polo que nos faremos cargo da implantación da nova funcionalidade.

Como creadores de unha aplicación que utilizará unha empresa, debemos facernos responsables de todos os casos que poidan xurdir derivados da utilización da mesma, procurar unha mellora contínua do producto, tanto externa como interna, lanzando novas actualizacións que permitan mellorar a experiencia dos usuarios.

Recursos hardware/software:  Ordenador, smartphone, Firebase, Android Studio, programas de ofimática.

Duración: Indeterminada. A duración desta fase será proporcional ao tempo en que a empresa utilice os nosos servizos.



### Diagrama de Gantt

Un diagrama de Gantt é unha representación gráfica da secuenciación que tes que seguir para realizar as tarefas planificadas.

![diagramaGantt](/doc/img/Gantt_Alea.png)

## Orzamento

O orzamento do proxecto será a suma do importe dos materiais que necesites para realizar o proxecto máis o importe que corresponde ao traballo realizado.

Tendo en conta que o proxecto se realizou dende a vivienda particular, non se necesitaron alugueres, nin contratos de subministros, polo que non os teremos en conta a hora de plasmalos nas taboas seguintes, xa que únicamente se necesitará un gasto mínimo de uso do xa contratado pola familia, polo que só se consumiría un porcentaxe dos custos. A continuación plasmaranse ditos aspectos:

- Gasto de electricidade. O precio medio da electricidade no momento de realizar o estudo é de 0.11253 €/kWh.
- Tarifa de internet 56€/mensuais aproximadamente, incluindo fibra e datos móbiles.Non é necesario a instalación xa que xa dispoñemos dela.

- Para o cálculo, os gastos de equipos informáticos plasmaranse únicamente na taboa de orzamento por partidas de inversión/gasto, xa que, aínda que se utiliza en todas as fases da taboa de orzamento por actividade, é un inversión inicial única.
- Calcularemos o salario dun traballador sobre uns 10€/h.
- Estableceremos algún gasto en recursos materiais para ter un fondo de previsión ante a necesidade de algún material para realizar as tarefas.
- Non teremos en conta para os cálculos o apartado _Soporte e mantemento_, xa que esta é unha actividade ao longo do tempo, que dependerá do tempo que o cliente utilice a nosa aplicación, así como das necesidades que irán aparecendo, polo que este cálculo se realizará independentemente no momento en que se realice algunha mellora significativa. Estableceremos aproximadamente un custo de 600€/ano para o cliente.

O maior custo no proxecto case sempre corresponde ás persoas, polo que é importante controlar o número de horas que se invisten en cada actividade para que non se nos desequilibre o orzamento. Tamén hai que coidar as subcontratacións; convén que traballen cun orzamento establecido.

 A continuación preséntanse dúas opción de táboa para facilitar a creación do orzamento do proxecto:

### Orzamento por actividade

| ACTIVIDADE | DURACIÓN | CUSTO (EUROS) | | CUSTO TOTAL ACTIVIDADE |
|--|--|--|--|--|
|            |          | PERSOAS|RECURSOS MATERIAIS|
| Estudo de necesidades e modelo de negocio | 22 días | 1.760€ | 100€ | 1.860€ |
| Desenvolvemento do proxecto| 145 días (aprox.)| 11.600€| 400€ | 12.000€ |
| Implantación| 4 días | 320€ | 100€ | 420€ |
| Soporte e mantemento*| indeterminada | - | - | - |

| TOTAL | PROXECTO |
| -- | -- |
| 1.368h | **14.280€** |

*_600€/anuais + posibles incrementos por actividade ou implantación de novas funcionalidades que necesiten un custo a maiores._

### Orzamento por partidas de inversión / gasto

| CONCEPTO | IMPORTE|
|--|--|
|**A) INVERSIÓNS**
|Gastos de establecemento e gastos de constitución|100€ tramitación alta de autónomos|
|Total inmobilizacións inmateriais|0€ ([cuota de Firebase para pequenos proxectos = 0€](https://firebase.google.com/pricing?hl=es))|
|Terreos| 0€|
|Construcións| 0€|
|Instalacións técnicas| 0€|
|Maquinaria| 0€|
|Ferramentas| 0€|
|Mobiliario e instalacións| 0€|
|Equipos informáticos| 1.300€ PC portátil + 110€ smartphone|
|Elementos de transporte| 0€|
|Outro inmobilizado material| 0€|
|Total inmobilizacións materiais| 0€|
|Outros gastos a distribuír en varios exercicios| 0€|
|**TOTAL INVERSIÓNS:**| **1600€**|
|**B) GASTOS**
|Compras de materiais| 0€|
|Arrendamentos| 0€|
|Publicidade, propaganda e relacións públicas| 0€ (publicidade por redes sociais)|
|Persoal| 0€|
|Reparacións e conservación| 100€/ano|
|Servizos de profesionais independentes| 0€|
|Outros gastos xerais| 0€|
|Gastos financeiros| 0€|
|Amortizacións| 160€/ano|
|Gastos de xestión e administración| 200€/ano|
|**TOTAL GASTOS:**| **460€/ano**|

|TOTAL ORZAMENTO POR PARTIDA DE INVERSIÓN:|
|--|
| 1.600€ fixos + 460€/ano. |

|TOTAL ORZAMENTO FIXO:| ORZAMENTO ANUAL: | TOTAL APROXIMADO: |
|--|--|--|
| **15.880€**| **460€ + 600€ mantemento**  | 15.880€ INICIAIS + 1.100€/anuais aproximadamente (con posibles incrementos por implantación de novas funcionalidades que supoñan un gasto a maiores)|

### WEBGRAFÍA

Guía para a elaboración de proyectos. Gobierno Vasco.
<https://www.pluralismoyconvivencia.es/upload/19/71/guia_elaboracion_proyectos_c.pdf>  (páxina 49 e seguintes)
