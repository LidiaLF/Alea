# REQUIRIMENTOS DO SISTEMA

Este documento describe os requirimentos para **_Alea App_** especificando que funcionalidade ofrecerá e de que xeito.

## Descrición Xeral

O proxecto consistirá nunha aplicación que permita ter un maior control sobre algúns aspectos das tarefas administrativas que se poden dar no entorno dunha empresa, ao mesmo tempo que ofrece unha plataforma persoal para cada empregado.

A principal funcionalidade que pretende cubrir é a de que cada empregado poida realizar ás fichaxes de entrada, saída e descansos de maneira autónoma dende o seu smartphone persoal, tanto de maneira física na entrada da oficina co Scanner, como a través da ubicación GPS, no caso de que o empregado teña que realizar tarefas derivadas do seu posto de traballo nun contexto externo.

Unha vez cuberta esta necesidade principal, tamén pretende dar soporte noutros aspectos fundamentais como os descritos nos seguintes apartados.



## Funcionalidades

A continuación detallaranse as funcionalidades máis básicas de **Alea App**, estas dependerán do tipo de usuario que acceda á aplicación.

Funcionalidades para un empregado:

**1.** Rexistro dos fichaxes de entrada, saída, inicio do descanso e fin do descanso.

**2.** Creación de eventos recordatorios no calendario. Aqueles que marque como "importantes" visualizaranse na pantalla principal da aplicación.

**3.** Visualización e descarga das nóminas mensuais enviadas polo administrador. O empregado terá un listado das suas últimas nóminas, ás que pode acceder cando desexe.

**4.** Listado de empregados da empresa, cos que se poderá comunicar mediante e-mail ou teléfono.

**5.** Configuración de algúns datos personais, como a foto de perfil, e número de teléfono.

**6.** Cambio de idioma da aplicación.



A maiores das anteriores, a un empregado administrador engadiranselle as seguintes funcionalidades:

 **1.** Rexistro de novos empregados, mediante un formulario no que se especificarán os datos do novo empregado, xornada laboral e a asignación de un correo corporativo único para cada empregado. Unha vez gardados estes datos na BD, o novo empregado recibirá un e-mail ao seu correo para o cambio da contrasinal de acceso a aplicación.

 **2.** Modificación dos datos dos empregados, sendo irremplazable o e-mail.

 **3.** Eliminar empregados, expecificando o motivo.
 
 **4.** Os empregados eliminados, almacenaranse nun apartado de histórico de empregados, gardando tanto os fichaxes dos últimos 4 anos, como unha ficha expecificando a data de alta, data de baixa, motivo e número de teléfono.
 Unha vez dado de baixa, o empregado non tendá acceso á aplicación.
 Tamén terá un botón "alta" por si queremos volver a contratalo, o que permitiría o acceso de novo á aplicación.

 **5.** Subida de nóminas dende o dispositivo, permitindonos seleccionar as nóminas de cada empregado á vez, e envialas correspondentemente a cada un. A subida de nóminas debe realizarse antes do remáte do mes correspondente.

 **6.** Descarga dos fichaxes de cada empregado, por mes e ano, volcando estes datos nun excel detallado.

  

## Requirimentos non funcionais

Necesitarase conexión a internet para un primeiro acceso á aplicación, actualización dos datos e visualización de datos actualizados.

Firebase permite que, no caso de que non teñamos conexión á rede, os datos queden almacenados na caché temporalmente, ata que a situación da rede se resolva. Polo que de estar a realizar algunha tarefa de envío ou recepción de datos contra algún servizo de Firebase, os datos non se perderían. Estes serán commiteados no momento en que se recupere a conexión.

Sen conexión a internet a aplicación proporcionanos un acceso limitado aos datos, xa que se visualizarán os últimos datos obtidos no momento da última conexión, pero permitindo o uso das funcionalidades máis necesarias, como son, neste caso, as fichaxes. 

## Tipos de usuarios

Os usuarios que poderán acceder ó noso sistema serán aqueles que formen parte do *Grupo Alea*, e teñan asignadas unhas credenciais corporativas, únicas e intransferibles (un usuario que non estea dado de alta como empregado da empresa non poderá acceder á aplicación).
Poderán diferenciarse polos permisos sobre os datos, pantallas que se lles amosan, operacións que poden levar a cabo, etc.

* **Empregado:**

    - Fichar a entrada, saída e descansos do traballo, dende a aplicación.
    - Fichar a entrada, saída e descansos do traballo por GPS.
    - Engadir eventos detallados no seu calendario persoal, dos cales, os importantes, se engadirán á pantalla de inicio.
    - Visualizar e descargar as nóminas enviadas polo administrador.
    - Enviar e-mails e realizar chamadas aos empregados pertencentes á empresa.
    - Cambiar aspectos persoais do perfil de usuario, como a foto, número de teléfono, etc.



