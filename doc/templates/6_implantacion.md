# FASE DE IMPLANTACIÓN

## Manual técnico

### Información relativa á instalación

* Requirimentos de hardware: 
    
    **Dispositivo Android 7.0 (Nougat) ou superior.**
* Software necesario:
    
    **Sistema Operativo Android. Software para a lectura de pdf e excel, e recomendable Drive**
* Configuración inicial seguridade: devasa, control usuarios, rede:
    
    **Será necesario establecer un usuario administrador (da man do programador). Unha vez establecido na Configuración Remota de Firebase, xa pode iniciar sesión coas credenciais establecidas e crear novos usuarios de maneira independente.**
* Carga inicial de datos na base de datos: 
    
    **A maior parte das escrituras na base de datos faraas o administrador, que será o encargado de crear novos usuarios, subir nóminas, etc. Os usuarios poderán acceder en forma de lectura a algúns destos datos.
    Firebase Cloud Firestore é unha base de datos non SQL na nube, no que se obteñen as actualizacións en tempo real**.
* Usuarios do sistema. Usuarios da aplicación.:
    
    **A aplicación tendrá dous tipos de usuarios: Administrador e Usuario. Dependendo de quen inicie sesión mostrará unha interfaz diferente, permitindo aos administradores acceder a unhas maiores funcionalidades para a xestión empresarial.**
    **Para o mantemento, configuracións (como a de establecer os administradores, etc), melloras ou cambios será necesario un programador ou persoa con coñecementos en Firebase para levar o control dos datos e posibles cambios que a empresa necesite realizar na base de datos ou a nivel funcionamento interno dos datos.**
* Diagrama final de despregue (se hai variacións con respecto ó realizado na anterior fase).

### Información relativa á administración do sistema, é dicir, tarefas que se deberán realizar unha vez que o sistema estea funcionando:
Necesitarase unha persona externa a empresa para dar soporte, resolución de dubidas ou problemas que xurdan por parte de esta.
Esta persoa poderá ser misma mente o programador da aplicación, ou unha persoa con coñecementos de Firebase, que poida resolver tarefas como:

* Firebase Cloud Firestore establece unhas reglas de seguridade para protexer os datos según a configuración establecida. No caso de que se queiran dar ou quitar permisos de acceso aos datos, a empresa deberá contactar co proveedor da aplicación explicando o que desexa, e este explicará os posibles cambios a realizar e posibles riscos que incorre ao cambiar as reglas de seguridade. En caso de ser factible cambiará as reglas de seguridade. 

A continuación mostrase un exemplo do tipo de reglas que se poden establecer para limitar o acceso a todos os datos que almacenemos en Firebase. Para máis información sobre ditas reglas consultar [este enlace.](https://firebase.google.com/docs/rules/rules-behavior?hl=es)


![exemplo reglas](/doc/img/Exemplo_Reglas_Firebase.png)


* Pode darse que sexa necesario cambiar o administrador da empresa, polo que esta deberá poñerse en contacto co proveedor da aplicación para que cambie os administradores da aplicación. Esta soporta ata 3 administradores, que serán modificador en Remote Config de Firebase.

* No caso de incidencias tanto de sistema (accesos non autorizados á BD, etc) como de fallos no software, informarase ao proveedor da aplicación para que solvente ditos problemas o máis rápido posible.

En resumo, a aplicación levará un continuo mantemento e administración por parte do proveedor da aplicación, que mantendrá un contacto periódico coa empresa para verificar que todo segue en correcto funcionamento, e no caso de xurdir algunha incidencia, imprevisto ou idea de mellora, solventalo o antes posible.

### Información relativa ó mantemento do sistema

* Corrixir erros.
    Correxiranse posibles erros non detectados na fase de probas, tanto software como de sistema o máis rápido posible. A empresa deberá notificar unha incidencia explicando o sucedido ao proveedor da aplicación, poñendose en contacto o máis rápido posible.
* Engadir novas funcionalidades.
    Co paso do tempo pode que a empresa demande novas funcionalidades ou melloras das existentes, polo que se comunicará o desexado para engadir estas novas funcionalidades á aplicación, garantizando que esta cubrirá todas as necesidades demandadas.
* Adaptación por actualizacións de software e/ou hardware.
    Conforme se vaian realizando **melloras significativas **na aplicación, instalaranse as novas actualizacións na empresa para que poidan comezar a usala cos novos funcionamentos e melloras.
## Xestión de incidencias

Poden ser incidencias de dous tipos: de sistema (accesos non autorizados á BD, etc) ou de fallos no software.
Para calquer tipo de incidencia podes contactar co proveedor da aplicación a través de [**este enlace**](https://gitlab.iessanclemente.net/damo/a19lidialf/-/issues/new), especificando o problema co que te atopaches. Este será resolto o antes posible.

Tamén podes contactar directamente a través do correo electrónico _lidialoureirofacal@gmail.com_ co asunto **Incidencia Alea**, especificando un teléfono ou e-mail de contacto, e poñeremonos en contacto o antes posible.


## Protección de datos de carácter persoal
Toda a información que contén a Base de Datos pertence aos usuarios, protexidos pola [**Lei de Protección de Datos**](https://www.boe.es/buscar/act.php?id=BOE-A-2018-16673).

## Manual de usuario

* [Manual de instalación](/documentacion/MANUAL_INSTALACIÓN.pdf)

A aplicación pretende ser o máis intuitiva posible, polo que non se fai estritamente necesaria unha formación específica para o seu uso.    
No caso de que fora necesario, proporcionase un manual de uso nos seguintes enlaces:
* [Manual de uso **Alea App**](/documentacion/MANUAL_USO_ALEA.pdf).
* [Manual de uso **Alea Scanner App**](/documentacion/MANUAL_USO_ALEASCANNER.pdf)