* **Administrador:**
      Poderá realizar as mesmas tarefas que un _Empregado_, pero ademáis pode: 
      
    - Dar de alta a un novo empregado, cubrindo un formulario donde se especificará, entre outros, aspectos como o tipo de xornada.
    - Modificar datos dos empregados.
    - Dar de baixa aos empregados, especificando o motivo da baixa.
    - Subir nóminas mensuais á plataforma, para cada empregado.
    - Descargar as fichaxes mensuais ou anuais, por cada empregado e volcar a información nun excel.
    - Acceder ao histórico de empregados, donde se mostrarán antigos empregados, dos que poder descargar as fichaxes dos últimos 4 anos, visualizar unha tarxeta cos datos do empregado e un botón para, en caso de que se desexe, volver a dalo de alta na empresa.


## Avaliación da viabilidade técnica do proxecto

### Hardware requirido

Para o desenvolvemento da aplicación:
- Un ordenador por parte do programador.
- Un ou varios dispositivos móbiles para as probas.

Para a implantación da aplicación:
- Unha tablet (ou dispositivos similar) para a instalación do _Scanner._ 
- Un dispositivos móbil (smartphone) por cada empregado, donde se instalará _Alea App._


### Software

Para o desenvolvemento da aplicación:
- Utilización de Android Studio na súa última versión, valendonos das ventaxas que proporciona o IDE, así como da creación dos emuladores para as probas (emulador de API igual ou superior á 24).
- Linguaxe de programación JAVA.
- Uso das ferramentas aportadas por Firebase que permiten a sincronización dos datos en tempo real, como o servizo de autentificación para o login(_Firebase Auth_); o servizo de almacenamento de datos na nube (_Cloud Firestore BD NoSQL_); o servizo de cargas e descargas de archivos xerados polo usuario, permitindo o almacenamento de diversos tipos de arquivos na nube (_Storage_); e o servizo de configuración remota, que, neste caso, permitenos definir e cambiar os administradores de maneira remota (_Remote Config_)

Para a implantación da aplicación:
- Necesitase que o dispositivo no que se instalen as aplicacións teña unha API igual ou superior á 24 (Android Nougat 7.0).
- Recomendase ter instalada a última versión de Google Drive e Docs Viewer. No caso de non dispoñer destas, a Alea app dalle a posibilidade de descargalas de maneira gratuíta redirixindoos a PlayStore.

## Interfaces 

Esta aplicación pretende comunicarse co usuario de maneira sinxela e o máis intuitiva posible, a través de pantallas propias da aplicación, que lle mostrarán os datos ao usuario guiandoo pola mesma.

Podemos ver interfaces de usuario que interactúan nesta aplicación no seguinte plano de páxina:
![Plano de páxina.](doc/img/AleaWireframe.png)

## Análise de riscos e interesados

Un dos posibles riscos cos que nos podemos atopar é ,que a hora da fichaxe, algún empregado tentase de fichar de maneira fraudulenta, ou que non poidese fichar presencialmente na empresa porque está a realizar algunha tarefa relacionada co seu posto, pero fora da oficina.

Para darlle solución a estes posibles problemas, implementaríase, como mellora futura, a fichaxe por GPS, o que garantizaría que cada fichaxe o realizaría un determinado empregado nunha determinada localización, sabendo se este o realiza dende a casa, o traballo ou un bar.

## Actividades

O proxecto constará de 3 fases principais, as cales a súa vez se dividirán en varias fases:

1. **Planificación:**
      Realizarase unha idea do proxecto, estudando ás necesidades que se pretenden cubrir, como se intentarán solventar, lenguaxe no que desenvolveremos a aplicación, base de datos, tecnoloxías a utilizar e diseño de Wireframes.
    
2. **Desenvolvemento da aplicación:**
      Desenvolverase tanto a funcionalidade como interfaz da aplicación, creación da base de datos, modelo E/R, creación de diagrama de clases, probas e corrección de erros.

3. **Fase final:**
      Implantarase a aplicación para que os usuarios a poidan empregar. Seguiranse a observar posibles erros que poidan aparecer e implementaranse posibles melloras futuras que vaian xurdindo. 


## Melloras futuras

- **Calendario** con eventos comúns, no que un usuario poida programar un evento no calendario de todos os usuarios.
- Implementación dun **chat** no apartado "Grupo Alea", que melloraría as comunicacións entre os empregados.
- Servizo de **notificacións** e recordatorios de tarefas importantes.
- Implementación dun apartado para **solicitar vacacións** para cada empregado. 
- Portar aplicación a IOS para dar soporte a dispositivos Apple, mediante **j2objc** de Google. 
