la instantánea de los cambios
Lo mas reciente arriba "HEAD"
Lo mas antiguo en lo profundo del fondo.
(#-) : apertura nuevo tema o subtema, (-#) : cierre nuevo tema o subtema, (#) comentario, (:) explicacion de comando, (->>>) cursor 


```json DICCIONARIO DE EXPERIENCIAS practicas    "ENTENDIENDO GIT"
{
  {"comandos FIFO": 04/08/2023"   *--------# Start (HEAD):   

          

->>>


git commit   -m "docs(GIT): :memo: Descripcion corta inperative"   -m "Drecripcion longer"   -m "List any breacking changes or issues closed"         
                    :pre-commit(antes de) "espacificacion conventionals commits"         
# :35) 31/08/2023 , hora de inicio: --:-- am, hora de fin: --:-- am,  sesion de estudio/practica: GIT, Descripcion:   # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
git commit -m "My head line" -m "My content line."   : Si sólo quieres, por ejemplo, una línea de encabezamiento y una de contenido, puedes utilizar Fuente: https://www.iteramos.com/pregunta/6513/anadir-salto-de-linea-a-git-commit--m-desde-la-linea-de-comandos 
git commit -m $'first line\nsecond line'             : Insertando linea de espaciado en un commit descripcion
git commit  -m "docs(GIT): :memo: Curso Git - OpenBootcamp" -m '#video: 4 Repositorio local 2 - Curso Git - OpenBootcamp, seccion video 2:14:09 / 2:20:47'               : Insertando linea de espaciado en un commit descripcion
                                                      #
                                                      #
                                                      docs(GIT): :memo: Curso Git - OpenBootcamp

                                                      #video: 4 Repositorio local 2 - Curso Git - OpenBootcamp, seccion video 2:14:09 / 2:20:47
                                                      #
                                                      #
                                                      #ejemplo de commit mas detallado en sus seis partes
                                                      #
docs(GIT): :memo: Descripcion corta inperative

Drecripcion longer

List any breacking changes or issues closed                                                      
                                                      #
                                                      #en linea de comandos seria:
git commit  -m "docs(GIT): :memo: Descripcion corta inperative" -m 'Drecripcion longer' -m 'List any breacking changes or issues closed'               
                                                      : Insertando linea de espaciado en un commit descripcion                                                      
                                                      #gerando cambio para probar
                                                      # 1 file changed, 1 insertion(+)
                                                      # test OK, aparentemente igual
                                                      # testear otra forma
                                                      #
git commit -m "docs(GIT): :memo: Descripcion corta inperative 
Drecripcion longer 

List any breacking changes or issues closed"           
                                                      #    
                                                      #  1 file changed, 14 insertions(+)
                                                      # test ok
                                                      #
                                                      # Este es elcommit "antes de el contenido de arriba (pre commit)"  , commit: tipo doc, repaso dia anterior 
git commit   -m "docs(GIT): :memo: Descripcion corta inperative"   -m "Drecripcion longer"   -m "List any breacking changes or issues closed"         
                                                                    #          
                                                                    # or
                                                                    #
git commit -m "docs(GIT): :memo: Descripcion corta inperative 
Drecripcion longer 

List any breacking changes or issues closed"               
                                                      #
                                                      # para que resulte asi:
                                                      #
docs(GIT): :memo: Curso Git - OpenBootcamp

#video: 4 Repositorio local 2 - Curso Git - OpenBootcamp, seccion video 2:14:09 / 2:20:47
                                                      #
                                                      #

git commit -m "first line\nsecond line\ntercera linea"
# :34) 30/08/2023 , hora de inicio: 07:00 am, hora de fin: 08:00 am,  sesion de estudio/practica: GIT, Descripcion:   # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
                  #haciendo un fork
                  # primer paso    :  crear el fork.
                  # segundo paso   : obtener el fork.  
                  # el tercero enviar mis cambios al repositorio
                  # el cuarto paso va a ser crearme la PULL REQUEST PR (open pull request) 
                  #ejemplo solicitud de pull request:
                  # mensaje es necesario crearme ficheros README.md
                  # create pull request
                  # despues el que tiene permisos sobre todo el reposositorio, puedo ver todas las pull request 
                  # veria el commit de quien hiso la pull request 
                  # vale como me parece bien lo que ha hecho este señor : creo el archivo README.md
                  #le doy al boton merge pul request, antes de darle click veo que no hay ningun fichero readme.md en mi repositorio
                  #confirmo lo que estoy haciendo otro boton, pull request close 
                  # si voy a pull reques ya no me pone que tenga alguna otra PR abierta 
                  # puedo ponerle close , para ver todas las que estan cerradas(PR) , filtro de busqueda.
                  #ahora si me voy al repositorio me aparece el fichero README.md quien fue creado en un commit por otro programador a el cual yo le he permitido, al hacer un merge de su coomit en mi repositorio, claro despues de revisar su codigo y asegurarme que no rompa el codigo.
                  #Si miro mi historial de commits pone:
                  # merge.vroman "ha creado un commit para hacer el merge." y ademas me pone verificado con firma digital, cosas que garantizan la autenticidad.
                  # este work flow es super tipico en el desarroyo tanto para empresas como para proyectos Open source.
                  #
                  #Git permete que alteremos el comportamiento de lo que hace (con los hooks "son script ejecutables ya sea en repo local o remoto").
                  # lo hace en local site o server site (remoto)
                  # hay una cositas que se llaman HOOKs estos se ejecutan en ciertos momentos 
                  # estan escritos en un leguaje de programacion que nosotros queramos. 
                  # pero que se tiene que poder ejecutar en nuestro Sistema Operativo
                  # en windows: ficheros .cmd, .ps (power shell) 
                  # en linux fricheros: SH, PY, perl, PHP 
                  # los hook estan dentro de mi repo local en:
                  # .git/hooks
ls                 : veo todo lo que tiene adentro  
                   # y todos son .sample, lo que evita que se dispare automaticamente.
                   # en que orden se ejecutan: primero 
                   #hook de pre commts            
                   #el siguiente es prepare-commit.smg  # elimina una de las lineas del rm
                   #commit msg : manipula las cosas el mensaje, cuando guardo es que este hook se dispara.
git commit -s fix3.txt  : -s mete la linea de firma de quien esta haciendo el commit, cambio firmado por mi, sos vos realmente el autor de ese codigo 
                    #hook post-commit usualmente para enviar correos electronicos, pero es absurdo que a mi me envie un email de mi propio commit
                    #post checkout se ejecuta despues de hacer un checkout
                    # el pre rebase, al cambiar de rama
                    #
                    #Ahora los que se ejecutan del lado del servidor SERVER SITE
                    #los que ejecuta el servidor cuando ocurre algo son: 
                    #pre-receiver : antes de recibir los datos.
                    #update       : cuando se reciven los datos
                    #POST-RECEIVE : cuando se tienen los datos se ejecuta, super comun para enviar por correo electronico una lista de correos cuando se hace un cambio
ssh 185.142.62.4    : este es un servidor de verdad 
                    #username
                    #password                 
git --bare init repo-central  : he inicializado un repositorio en este servidor remoto del tipo bare                
                    #trabajaremos con este repo
git clone git+ssh://vroman@185.142.62.4:/home/vroman/repo-central       : equipo local
password            #me pide la cntraseña de su servidor                         
                    # y lo hemos clonado aqui en repo central
                    #ahora quiero que cada vez que halla un cambion el servidor remoto de la repo 
                    #me mande un correo a la cuenta de email o lo pudes configurar para que publique en tus redes sociales con las apis tuiter,face,etc.
                    #lo hago un un HOOk que se llama 
                    #post-receive
                    # lo voy a crear
                    # me creo el post receiber con el editor nano
                    # hago copi y paste es un script vastante grande.
                    #le doy los permisos de ejecucion a este script 
chmod                     
nano config         # configuro hook , email 
                    # esto tiene que funcionar
                    #video: 4 Repositorio local 2 - Curso Git - OpenBootcamp 2:14:09 / 2:20:47
                    #este hook se va a ejecutar cuando yo haga un push
git push origin master : voy a enviar a mi servidor mi rama master 
                    # me pide la clave
                    #recapitulacion
                    #comandos avanzados: 
git reset 
git blame 
git bisect
git stash           : para parar el trabajo actual                    
git branch           : crear ramas
git checkout        : crear ramas 
git merge             : fusionar ramas
git rebase            : fusionar ramas 
cherry picking        : fuaionar cosas concretas no ramas completas 
work flow local       : Metodo: bajarme los cambios, hacer mis cambios, revisar mis cambios, comitear a mi repositorio local los cambios 
working flow work     : tipico en empresas  y proyectos Open Source su metodo:
                      #clonar un repositorio de un tercero utilizando github (hacer un FORK)
                      : bajarnos nuestro repositorio clonandolo 
                      #hacer nuestros cambios 
                      #hacer un commit
                      #hacer un push 
                      # y luego abrir un pull request (PR)
                      #mainteiner desarrollador autorizado podra aplicar esos cambios aceptando el pull request, es quien puede hacer el meger de los pull request en el repo original.
                      # y como esos cambios se integran mediante un merge en la rama final de desarrollo de este repositorio
                      #por ultimo hemos visto los git hooks 
                      # nos permiten alterar el comportamiento tanto local como server sate de git 
                      #debes profundizar por vuestra cuenta en esto para poder hacer comandos mas potentes
                      #hemos terminado por ahora esta sesion 
                      #video: 4 Repositorio local 2 - Curso Git - OpenBootcamp 2:14:09 / 2:20:47                      
                      #
                      # este es el commit de esta session de estudio:
                      #
docs(GIT): :memo: Curso Git - OpenBootcamp

#video: 4 Repositorio local 2 - Curso Git - OpenBootcamp, seccion video 2:14:09 / 2:20:47
                      #
                      #
# Este es elcommit "antes de el contenido de arriba (pre commit)"  
# :33) 29/08/2023 , hora de inicio: 8:00 pm, hora de fin: 9:00 pm,  sesion de estudio/practica: GIT, Descripcion:   # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
                            PRE COMMT:
                            Cómo crear tu PERFIL de GITHUB desde cero *muy sencillo* (Curso de Github) #3
                            Agradecimientos al Autor: canal de youtube "Programa Con Jorge."
                            link: https://www.youtube.com/watch?v=nrMSM3NleUM
                            usando conventional commit como seria este commit:
                            #commit 1
1.Tipo: docs                 :o chore(otros cambios que no modifican src ni archivos de pruebas).
2.Scope: GIT                 :"new scope GIT" (de tematica, o area a tratar).
3.gitmoji: :memo:            :Agregar o actualizar documentación. "los commits siguientes pueden ser(en proceso)"
4.crear tu PERFIL de GITHUB  :write a short, imperactive tense descrition of the change. "los commits siguientes pueden ser(en proceso) o detallar tematica nueva dependiente de este -new tip de la tematica"
5.Cómo crear tu PERFIL de GITHUB desde cero *muy sencillo* (Curso de Github) #3          "los commits siguientes pueden ser(en proceso) o detallar tematica nueva dependiente de este -new tip de la tematica"                 
                             :provide a longer description of the change.
6.link. https://www.youtube.com/watch?v=nrMSM3NleUM                             
                            cuando ejecutas el commit 
                            1. Si el video es corto, enseñansa es corta  cuando lo termines.
                            2. Si el video es largo y requieres varias sessiones o dias de trabajo y estudio, creas sub-commit, es hacer el mismo commit indicando el prograso del mismo (el avence, por que parte del video vaz) tiempo de estudio, lineas de redaccion, pausas de la actividad: pueden ser variables que te direccionen a hacer un sub-commit de una commit no terminado.
                            3. cuando no hacer commit
                            # commit 2, segundo commit de ejemplo para este estudio POST COMMIT a lo que ya se ha avanzado sin tener un commit definido:
                            #En que momento debo realizar un commit en git
1.Tipo: docs                 :o chore(otros cambios que no modifican src ni archivos de pruebas).
2.Scope: GIT                 :"new scope GIT" (de tematica, o area a tratar).
3.gitmoji: :memo:            :Agregar o actualizar documentación. "los commits siguientes pueden ser(en proceso)"
4.Cuando hacer un commit    :write a short, imperactive tense descrition of the change. "los commits siguientes pueden ser(en proceso) o detallar tematica nueva dependiente de este -new tip de la tematica"
5.¿En que momento debo realizar un commit en git?
                             :provide a longer description of the change.    :"los commits siguientes pueden ser(en proceso) o detallar tematica nueva dependiente de este -new tip de la tematica"                 
6.link: https://es.stackoverflow.com/questions/4144/en-que-momento-debo-realizar-un-commit-en-git
                            #-
                            nuevas lecturas: nuevos commits:  3. cuando no hacer commit
                            ¿En que momento debo realizar un commit en git? (https://es.stackoverflow.com/questions/4144/en-que-momento-debo-realizar-un-commit-en-git)
                            Sobre la elaboración de salchichas (https://sethrobertson.github.io/GitBestPractices/)
                            A algunas personas les gusta ocultar la fabricación de salchichas¹ , o en otras palabras pretender ante el mundo exterior que sus confirmaciones surgieron completamente formadas y perfectamente en su repositorio de git. Ciertos grandes proyectos públicos exigen esto, otros exigen concentrar todo el trabajo en un gran compromiso y a otros no les importa.
                            Una buena razón para ocultar la elaboración de salchichas es si cree que puede estar seleccionando muchos compromisos (aunque esto también suele ser una señal de un mal flujo de trabajo). Tener una o una pequeña cantidad de confirmaciones para elegir es mucho más fácil que tener que encontrar una confirmación aquí, otra allá y la mitad de esta otra. Este último enfoque hace que el problema sea mucho más difícil y normalmente dará lugar a conflictos de fusión cuando finalmente se fusione la rama donante.
                            Ejemplo de elaboracion de salchicha, repo de un documento:
                            https://github.com/SethRobertson/GitBestPractices/commit/2dfa39600061a3ef6d48f721ea8e442eeb51cddf
                            #commit 3 de ejemplo, descriocion  de varias teaticas
                            5 pasos para escribir mejores mensajes de confirmación link: https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/
                            #
                            Resumamos las pautas sugeridas:
                            1.Capitalización y puntuación: escriba en mayúscula la primera palabra y no termine en puntuación. Si utiliza confirmaciones convencionales, recuerde usar todo en minúsculas.
                            2.Estado de ánimo: utilice el modo imperativo en la línea de asunto. Ejemplo – Add fix for dark mode toggle state. El modo imperativo da el tono con el que estás dando una orden o petición.
                            3.Tipo de confirmación: especifique el tipo de confirmación. Se recomienda y puede ser aún más beneficioso tener un conjunto consistente de palabras para describir sus cambios. Ejemplo: corrección de errores, actualización, refactorización, mejora, etc. Consulte la sección sobre compromisos convencionales a continuación para obtener información adicional.
                            4.Longitud: Lo ideal es que la primera línea no tenga más de 50 caracteres y el cuerpo esté restringido a 72 caracteres.
                            5.Contenido: Sea directo, trate de eliminar palabras y frases de relleno en estas oraciones (ejemplos: aunque, tal vez, creo, más o menos). Piensa como un periodista.
                            #Cómo encontrar a su periodista interior
                            Los periodistas y escritores se hacen preguntas para asegurarse de que su artículo sea detallado, sencillo y responda todas las preguntas del lector.
                            Al escribir un artículo buscan responder quién , qué , dónde , cuándo , por qué y cómo.  Para propósitos de confirmación, es muy importante responder el qué y el por qué de nuestros mensajes de confirmación.
                            Para llegar a compromisos bien pensados, considere lo siguiente:
                            #
                            1.¿Por qué he hecho estos cambios?
                            2.¿Qué efecto han tenido mis cambios?
                            3.¿Por qué era necesario el cambio?
                            4.¿A qué se refieren los cambios?
                            #
                            Supongamos que el lector no comprende a qué se refiere la confirmación. Es posible que no tengan acceso a la historia que aborda los antecedentes detallados del cambio.
                            No espere que el código se explique por sí mismo. Esto es similar al punto anterior.
                            Puede parecerle obvio a usted, el programador, si está actualizando algo como estilos CSS, ya que es visual. Es posible que tenga un conocimiento profundo de por qué se necesitaban estos cambios en ese momento, pero es poco probable que recuerde por qué lo hizo cientos de solicitudes de extracción más adelante.
                            Deje claro por qué se realizó ese cambio y observe si puede ser crucial para la funcionalidad o no.
                            #
                            Vea las diferencias a continuación:
                            git commit -m 'Add margin'
                            git commit -m 'Add margin to nav items to prevent them from overlapping the logo'
                            Está claro cuál de ellos sería más útil para futuros lectores.
                            #
                            Imagina que estás escribiendo un artículo importante y de interés periodístico. Da el titular que resuma lo que pasó y lo que es importante. Luego, proporcione más detalles en el cuerpo de forma organizada.
                            En el cine, a menudo se cita "mostrar (no contar)" utilizando imágenes como medio de comunicación en comparación con una explicación verbal de lo que está sucediendo.
                            En nuestro caso, " dígale  no [solo] muestre"; aunque tenemos algunos elementos visuales a nuestra disposición, como el navegador, la mayoría de los detalles provienen de la lectura del código físico.
                            Si es usuario de VSCode, descargue la extensión Git Blame . Este es un excelente ejemplo de cuándo los mensajes de confirmación útiles son útiles para futuros desarrolladores.
                            Este complemento enumerará la persona que realizó el cambio, la fecha de los cambios y el mensaje de confirmación comentado en línea.
                            Imagínese lo útil que podría ser esto para solucionar un error o rastrear los cambios realizados. Otras menciones honoríficas para ver información histórica de Git son Git History y GitLens .
                            -#
                            # tercer de ejemplo commit unificado 
1.Tipo: docs                 :o chore(otros cambios que no modifican src ni archivos de pruebas).
2.Scope: GIT                 :"new scope GIT" (de tematica, o area a tratar).
3.gitmoji: :memo:            :Agregar o actualizar documentación. "los commits siguientes pueden ser(en proceso)"
4.practicas git              :write a short, imperactive tense descrition of the change. "los commits siguientes pueden ser(en proceso) o detallar tematica nueva dependiente de este -new tip de la tematica"
5.pasos para escribir mejores mensajes de confirmación
                             :provide a longer description of the change.    :"los commits siguientes pueden ser(en proceso) o detallar tematica nueva dependiente de este -new tip de la tematica"                 
6.                           :opcional  "pie del commit" dar enter 
                              #El mismo commit escrito de manera manual sin el plugin conventional commits
                              #
                              #
docs(GIT): :memo: practicas git

pasos para escribir mejores mensajes de confirmación                              
                              #
                              #
git add .                    : 
git commit -am "docs(GIT): :memo: practicas git pasos para escribir mejores mensajes de confirmación"

                              #
                              #
# :33) 29/08/2023 , # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
# :32) 28/08/2023 , # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
#-
                    #CONVENTIONAL COMMITS
                    #estructura de mensaje de confirmación consistente:
                    #
                    #
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
                    #
                    #
                    #-    
                    #SISTEMA DE VERSIONES SEMVER 
                    #El versonamiento semantico (SemVer.org)
                    #es la forma en la que indicamos el numero de version de cierto proyecto
                    #normalmente todos los paquetes tienen tres numeros:
                    #ej: v1.1.1  (paquete version 1.1.1.)
                    #1.el primer numero corresponte a una version mejor(mayor),
                    #es decir un cambio vastante grande que puede romper versiones anteriores
                    #2.el segundo digito coresponde a una version minor (añadiendo funcionalidades, mejoras)
                    #que suelen ser FEAT (FEATURE(Mejoras)), que se van añadiendo a la version mas grande 
                    #y el ultimo numero coresponde a un parch (parche), 
                    #es decir: un arreglo que se hace por un bug(error que se ha detectado, etc...)
                    -#                            
                    tipos mas habituales de commit:
fix                 :que es cuando estamos arreglando un bug 
                    #este tipo de commit se correlaciona con una version de tipo patch.                   
feat (feacture)    :nueva funcionalidad o caracteristica que estamos añadiendo al proyecto  (feactures: mejoras)
                    #en el versionado semantico (SEMVER), este commit coresponde con una version minor  
                    #es decir el segundo digito
BREAKING CHANGE     #Si aparece en mayusculas dentro de la descripcion o en el pie de pagina de un commit
                    # o puede ser remplazado por una signo de exclamacion a final del pie del commit (!)
                    #corresponde a una version major, primer digito de SemVer.
                    #es decir estamos subiendo la version VerSem primer digito v2.0.0
                    #porque esta habiendo cambios vastante importantes 
                    #con respecto a versiones anteriores del proyecto                    
                    #types other than fix: and feat: are allowed, 
                    #for example @commitlint/config-conventional (based on the Angular convention) 
                    #recommends build:, chore:, ci:, docs:, style:, refactor:, perf:, test:, and others.
build               :Cuando hacemos un cambio que afecte al sistema de compilacion o de dependencias externas
chore:              :Hacemos cambios pero no afectan al codigo fuente     
ci                  :Es todo lo relacionado a la integracion continua, y aquellos scrips que estemos modifcando ej: un gitHubActions
docs                :Si estamos tocando algo referente a la documentacion del proyecto
style               :cambios referentes al css y al estilo del proyecto, presentacion correcciones ortograficas
refactor:
perf:
test                :Cuando estamos añadiendo pruebas que faltan
                    #(time-video: 4:06 / 12:43):https://www.youtube.com/watch?v=SigVVJmUGv8
                    #dejando una linea en blanco el pie de pagina del commit, que fix estamos cerrando, cierta issue (Tema, problematica que requiera cerrarse), etc..
El pie del commit   :podemos decir que PULL REQUEST (PS) estamos cerrando                    
[optional scope]    : significado 1
(optional scope)    : significado 2: nueva fecture enfocada al paquete o el proyecto dentro de un monorepo(?) del el API
                    #entonces ese SCOPE se pone entre parentesis (api) y el commit es del tipo feat
feat(api)!: send an email to the customer when a product is shipped 
                    :Commit message with scope and ! to draw attention to breaking change                    
                    #mensaje de commit mucho mas elaborado:                     
                    #
                    #
fix: prevent racing of requests

Introduce a request id and a reference to latest request. Dismiss
incoming responses other than from latest request.

Remove timeouts which were used to mitigate the racing issue but are
obsolete now.

Reviewed-by: Z
Refs: #123                    
                    #
                    #Y en una sola linea seria:
                    #
git commit -m "fix: prevent racing of requests\nIntroduce a request id and a reference to latest request. Dismiss incoming responses other than from latest request.\nRemove timeouts which were used to mitigate the racing issue but are obsolete now.\nReviewed-by: Z \nRefs: #123"  
                    : en una sola linea
                    : Commit message with multi-paragraph body and multiple footers
                    #Se trata de un fix, no posee scope, aqui vemos la descripcion, vemos un resumen un poco mas detallado.
                    # y final mente en el pie de pagina podemos ver que esta revisado o se ha hecho per programin (progrmacion entre dos perdonas par) junto con otra persona
                    #y lo hace referencia a una iso concreta ya sea de github issues, gira    
                    #
                    #tambien puede estar un BREAKING CHANGE en esta seccion de pie del commit y coresponde a SemVer digito primero cambio MAJOR, se suve la version porque esta habiendo cambios vastante importantes con respecto a versiones anteriores del proyecto
                    #
                    #PORQUE USAR CONVENCIONAL COMMITS
                    #varia ventajas: 
                    #1. unificar la forma de escribir esos mensajes dentro del equipo. 
                    #2. Siguendo este estandar o especificacion: podemos configurar herramientas de automatizacion y tener un fichero change-log de forma automatica.
                    #3. Si especificamos bien que tipo de commit es, podemos ajustarlo con SEMVER y determinar automaticamente cuando hay un cambio de version y utilizando herramientas, hacer que ese numero se actualice de manera automatica.
                    #4. puedes usarlo tambien para automatizar los procesos de build y de despliegue o publicacion si se trata de uns libreria 
                    #5. tambien permite si estas haciendo un proyecto open source o para gente que este entrando de nuevo en un proyecto (por primera vez al proyecto) de tu empresa comprender el proyecto, es un proceso de UNBORDING, hacer mas facil para estas personas nuevas en el proyecto que todavia no tienen un contexto del proyecto, permitirles explorar el historial de commits para que se hagan una idea de por donde van los cambios.    
                    #estos cambios lo podemos hacer de manera manual o atravez de una herramienta extension o pluging de VSCODE: conventionals commits , permite hacerlo de una manera automatica
scopes              : conventionalCommits.scopes : "GI", "UI" nombre de paquetes, modulos a los que haces referencia es como en que departamento o modulo del proyecto estas commiteando, algo asi como clasificasion.
                    #Establecer un linter que verifique si los mensajes de commits siguen este patron
                    # porque tu puedes tener tu extencion de visual estudio code, o seguir esta nomenclatura, esta especificacion. 
                    # pero el resto del equipo no y si ya habeis llegado a un concenso 
                    #lo suyo es que todas las personas de un proyecto sigan ese convenio
                    #para ello tenemos herramientas como: commitlint
                    #que seria como el slint para los ficheros de JavaScript
                    #pero para los mensajes de commits
                    #es una herramienta de linea de comandos
                    #pero la podemos integrar en nuestro proyecto
                    #he incluso unirlo con nuestro GitHub 
                    #para asegurarnos que cada vez que vamos a hacer un commit 
                    #ese hook se lance 
                    #verifique si sigue las normas de estilo de convencional commit
                    #y si es asi el commit se realizara.
gitmoji             :https://gitmoji.dev/ # es un proyecto estandarrizar imagenes en el area de git commit descriptions.        
                    #un ejemplos:
:art:               :Improve structure / format of the code.
:zap:               :Improve performance.
:fire:              :Remove code or files.
:bug:               :Fix a bug.
:lipstick:          :icono del pintalabios, si haz añadido o actualizado la UI y los ficheros de estilo style, este es el que mas se encaja.
                    #son opcionales pero dan un poco de colorido a tu repositorio
                    # es una libreria de 70 imagenes relacionadas a descripciones git
                    #una imagen vale mas que mil palabras, es bueno saber esta especificacion.  
                    #igual que conventional commits pero mas visual a la hora de darle significado a los commits
                    #commitlint example:
npm init -y         #nos crea el fichero package.json                     
                    #ahora vamos a instalar dos dependencias de desarrollo:
npm install --save-dev @commitlint/cli @commitlint/config-conventional                     
                    "devDependencies": {
                      "@commitlint/cli": "^17.7.1",
                      "@commitlint/config-conventional": "^17.7.0"
                    }
                    #commitlint cli
                    #y commitlint conventional
commitlint.config.js :una vez instaladas creamos un fichero en la raiz de nuestro proyecto (commitlint.config.js)
                     #y añadimos el siguiente contenido: 
                     module.exports = {
                       extends: ['@commitlint/config-conventional'],
                     };
                     #vasicamente estamos heredando las reglas de estilos de conventional commit, que es la libreria que acabamos de instalar  
                     #ahora vamos a integrarlo con HUSKY (configurar husky y lintestate para automatizar todo este proceso de gitsHubs)
                     #instalariamos HUSKY como dependencia de desarrollo
npm i -D husky              
                    "devDependencies": {
                        "husky": "^8.0.3"
                      }       
                     #añadiriamos el script-prepare que lo que hace es llamar "husky install" dentro del packjson
npm set-script [<script>] [<command>]                     
npm set-script prepare 'husky install'      #no funciono el comando en windows               
npm config set script-shell "d:\\D-Program Files\\git\\bin\\bash.exe"   : no soluciono
npm set-script prepare 'husky install'  # no funciona
npm config delete script-shell                                          : revertir el proceso
set-script           :has been deprecated as per documentation, se procede hacerlo manual en el archivo package.json
                    "scripts": {
                        "prepare": "husky install"
                      },
                     #y llamaremos a este script que acabamos de crear para que se instale husky en el proyecto
npm run prepar                                           
                     #nos da error porque no tenemos configurado un repositorio
                     #husky - .git can't be found (see https://typicode.github.io/husky/#/?id=custom-directory)                     
                     #llamamos a git init para que se inicialice
git init                     
                     #y ahora si que se configurara husky correctamente
npm run prepar       : husky - Git hooks installed
                     #ahora vamos añadir el hook-commit-message : este hook va a verificar el mensage de commit
                     #hay distintos githubs, no confundir con los reacts hub
                     #pre-commit y pre-push : son hook o script que se van ajecutar antes de hacer commit o antes de hacer un push ala rama principal o a la rama origen de nuestro repositorio
                     # el hook commit-message lo que va a verificar es el mensaje de commit                     
npx husky add .husky/commit-msg "npx --no -- commitlint --edit ${1}" : enter y ya se nos habra creado este escript, solo se tiene que hecer en este momento                     
                     #husky - created .husky/commit-msg  : y ya se nos ha creado este script
                     #esto solo lo tienen que hacer en este momento no tienes que hacerlo cada vez que haces un commit
                     #esta es la gracia de husky que automatiza todo este script y no tienes que hacerlo cada vez que ejecutas un commit
                     #https://typicode.github.io/husky/
                     #entonces vamos aprovarlo 
                     #creamos un fichero .gitgnore
                     #y aqui vemos que tenemos cinco cambios 
git add .                     
git commit -am "initial commit" : Este es un ejemplo de un commit que no sigue la espeficicacion de conventional commit, no le estamos diciendo de que tipo es, no hay un SCOPE aunque es opcional, 
                                 # es simplemente un mensaje     
                                 # como puedes ver nos salta un error:
                                 #
                                 ⧗   input: initial commit
                                 ✖   subject may not be empty [subject-empty]
                                 ✖   type may not be empty [type-empty]

                                 ✖   found 2 problems, 0 warnings
                                 ⓘ   Get help: https://github.com/conventional-changelog/commitlint/#what-is-commitlint
                                 husky - commit-msg hook exited with code 1 (error)
                                 #
                                 # el sujeto no puede estar vacio, 
                                 #el tipo no puede estar vacio y no se ha podico realizar el commit
                                 #entonces vamos hacerlo denuevo pero siguiendo la especificacion de conventional commits  
                                 #implementamos la herramienta, el pluging de VSCODE conventional commit para realizar el commit
tipo chore                        : es commit del tipo chore, no tiene scope 
                                  #y hay un emmoji especial para cuando se empieza un proyecto(begin a project)                    
                                  # descripcion corta: inicial commit
                                  # no le ponemos descripcion 
                                  # y no le ponemos ningun braking changes pie del commit
                                  # le decimos que salve todo
                                  #y ahora si que no ha salido ningun error.
                                  #si nos vamos al historial de commits podemos ver que esta aui y que ha funcionado correctamente.
                                  # para terminar y dejar esto finisimo, tenemos una herramienta 
                                  # conventional change-log que nos permite: 
                                  #nos permite generar ese fichero de cambios entre versiones (change-log) 
                                  #si seguimos las normas de estilo de conventional commit
                                  #se instalar de forma global la libreria conventionalchangelog-cli, tambien se puede instalar de forma local en tu propio proyecto
npm install -g conventional-cahngelog-cli : error ortografico
                                  :npm ERR! 404 Not Found - GET https://registry.npmjs.org/conventional-cahngelog-cli 
npm install -g conventional-changelog-cli  :https://www.npmjs.com/package/conventional-changelog-cli
                                  : added 86 packages in 11s :ok
                                  #y el comando a utilizar seria 
conventional-changelog -i CHAGELOG.md -s -r 0
                                  #nos crea el fichero CHANGELOG.md, con el siguiente contenido: 
                                  #
                                  ## 1.0.0 (2023-08-29)

                                  * chore: :tada: initial commit 0c36721

                                  #
                                  #y hasta ahora aparece el unico commit que hemos hecho
                                  #pero como puedes ver que se a tratado 
                                  #de un cambio pequeño utiliza 
                                  #el ultimo numero de SEMVER (0.0.1)
                                  #es decir un parche (pach), ademas aparece la fecha en la que se ha hecho el commit
                                  # y la lista de aquellos commits que se hallan hecho
                                  # si hacemos un commit que lleve un cambio MINOR o un cambio MAJOR 
                                  #pues el versionado tambien se ira incrementando automaticamente
git add CHANGELOG.md              : añadiriamos este archivo que se ha creado                     
chore:release a pach version     :y añadiriamos un pequeño commit que seria CHORE, (opcional por ser pequeño lo puedes hacel manual sin la herramienta pero respetanto la especificacion conventional commit, si no respetas esta especificacion de igualmanera no te permitira hacer el commit) o con la herramienta conventionals commits
                                  # ahora que tenemos el directorio de trabajo de git limpio podemos ejecutar
npm version patch                 # he indicar de que tipo sera este cambio de version, y el automaticamente se va a encargar de subir de version nuestro paquete.
npm version major                 #pues vemos que sube la version 1.0.0                                  
npm version major                 #pues vemos que sube la version 2.0.0                                  
npm version [<newversion> | major | minor | patch | premajor | preminor | prepatch | prerelease | from-git] 
                                  : https://docs.npmjs.com/cli/v9/commands/npm-version
npm version minor                 #pues vemos que sube la version 2.1.0
                                  #este comando te crea un commit automaticamente al cambio de version
                                  #como puedes ver de esta forma siguiendo ciertas herramientas 
                                  #puedes tener automatizado 
                                  #todas estas pequeñas tareas 
                                  #que no son muy dificiles de hacer 
                                  #pero si que te van robando tiempo en el dia a dia
                                  #incluso pueden inducirte a errores
                                  #fuente, fin del viedo: https://www.youtube.com/watch?v=SigVVJmUGv8
                                  #Que especificaciones conoces, cuales manejas, cuales dominas. 
                                  #vas a empezar a iplementarlos en tus proyectos en tu empresa?, fin del video
                                  # link: https://www.youtube.com/watch?v=SigVVJmUGv8
                    #-
                    fuente: https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/
                    #La anatomía de un mensaje de compromiso
git commit -m <message>                   :Básico
git commit -m <title> -m <description>    :Detallado
                    #tipos de commits  
chore               :cambios que no se relacionan con una solución o característica y no modifican archivos src o de prueba (por ejemplo, actualización de dependencias)
refactor            :código refactorizado que no corrige un error ni agrega una característica                        
docs                :actualizaciones de documentación como el README u otros archivos de rebajas
style               :cambios que no afectan el significado del código, probablemente relacionados con el formato del código, como espacios en blanco, falta de punto y coma, etc.
test                :incluir pruebas nuevas o corregir pruebas anteriores
perf                :mejoras de rendimiento
ci                  :integración continua relacionada
build               :cambios que afectan el sistema de compilación o dependencias externas
revert              :revierte una confirmación anterior
                    #Ejemplo de compromiso convencional completo:
                    #
                    #
fix: fix foo to enable bar

This fixes the broken behavior of the component by doing xyz. 

BREAKING CHANGE
Before this fix foo wasn't enabled at all, behavior changes from <old> to <new>

Closes D2IQ-12345
                    #
                    #
                    #Comparaciones de mensajes de confirmación
                    #Revise los siguientes mensajes y vea cuántas de las pautas sugeridas marcan en cada categoría.
                    #Bien
feat: improve performance with lazy load implementation for images          :Bien
chore: update npm dependency to latest version                              :Bien   
Fix bug preventing users from submitting the subscribe form                 :Bien
Update incorrect client phone number within footer body per client request  :Bien                 
                    #Mal
fixed bug on landing page         :Mal
Changed style                     :Mal
oops                              :Mal
I think I fixed it this time?     :Mal
mensajes de confirmación vacíos   :Mal           
                      #Natalia Pina  Ingeniero UX en D2iQ. Entusiasmado por CSS, React, JavaScript, TypeScript, sistemas de diseño, UX y diseño de UI.                
                    -#            
-#
# :31) 27/08/2023 , # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
          #-------
          # ¿Cuáles son los 3 estados de git? 
          # confirmado (committed), modificado (modified), y preparado (staged).
          #--------
          #-
          # Comandos básicos en la terminal de Git Bash en Windows
            La ruta principal en Windows es c:/, en UNIX es solo /.
            Windows no hace diferencia entre mayúsculas y minúsculas, pero UNIX si.
            Git Bash usa la rua /c para dirigirse al disco c:/ en Windows. 
            Por lo tanto, la ruta del usuario con el que estás trabajando es /c/Users/NombreUsuario
            Comandos
pwd             : nos muestra la carpeta actual en la que nos encontramos.
mkdir           : nos permite crear carpetas, p. ej. mkdir NuevaCarpeta
touch           : nos permite crear archivos nuevos, p.ej. touch NuevoArchivo.txt
cat             : nos permite ver el contenido de un archivo, p.ej. cat NuevoArchivo.txt
cd              : nos permite cambiarnos de carpeta, p.ej. cd NuevaCarpeta.
cd ..           : nos permite regresar al directorio o carpeta anterior.
cd o cd ~       : nos lleva a la ruta del usuario.
cd /c           : nos vamos al disco C:/.
cd -            : nos lleva directamente al ultimo directorio visitado.
ls              : nos permite ver los archivos de la carpeta donde estamos actualmente.
ls -l           : Ver todos los archivos como una lista en donde incluye el usuario, grupo, permisos sobre el archivo, tamaño, fecha y hora de creación.
ls -lh          : Muestra la misma información que ls-l pero con unidades de tamaño, es decir, kb o mb.
ls-R            : muestra el contenido de todos los sudirectorios de forma recursiva.
ls -S           : Ordena los resultados por tamaño de archivo.
rm              : Nos permite borrar un archivo o carpeta ej: rm NuevoArchivo.txt
rmdir “nombre del directorio”/    : borrar un directorio: Solo funciona con directorios vacíos.
rm -r ‘nombre de la carpeta’      :me permite eliminar la carpeta y los archivos dentro de ella de forma recursiva.
cp “nombre del archivo que quremos copiar” “nombre del directorio a donde lo queremos copiar”                   : nos permite copiar un archivo.
mv “el directorio de donde queremos mover/el nombre del archivo” “el directorio hacia donde lo queremos mover”  : nos permite mover un archivo.
clear           : nos permite limpiar la pantalla.
history         : ver los últimos comandos que ejecutamos y un número especial con el que podemos volver a repetir el comando.
                #-
                #-
                ¿Cuáles son los comandos GIT más utilizado
git config
git clone
git init
git status
git push
git add
git commit
git branch                
#-
         #Un proyecto GIT consta de tres secciones principales: 
         #WORKING DIRECTORY   : el directorio de trabajo, 
         #STAGING (INDEX)     : el área de preparación, 
         #LOCAL (REPOSITORY)  : y el directorio git.
         #REMOTE (REPOSITORY) : mas la opcion de repositorio remoto centralizado para trabajo en equipo sobre un mismo repositorio.
         #Cuando quieres tomar una foto una instantannea cuando ya hay algo definido minimamente, cuando ya hay algo funcional
         # aqui es cuendo se suele hacer un commit. de otra maneda pueden ser solo commits de doc: backup.
         # si haces elgo publico que quieres mostrar, y para que lo haces.
         # El directorio de trabajo es donde se agregan, borran y editan los archivos. 
         # Luego, los cambios son preparados (indexados) en el área de preparación. 
         # Después de que confirmes tus cambios, la instantánea de los cambios se guardará en el directorio git.
         # El software puede tener una fuerte curva de aprendizaje, pero hay muchos tutoriales disponibles para ayudarte.
         # Comandos de GIT básicos:                   
git init                        : git init creará un nuevo repositorio local GIT. El siguiente comando de Git creará un repositorio en el directorio actual                   
git init [nombre del proyecto]  : Como alternativa, puedes crear un repositorio dentro de un nuevo directorio especificando el nombre del proyecto                   
git clone nombredeusuario@host:/path/to/repository
                                :git clone se usa para copiar un repositorio. Si el repositorio está en un servidor remoto, usa
git clone /path/to/repository   :A la inversa, ejecuta el siguiente comando básico para copiar un repositorio local                   
git add <temp.txt>              :git add se usa para agregar archivos al área de preparación. Por ejemplo, el siguiente comando de Git básico indexará el archivo temp.txt 
git commit –m “El mensaje que acompaña al commit va aquí”
                                :git commit creará una instantánea de los cambios y la guardará en el directorio git.
                                # Consejo profesional Ten en cuenta que los cambios confirmados no llegarán al repositorio remoto.
git config --global user.email tuemail@ejemplo.com
                                :git config puede ser usado para establecer una configuración específica de usuario, como el email, nombre de usuario y tipo de formato, etc. Por ejemplo, el siguiente comando se usa para establecer un email                                
git config --local user.email tuemail@ejemplo.com
                                :La opción -global le dice a GIT que vas a usar ese correo electrónico para todos los repositorios locales. Si quieres utilizar diferentes correos electrónicos para diferentes repositorios, usa el siguiente comando
git status                      :git status muestra la lista de los archivos que se han cambiado junto con los archivos que están por ser preparados o confirmados 
git push  origin <master>       :git push se usa para enviar confirmaciones locales a la rama maestra del repositorio remoto. Aquí está la estructura básica del código
                                #Consejo profesional Reemplaza <master> con la rama en la que quieres enviar los cambios cuando no quieras enviarlos a la rama maestra.
git checkout -b <branch-name>
                                : git checkout crea ramas y te ayuda a navegar entre ellas. Por ejemplo, el siguiente comando crea una nueva y automáticamente se cambia a ella
git checkout <branch-name>      : Para cambiar de una rama a otra, sólo usa
git remote -v                   :git remote te permite ver todos los repositorios remotos. El siguiente comando listará todas las conexiones junto con sus URLs
git remote add origin <host-or-remoteURL>
                                :Para conectar el repositorio local a un servidor remoto, usa este comando
git remote <nombre-del-repositorio>
                                :Por otro lado, el siguiente comando borrará una conexión a un repositorio remoto especificado 
git branch                      :git branch se usa para listar, crear o borrar ramas. Por ejemplo, si quieres listar todas las ramas presentes en el repositorio, el comando debería verse así 
git branch -d <branch-name>     :Si quieres borrar una rama, usa
git pull                        :git pull fusiona todos los cambios que se han hecho en el repositorio remoto con el directorio de trabajo local
git merge <branch-name>         :git merge se usa para fusionar una rama con otra rama activa
git diff --base <file-name>     :git diff se usa para hacer una lista de conflictos. Para poder ver conflictos con respecto al archivo base, usa  
git diff <source-branch> <target-branch>
                                :El siguiente comando se usa para ver los conflictos que hay entre ramas antes de fusionarlas 
git diff                        : Para ver una lista de todos los conflictos presentes usa
git tag 1.1.0 <instert-commitID-here>
                                : git tag marca commits específicos. Los desarrolladores lo usan para marcar puntos de lanzamiento como v1.0 y v2.0.
git log                         :git log se usa para ver el historial del repositorio listando ciertos detalles de la confirmación. Al ejecutar el comando se obtiene una salida como ésta    
                                #commit 15f4b6c44b3c8344caasdac9e4be13246e21sadw
                                #Author: Alex Hunter <alexh@gmail.com>
                                #Date:   Mon Oct 1 12:56:29 2016 -0600
git reset - -hard HEAD          :git reset sirve para resetear el index y el directorio de trabajo al último estado de confirmación                                
git rm filename.txt             :git rm se puede usar para remover archivos del index y del directorio de trabajo.
git stash                       :git stash guardará momentáneamente los cambios que no están listos para ser confirmados. De esta manera, pudes volver al proyecto más tarde.
git show                        :git show se usa para mostrar información sobre cualquier objeto git.
git fetch origin                :git fetch le permite al usuario buscar todos los objetos de un repositorio remoto que actualmente no se encuentran en el directorio de trabajo local.
                                #cuales son los objetos de un repositorio:  
git ls-tree HEAD                :git ls-tree te permite ver un objeto de árbol junto con el nombre y modo de cada ítem, y el valor blob de SHA-1. Si quieres ver el HEAD, usa:
git cat-file –p d670460b4b4aece5915caf5c68d12f560a9fe3e4
                                :git cat-file se usa para ver la información de tipo y tamaño de un objeto del repositorio. Usa la opción -p junto con el valor SHA-1 del objeto para ver la información de un objeto específico, por ejemplo:
git grep “www.hostinger.com”    :git grep le permite al usuario buscar frases y palabras específicas en los árboles de confirmación, el directorio de trabajo y en el área de preparación. Para buscar por www.hostinger.com en todos los archivos, usa:
gitk                            :gitk muestra la interfaz gráfica para un repositorio local. Simplemente ejecuta
git instaweb –http=webrick      :git instaweb te permite explorar tu repositorio local en la interfaz GitWeb. Por ejemplo:
git gc                          :git gc limpiará archivos innecesarios y optimizará el repositorio local.
git archive - -format=tar master
                                :git archive le permite al usuario crear archivos zip o tar que contengan los constituyentes de un solo árbol de repositorio. Por ejemplo:
git prune                       :git prune elimina los objetos que no tengan ningún apuntador entrante.                            
git fsck                        :git fsck realiza una comprobación de integridad del sistema de archivos git e identifica cualquier objeto corrupto
git rebase master               :git rebase se usa para aplicar ciertos cambios de una rama en otra. Por ejemplo.
.                                # fuente: https://www.hostinger.es/tutoriales/comandos-de-git  
#-
#-
                  #10 Comandos de Git Que Todo Desarrollador Debería Saber
                  #fuente: https://www.freecodecamp.org/espanol/news/10-comandos-de-git-que-todo-desarrollador-deberia-saber/
                  #Git es una parte importante de quien programa a diario 
                  #(especialmente si estás trabajando con un equipo) 
                  #y se usa extensamente en la industria de software.
git clone <https://link-con-nombre-del-repositorio>
                  :Git clone es un comando para descargarte el código fuente existente desde un repositorio remoto (como Github, por ejemplo). En otras palabras, Git clone básicamente realiza una copia idéntica de la última versión de un proyecto en un repositorio y la guarda en tu ordenador.
                  #Hay un par de formas de descargar el código fuente, pero principalmente yo prefiero clonar de la forma con https                  
                  #Esto hará una copia del proyecto en tu espacio de trabajo local y así podrás empezar a trabajar con él.
git branch <nombre-de-la-rama>   :Creando una nueva rama
                  :Las ramas (branch) son altamente importantes en el mundo de Git. Usando ramas, varios desarrolladores pueden trabajar en paralelo en el mismo proyecto simultáneamente. Podemos usar el comando git branch para crearlas, listarlas y eliminarlas.                  
git push <nombre-remoto> <nombre-rama>
                  :Este comando creará una rama en local. Para enviar (push) la nueva rama al repositorio remoto, necesitarás usar el siguiente comando
git branch        :Visualización de ramas 
git branch --list :Visualización de ramas   
git branch -d <nombre-de-la-rama>
                  :Borrar una rama
git checkout <nombre-de-la-rama>                  
                  :Este es también uno de los comandos más utilizados en Git. Para trabajar en una rama, primero tienes que cambiarte a ella. Usaremos git checkout principalmente para cambiarte de una rama a otra. También lo podemos usar para chequear archivos y commits.
                  #Hay algunos pasos que debes seguir para cambiarte exitosamente entre ramas:
                  #Los cambios en tu rama actual tienen que ser confirmados o almacenados en el guardado rápido (stash) antes de que cambies de rama.
                  #La rama a la que te quieras cambiar debe existir en local.
git checkout -b <nombre-de-tu-rama>
                  :Hay también un comando de acceso directo que te permite crear y cambiarte a esa rama al mismo tiempo
                  #Este comando crea una nueva rama en local (-b viene de rama (branch)) y te cambia a la rama que acabas de crear
git status        :El comando de git status nos da toda la información necesaria sobre la rama actual.
                  #Podemos encontrar información como:
                  #Si la rama actual está actualizada
                  #Si hay algo para confirmar, enviar o recibir (pull).
                  #Si hay archivos en preparación (staged), sin preparación(unstaged) o que no están recibiendo seguimiento (untracked)                  
                  #Si hay archivos creados, modificados o eliminados
staged            :archivos en preparación               
unstaged          :archivos sin preparación  
untracked         :que no están recibiendo seguimiento
                  :git status nos da información acerca del archivo y las ramas 
git add <archivo> : Cuando creamos, modificamos o eliminamos un archivo, estos cambios suceden en local y no se incluirán en el siguiente commit (a menos que cambiemos la configuración).
                  #Necesitamos usar el comando git add para incluir los cambios del o de los archivos en tu siguiente commit.                  
                  # es como quien dice: que vas a incluir en tus commits
git add -A        :Añadir todo de una vez          
                  #Si revisas la captura de pantalla que he dejado en la sección 4, verás que hay nombres de archivos en rojo - esto significa que los archivos sin preparación. 
                  #Estos archivos no serán incluidos en tus commits hasta que no los añadas.   
                  #Para añadirlos, necesitas usar el git add:
                  #Los archivos en verde han sido añadidos a la preparación gracias al git add
                  #Importante: El comando git add no cambia el repositorio 
                  #y los cambios que no han sido guardados 
                  #hasta que no utilicemos el comando de confirmación git commit.
git commit -m "mensaje de confirmación"
                  :Importante: Git commit guarda tus cambios únicamente en local.
                  #Este sea quizás el comando más utilizado de Git. 
                  #Una vez que se llega a cierto punto en el desarrollo, 
                  #queremos guardar nuestros cambios 
                  #(quizás después de una tarea o asunto específico).
                  #Git commit es como establecer un punto de control en el proceso de desarrollo 
                  #al cual puedes volver más tarde si es necesario.
                  #También necesitamos escribir un mensaje corto 
                  #para explicar qué hemos desarrollado o modificado en el código fuente.
git push <nombre-remoto> <nombre-de-tu-rama>
                  :Git push envía tus commits al repositorio remoto.
                  #Después de haber confirmado tus cambios, el siguiente paso que quieres dar es: 
                  #enviar tus cambios al servidor remoto.
git push --set-upstream <nombre-remoto> <nombre-de-tu-rama>            : -u (--set-upstream)  
                  :De todas formas, si tu rama ha sido creada recientemente, puede que tengas que cargar y subir tu rama con el siguiente comando:                  
                  #Importante: Git push solamente carga los cambios que han sido confirmados.                  
                  # or
git push -u origin <nombre-de-tu-rama>                  
                  : -u (--set-upstream)
git pull <nombre-remoto>
                  :El comando git pull se utiliza para recibir actualizaciones del repositorio remoto. Este comando es una combinación del git fetch y del git merge lo cual significa que cundo usemos el git pull recogeremos actualizaciones del repositorio remoto (git fetch) e inmediatamente aplicamos estos últimos cambios en local (git merge).                  
                  :Esta operación puede generar conflictos que tengamos que resolver manualmente.
git revert        :A veces, necesitaremos deshacer los cambios que hemos hecho. 
                  #Hay varias maneras para deshacer nuestros cambios en local y/o en remoto 
                  #(dependiendo de lo que necesitemos), 
                  #pero necesitaremos utilizar cuidadosamente estos comandos 
                  #para evitar borrados no deseados.  
                  #Una manera segura para deshacer nuestras commits es utilizar git revert.                
 git log -- oneline
                  :Para ver nuestro historial de commits
                  #histórico de git en mi rama master
git revert 3321844
                  :Entonces, solo necesitamos especificar el código de comprobación que encontrarás junto al commit que queremos deshacer                     
                  #Después de esto, verás una pantalla como la de abajo 
                  #-tan solo presiona shift + q para sali  
                  # un mensaje vacio aborta a un commit, es obligatorio un minimo mensaje de descripcion del commit 
                  :El comando git revert deshará el commit que le hemos indicado, 
                  #pero creará un nuevo commit deshaciendo la anterior.
                  #commit generado con el git revert
                  #La ventaja de utilizar git revert 
                  #es que no afecta al commit histórico. 
                  #Esto significa que puedes seguir viendo todos los commits en tu histórico, incluso los revertidos.
                  #Otra medida de seguridad es que todo sucede en local a no ser que los enviemos al repositorio remoto. Por esto es que git revert es más seguro de usar y es la manera preferida para deshacer los commits.
git merge <nombre-de-la-rama>                  
                  #10. Git merge
                  #Cuando ya hayas completado el desarrollo de tu proyecto en tu rama 
                  #y todo funcione correctamente, 
                  #el último paso es fusionar la rama con su rama padre (dev o master). 
                  #Esto se hace con el comando git merge.
                  #Git merge básicamente integra las características de tu rama con todos los commits realizados 
                  #a las ramas dev (o master).  
                  #Es importante que recuerdes que tienes que estar 
                  #en esa rama específica que quieres fusionar con tu rama de características.
git checkout dev  : Primero, debes cambiarte a la rama dev
                  #Por ejemplo, cuando quieres fusionar tu rama de características en la rama dev
git fetch         :Antes de fusionar, debes actualizar tu rama dev local
git merge <nombre-de-la-rama>
                  :Por último, puedes fusionar tu rama de características en la rama dev
                  #Pista: Asegúrate de que tu rama dev tiene la última versión 
                  #antes de fusionar otras ramas, 
                  #si no, te enfrentarás a conflictos u otros problemas no deseados.
                  #Aquí están mis 10 comandos de git más usados cuando me enfrento a la programación en mi día a día. 
                  #Hay muchas más cosas que aprender sobre Git y las explicaré más adelante en oros artículos. 
                  #Si quieres aprender más sobre el desarrollo web, ¡puedes seguirme en Youtube! : https://www.youtube.com/channel/UC1EgYPCvKCXFn8HlpoJwY3Q
                  #¡Gracias por leerme!
                  #Traducido del artículo de Cem Eygi - 10 Git Commands Every Developer Should Know  : https://www.freecodecamp.org/news/10-important-git-commands-that-every-developer-should-know/
                  #Cara sonrriente carismatica de perfil y
                  #Nora Gonzalo Ciordia, FullStack Dev Jr living in Madrid LinkedIn: https://www.linkedin.com/in/noragonzalo/
#-                  
                  #Aprende a codificar de forma gratuita. 
                  #El plan de estudios de código abierto de freeCodeCamp 
                  #ha ayudado a más de 40,000 personas a obtener trabajos como desarrolladores. 
                  #Empezar : https://www.freecodecamp.org/learn/
freeCodeCamp      :Empezar : https://www.freecodecamp.org/espanol/learn/
                  #Si eres nuevo en la programación, te recomendamos comenzar por el principio y obtener estas certificaciones en orden.
                  #Para obtener cada certificación, construye los 5 proyectos requeridos y consigue aprobar todas las pruebas 
                  #Puedes agregar estas certificaciones a tu currículum o LinkedIn. Pero más importante que las certificaciones es la práctica que obtienes en el camino
                  #Si te sientes abrumado, es normal. Programar es difícil.
                  #La práctica es la clave. Práctica, práctica, práctica.
                  #Y este currículo te brindará miles de horas de práctica de programación.
                  #Y si deseas aprender más sobre matemáticas y teoría de la informática, 
                  #también tenemos miles de horas de cursos en video en el canal de YouTube de freeCodeCamp: https://www.youtube.com/freecodecamp
                  #Si deseas obtener un trabajo de desarrollador o clientes independientes, 
                  #las habilidades de programación serán solo una parte del rompecabezas. 
                  #También necesitas construir tu red personal 
                  #y tu reputación como desarrollador.
                  #Puedes hacer esto en LinkedIn y GitHub, y también en el foro freeCodeCamp: https://forum.freecodecamp.org/.
                  #¡Feliz día programando!
                  #- Quincy Larson, el profesor que fundó freeCodeCamp.org
                  # Bienvenido a freeCodeCamp.org
                  #Ahora veo que las circunstancias de nuestro nacimiento no importan. 
                  #Es lo que hacemos con el regalo de la vida lo que nos define
                  #MewTwo - Pokemon
                  #1. Certificacion diseño Web resposivo : https://www.freecodecamp.org/espanol/learn/2022/responsive-web-design/                  
                  #2. Certificacion Algoritos de JavaScript y estructuras de datos
                  #3. Certificacion librerias de desarrollo de la interfaz
#-                  
#-
# :30) 26/08/2023 , # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
          # estudiando y organizando contenido
          # es una demo en el curso de Git puedes ignorar la PR (PULL REQUEST) : solicitudud que intengres mis contribuciones al proyecto FORKeado.
          # me puedo hacer un auto Pull Request, a mi mismo, yo podria decirle que la acepto, que sus commits se apliquen a mi repositorio, pero debo de tener los permisos. 
          # me voy a un proyecto en el que si tengo permisos para hacerlo yo mismo todo
          # cree otra cuenta github para relizar las pruebas de FORK : miguelepst@gmail.com user: okmiguel
          # curso interactivo de git en ingles: https://skills.github.com/
          # Learn how to use GitHub Get started with an "Introduction to GitHub" course in GitHub Skills. 
          # GitHub Skills Learn how to use GitHub with interactive courses designed for beginners and experts. 
          # What do you want to do first? Every developer needs to configure their environment, so let's get your GitHub experience optimized for you.
          # opcion 2: Collaborate with your team Improve the way your team works together and get access to more features with an organization. : https://github.com/organizations/plan
          # tiene un plan gratuito: Pick a plan for your organization, costos: 0, 4 usd, 19.25 usd por mes
          # opcio 1: Start a new project Start a new repository or bring over an existing repository to keep contributing to it. 
          # https://github.com/new       # Crear nuevo repositorio
#-          
https://github.com/search                # buscar a alguien en github
https://github.com/search/advanced       # busqueda avanzada
                                         # Users options
                                         # From this location : colombia    , influencer de colombia
                                         # With this many followers : >1000
                                         # With this many public repositories : > 50   # que este muy activo
                                         # Working in this language: JavaScript   (es igual a Angular)
                                         # le das en buscar
                                         # como crear tu perfil en github: debes poner tu correo
                                         # otra manera de buscar usuario es ir donde otro usuarios y ver aquien sigue este tio, investigas.
                                         # y eliges a quienes vas aseguir
                                         # para que amplies tu red de contactos
                                         # Cómo crear tu PERFIL de GITHUB desde cero *muy sencillo* (Curso de Github) #3
                                         # https://www.youtube.com/watch?v=nrMSM3NleUM
#-                                         
# :29) 25/08/2023 , # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
# :28) 24/08/2023 , # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
#----------------------------------------------------
#- GitHub despues de crear un repositorio #
#----------------------------------------------------
…or create a new repository on the command line
echo "# primer" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/okmiguel/primer.git
git push -u origin main

…or push an existing repository from the command line

git remote add origin https://github.com/okmiguel/primer.git
git branch -M main
git push -u origin main

                    # Creando un repositorio en gitHub y vinculandolo con un repositorio local
                    # Configuracion rapida si ya has hecho este tipo de cosas antes
                    # Quick setup — if you’ve done this kind of thing before
https://github.com/Miguelepst/git-exp-dicc.git        # Ruta del repositorio de GitHub
                    # O crear un nuevo repositorio en la linea de comandos
                    # …or create a new repository on the command line
echo "# git-exp-dicc" >> README.md          # crear un archivo README.md con el contenido interno: # git-exp-dicc
git init                                    # inicializar repositorio  
git add README.md                           # agregar readme.md al staged
git commit -m "first commit"                # commit 1, el inicial, hacer primer confirmacion de cambio, commit inicial
git branch -M main                          #  -M  move/rename a branch, even if target exists  
                                            # https://git-scm.com/docs/git-branch
                                            # Con una opción -mo -M, se cambiará el nombre de <oldbranch> a <newbranch>. Si <oldbranch> tenía un reflog correspondiente, se le cambia el nombre para que coincida con <newbranch> y se crea una entrada de reflog para recordar el cambio de nombre de la rama. Si <newbranch> existe, se debe usar -M para forzar el cambio de nombre. 
                                            # https://www.makigas.es/series/tutorial-de-git/git-reflog
                                            #  git-reflog, El reflog es un log especial donde se incorporan commits cada vez que se hace un cambio de rama o un reset, lo que puede ser usado en caso de emergencia para recuperar un estado anterior de la rama si la liamos con el rebase, reset o checkout.
git remote add origin https://github.com/Miguelepst/git-exp-dicc.git     # pero si ya habia sido fijado anteriormente da error
                                            # Curso Avanzado de Git y Github - 7. Ramas de seguimiento: https://www.youtube.com/watch?v=kYqBFAsD-r8 
                                            # git push -u origin master                    Cuando uno sube una rama le podemos dar la opcion -u, lo que dice: Cree una rama de seguimiento para esta rama y la enlaace con esta rama.
                                            # git push -u origin mi-rama                  
git push -u origin main                     # --set-upstream (-u), crear una rama de seguimiento de la rama main local en el remoto 
                            # create a new repository on the command line
git init                    # inicializando el repositorio Te ubica en la rama MASTER, MAIN
                            # Initialized empty Git repository in D:/acumulacion-ftp/practica-diaria/3-musica/canto/test-borrar/.git/
git add .                   # agregar contenido staged
git commit -m "mi tarea"    # Insertar cambios 
git remote add origin https://github.com/Miguelepst/git-exp-dicc.git   # vincular repositorio local con el remoto, si ya estaba definido da error
git push   origin master    # enviamos el contenido al remoto
                            # si mostrara un error 
                            # es porque no estas en una rama diferente, puede ser en vez de master la rama "main" o en otra diferente.     
                            # git push   origin main    # enviamos el contenido al remoto de la rama main
                            # Si el repositorio ya existe
                            # …or push an existing repository from the command line
git remote add origin https://github.com/Miguelepst/git-exp-dicc.git    # vincular a remoto 
git branch -M main          # -M (MOVE), Cambio el nombre del <oldbranch> to <newbranch> con force (-M), sin force (-m), master to main.
                            # otro ejemplo: 
                            # Rename your local master branch into main with the following command:
                            # $ git branch --move master main
                            # There’s no master branch locally anymore, because it’s renamed to the main branch.
git push -u origin main     # -u (--set-upstream) crea una rama de seguimiento en remoto de la rama local main y envia los commits.
                            # https://git-scm.com/docs/git-push   -u (--set-upstream)
                            # otra opcion es importar un repositorio de otro repositorio online.
                            # …or import code from another repository
                            # You can initialize this repository with code from a Subversion, Mercurial, or TFS project.
                            #Git Bash Here   Consola de Git ubicada en la carpeta local
#----------------------------------------------------
#----------------------------------------------------
git config --global -l      # git config --global --list   (-l), listar configuracion global 
                            # cuando es un comando reducido se pone un igual ejemplo: 
                            # --list seria igual a: -l
ls -all                     # ver todos los archivos inclusive los ocultos 
pwd                        # ubicacion de mi repositorio      
                           # local se utiliza para un proyecto git ya iniciado
                           # y queremos mostrar que lo que hallamos aportado fuimos nosotros
git config --global user.email none     # asigna none, como variable de correo                        
                           #satge area
                           # todo en git se basa en confirmaciones commits
                           # Retomar clase :https://www.youtube.com/watch?v=y6n4u2Ncm1M&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=3
                           # time video: 5:42 / 1:03:31
#----------------------------------------------------------------
#----------------------------------------------------------------
                           # explicacion: config en git zonas system, global y local
                           # pequeña configuracion en git
                           # por norma general las confirmaciones en git 
                           # van asociadas a un nombre y a un correo electronico.
                           # como le digo a GIT que utilice mi nombre y mi direccion de correo electronico 
                           # para asociarlas a los commit que yo realice.
git config                 # esta en tres partes la configuracion y la podemos 
                           # SYSTEM: la primera utilizada a nivel de sistema operativo
                              # SYSTEM      # raramente utilizada, no usada.                        
                           # GLOBAL: la siguiente es la opcion global se aplica a todos los repositorios de un usuario, es general a todos los repositorios de un usuario X, global     
                              # GLOBAL  
                              # es decir todos los repositorios que esten dentro de la carpeta de mi usuario, o pertenescan a un usuario usara esta configuracion en el caso de no tener definida unca configuracion local o especifica a de un repositorio.
                              # Suele configurarse una vez y no mas a no ser que se desee cambiar de usuario al estar trabajando en el pc de otro usuario.
                           # LOCAL: por ultimo la zona de configuracion LOCAL 
                              # LOCAL
                              # los cambion de mi configuracion local 
                              # se aplica a la configuracion de mi repositorio actual 
                              # es la que mas veces se va a usar en el caso de querer definir un auario especifico de un repositorio especifico local.
                           # como puedo modificar unas u otras    
git config  --zonaAModificar # ejemplo
git config --system 
git config --global       # modificaria mi fichero de usuario, afecta a todo lo del usuario
git config --local        # modifica la configuracion de mi repositorio actual, afecta a solo un repositorio especifico
                          # si yo tengo un unico repositorio 
                          # mis cambios de configuracion serian para ese unico repositorio
git config --global       # si como usuario tengo multiples repositorios, y no quiero estar configurando uno por uno de manera LOCAL, entonces hago la configuracion de git de manera GLOBAL. 
                          # Es algo asi como los niveles de confuguracion de git. Git trata de commits de cambios y de identificar la persona que genera esos cambios de versiones.          
                          # todos mis repositorios van a tener la misma configuracion
                          # no tengo que ir uno por uno                          
                          # cual es la que manda, cuanto mas cerca de repositorio mas mandamos, LOCAL es la mas cercana al repositorio,la mas alejada del repositorio es SYSTEM.
                          # en primer lugar estaria SYSTEM como la mas alejada del repositorio
                          # las opciones de SYSTEM serian sobre escritas con las opciones GLOBAL, que es mas proxima al repositorio.
                          # y las opciones GLOBAL serian sobre escritas con las opciones LOCAL, que es la mas sercana al repositorio que se este trabajando.
                          # LOCAL es lo mas cerca al repositorio.
git config --list --system    # para ver mi configuracion actual (system).
                              # parametrizar git a nivel de sistema es raro.
git config --list --global 
git config --list --local     # A nivel local dentro de la carpeta .git hay un fichero que se llama config 
                              # y de ahi es donde sale esta informacion de configuracion local al repositorio especifico
                              # cuando modificamos local, 
                              # lo que estamos modificando es ese fichero: .git/config
cat .git/config               # esta es la configuracion local 
cat $HOME/.gitconfig          # esta es la global, variable del usurio X en el sistema operativo
                              # que es cuando usamos un: git config global
                              # estamos modificando el fichero .gitconfig variable del usurio $HOME
                              # dentro de nuestro directorio de usuario
                              # en windows sera: c:/user/nombreDeUsuario($HOME)     
                              # "C:\\Users\\Equipo\\AppData\\Local\\Programs\\Microsoft VS Code\\bin\\code\"                          
                              # y cuando estamos modificando el --system 
cat /etc/gitconfig            # El archivo de configuracion gitconfig se encuentra en la carpeta /etc/gitconfig
                              # al tratar de imprimirlo en pantalla con cat me dice: que no esta definido, no esta, no lo tengo, no se ha hecho esta configuracion y es comun que sea asi, es una configuracion mucho mas generalizada, puede abarcar a todos los usurios de yn mismo systema SYSTEM, pero para que se aplicase no deberia estar definida la configuracion GLOBAL y mucho menos la configuracion LOCAL de git.                     
                              # system : lo vas autilizar cero veces.
                              # global : lo vas a utilizar una vez, configura opciones por defecto del usuaro del sistema operativo para todos sus repositorios
                              # local : lo vas a utilizar mas veces porque: 
                                # en ciertos repositorios tenes que usar (un usuario diferente sobre quien genera los commits sobre el repositorio que asi lo requiera) vuestro email del trabajo, si son cosas de trabajo 
                                # y en otros repositorios tienes que usar/mostrar vuestro email real y no el de la empresa o el de la uiniversidad.
                                # si son cosas  de proyectos open source que pueden ser vuestros personales, 
                              # como cambio yo una opcion:  
git config --list --global                    # listar, imprimir, mostrar configuracion global en pantalla            
git config --global user.name "Jose test"     # nombre de la opcion seguido del valor de la opcion 
git config --global user.name                 # visualiza opcion nombre
git config --global user.name " "             # Cambio el valor a user espacio en blanco " ", no es un unset, o reset del valor del parametro.
git config --global user.name none            # Cambio el valor a user a "none "
cat $HOME/.gitconfig                          # otra manera, # listar, imprimir, mostrar configuracion global en pantalla                  
                                              # Quiero cambiar las opciones 
                                              # referentes a un repositorio especifico, a uno particular 
                                              # quiero que se salga de la configuracion general:
git config --local user.email "vroman@noreply.users.github.com"   # cambiar configuracion email a nivel local del repositorio
cat .git/config                                # "vroman@noreply.users.github.com"  # imprimir configuracion LOCAL
git config --list --local                      # "vroman@noreply.users.github.com"  # otra manera de imorimir configuracion local 
                                               #  cuando se va a utilizar este email 
                                               # cuando yo haga un commit o una corfirmacion 
                                               # dentro de este repositorio particular
                                               # Cuando se va a utilizar el otro email, el global 
                                               # cuando haga una confirmacion 
                                               # fuara de este repositorio (que posee email en su configuracion local)
                                               # en cualquier otro repositorio relacionado a la cuenta usuario que no posea usuario configurado en su LOCAL
#------------------------------------------------------------------------------------
#------------------------------------------------------------------------------------
                                               # otros comandos implementados, requeridos EXP
git config --global --remove-section user.name ='off'         # NO funciono: eliminar al usuario
git config --global --remove-section user.name                # no funciono.  
git config --global --unset-all user.name                     # OK: es hacer un reset del valor user.name
git config --global --replace-all user.name "New User Name"   # otro comando
git config --global -e                         # Este comando abrirá el editor GNU nano o VSCODE editor si lo tienes configurado como editor de texto predeterminado para git con la configuracion global. 
                                               # de este modo puedes cambiar la configuracion del archivo 
git config --global --remove-section user      # OK: elimina la configuracion de user a nivel GLOBAL
git config --local --remove-section user       # OK:  elimina la configuracion de user a nivel LOCAL
git config --global --unset-all user.name      # no implentado
git config --global --add user.name <whatever> # no implementado
git version                                    # git version 2.38.1.windows.1
                                               # The latest version is 2.42.0.
#------------------------------------------------------------------------------------
#------------------------------------------------------------------------------------
                      # <tipo>[alcance opcional]: <descripción>
                    ### Haz tus mensajes de GIT Commit PROFESIONALES con CONVENTIONAL COMMITS
                      # El porque estandarizar, el porque de su importancia:
                      # La estructura completa del mensaje de confirmación COMMIT
                      # en Conventional Commits ayuda a estandarizar y categorizar 
                      # los cambios realizados en el código, 
                      # lo que facilita la comprensión y seguimiento de los cambios a lo largo del tiempo.  
                      # La estructura típica de un mensaje de confirmación en Conventional Commits es la siguiente:
                      # <tipo>[alcance opcional]: <descripción>
                      # Haz tus mensajes de GIT Commit PROFESIONALES con CONVENTIONAL COMMITS, 
                      # youtuber: https://www.youtube.com/@CarlosAzaustre
                      # canal de youtube: Learn JavaScript with Carlos Azaustre
                      # https://www.youtube.com/watch?v=SigVVJmUGv8 
                      # cuando no sabes que mensajes ponerles a tus commits 
                      # Herramienta: https://www.conventionalcommits.org/en/v1.0.0/
                      # El mensaje de confirmación debe estructurarse de la siguiente manera:
                      # <type>[optional scope]: <description>
                      # [optional body]
                      # [optional footer(s)]
                      #
                      # explicacion:
                      # [optional scope] El "alcance opcional" se refiere a una descripción breve y concisa de la sección específica del código que ha sido modificada en el commit. 
                      # No es obligatorio incluirlo, pero puede proporcionar información adicional sobre el cambio que se realizó. 
                      # Por ejemplo, si estás trabajando en un proyecto de software con múltiples componentes o módulos, 
                      # el "alcance" podría indicar en cuál de ellos se hicieron los cambios.
                      # Los tipos:
                      # fix : reparacion de codigo
                      # feat: nueva funcionalidad que se esta añadiendo al proyecto 
                      # BREAKING CHANGE: 
                      # types other than fix : recommends build:, chore:, ci:, docs:, style:, refactor:, perf:, test:, and others.
                      # footers other than BREAKING CHANGE
                      # Ej:
                      # feat: allow provided config object to extend other configs
                      # BREAKING CHANGE: `extends` key in config file is now used for extending other config files
#-----------------------------------------------------------------------------
#-----------------------------------------------------------------------------
                      # EXP EXPERIENCE:
git remote add origin https://github.com/Miguelepst/test1.git  # Error: ya existe
git branch -M main            # Rename your local master branch into main with the following command
git push -u origin main       # To let others see the new main branch, you need to push it to the remote. This makes the renamed branch available on the remote.               
                             ### Solucion:
git remote set-url origin https://github.com/Miguelepst/test1.git        # repositorio GitHub Internet
git remote -v                  # verificar las direcciones remotas
git config user.password ghp_mgv007r0v3Q1DrGiVQlVPSDWUWURafcJrZPs1fNbcU  # token de acceso x 7 dias caducidad.

#-----------------------------------------------------------------------------
#-----------------------------------------------------------------------------
                               # docs[]: comandos 
git config --local --remove-section user
git config --local user.name "Miguel Cartagena"
git config --local user.email miguel@noreply.com
cat .git/config
git config --global --list
git add .
git commit -am "doc: "
git push
#-----------------------------------------------------------------------------
#-----------------------------------------------------------------------------
                                       # Docs: estudio git comandos,     fuente: https://git-scm.com/book/be/v2/Git-Branching-Branch-Management
                                       # Changing the master branch name
$ git branch --move master main        # (-m) Rename your local master branch into main with the following command
                                       # There’s no master branch locally anymore, because it’s renamed to the main branch.
$ git push --set-upstream origin main  # (-u) To let others see the new main branch, you need to push it to the remote. This makes the renamed branch available on the remote.
git branch --all                       # result:
                                       # * main
                                       #   remotes/origin/HEAD -> origin/master
                                       #   remotes/origin/main
                                       #   remotes/origin/master
                                       # Your local master branch is gone, as it’s replaced with the main branch. 
                                       # The main branch is also available on the remote. 
                                       # But the remote still has a master branch. 
                                       # Other collaborators will continue to use the master branch as the base of their work, 
                                       # until you make some  further changes.
                                       # ...
$ git push origin --delete master      # After you’ve done all these tasks, 
                                       # and are certain the main branch performs just as the master branch, 
                                       # you can delete the master branch
#-----------------------------------------------------------------------------
#-----------------------------------------------------------------------------                                       
# :27) 23/08/2023 ,  # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
            # Fork :
            # Es copiar y pegar, Duplicar un proyecto.
            # yo me quiero hacer una copia de un proyecto de otra persona para poder trabajar en el.
            # porque quiero contribuir a ese proyecto.
            # pero quiero hacer cambios sin afectar a ese proyecto todavia "despues puedo solicitar que mis cambios se aplique el proyecto original el propietario del reposotorio deside si acepta o no", es un duplicar un proyecto app.
            # la ventaja de fork:
            # cualquier cambio que realices sobre el proyecto no va afectar al otro proyecto, al original,
            # tu te haz hecho tu copia, tienes tu copia y puedes generar alteraciones generar cambios, generar tus propios commits
            # que eso no va afectar al proyecto padre.  
            # bifurcacion de los proyectos de codigo abierto, potencialmente pueden haber copias infiitas.
            # si somos X personas en el mundo podrian haber x versiones de ese mismo proyecto.
            # y cada uno tendriamos nuestra propia copia de seguridad.
            # FORK: copiar y pegar de toda la vida duplicar un proyecto.
            # historias graciosas con el OPEN source que se dan:
            # de comunidades, bitcoin, 
            # muchas veces han habido proyectos en donde ha habido una parte de la comunidad del proyecto
            # que no ha estado deacuerdo con la trayectoria a la que se ha estado dirigiendo el proyecto de codigo abierto.
            # y han dicho, sabes que, como es de codigo abierto "groceria dedo propietario creador: que osden por el *** ",  
            # me voy hacer mi propio proyecto, 
            # entonces se hacen esas bifurcaciones, esas direcciones de rumbos diferentes : Buena manera de ver los FORK
            # en un momento dado haces una copia del proyecto, se bifurca al hacerle un FORK
            # ejemplo:
            # imagiraros que vas a GitHub
            # quiero explorar proyectos que sean super populares 
            # quiero aprender de esos proyectos 
            # y quiero tener una copia de esos proyectos para poder modificarlos 
            # por ejemplo vamos a tirarnos una locura Maxima
            # este proyecto me encanta y quiero aprender 
            # quiero hacer cambios sin entorpecer este proyecto 
          ### pues aqui es cuando me haria una copia de ese proyecto, me haria un fork
            # FORK 
            # Te da la opcion despues de pedirles al propietario del repositorio que integren 
            # en su repositorio un cambio que tu haz hecho.
            # esto se llama una pull request : solicito que incorporen un cambio tu yo 
            # en el repositorio central principal desde donde lo bifurcaste
            # y esto se los podria yo enviar a mis compañeros de trabajo y decirles 
            # oye estoy haciendo estos cambios que te parecen, y me podrian dar citas, sugerencias.
            # y coloborar entorno a ella
            # es muy sencillo El FORK, hacer un duplicado una copia de un repositorio externo el tu yo
            # y una vez haz hecho el fork, 
            # se comporta como un repositorio como otro cualquiera que tubieras en tu cuenta de gitHut
#--------------------------------------------------------------------------
#--------------------------------------------------------------------------
          ### Access token: para conectar nuestros repositorios locales con nuestros repositorios remotos 
            # debemos generas un ACCESS TOKEN politica got 2021
            # para poder acceder alos repositorios remotos.
            # nueva politica de seguridad conocida como access token
git init    # inicializar el repositorio 
            # lo siguiente configuraciones de identidad 
git config user.name Miguelepst                                                  # coloco el usuario que tengo asociado en GitHut, no necesariamente, no necesariamente puede ser la configuracion local de repositorio git            
git config user.email  miguelepst@hotmail.com                                    # aqui debe ir el email que tengamos asociado a nuestra cuente de GitHub, no necesariamente puede ser la configuracion local de repositorio git
git config user.password ghp_mgv007r0v3Q1DrGiVQlVPSDWUWURafcJrZPs1fNbcU          # token de cceso valido por 7 dias.
git remote add origin https://github.com/Miguelepst/git-exp-dicc.git             # Ruta: url del repositorio remoto gitHub
                                                                                 # ya esta todo configurado, provemos hacer un git add y un git push
git add .                                                                        # para agregar todo 
git commit -am probandoPat           
git push -u origin master 
#--------------------------------------------------------------------------


# :26) 22/08/2023 ,  # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
                 # work flow : una forma de trbajar utilizando git.
                 # update normal es:
                 # update --> change --> review --> commit
ls               
git pull         # lo primero que hago es un update, o un git fech ,es la parte update
git fech         # para saber si han habido cambios remotos
                 # si tuviera un repositorio remoto
                 # como no ha habido cambios ahora yo tengo que hacer los mios, tengo mi copia de trabajo local .git.
vi master1.txt   # cambio este fichero
vi master2.txt   # cambio este otro fichero
                 # como verifico mis cambios, podes usar cualquier herramienta grafica, ej: fork
git diff         # o usar esta herramienta, que cambios aun no has enviado a vuestra carpetica local: .git  , es la parte review                
git commit -am "cambio" ## es lasigiente parte del flujo
vi master1.txt   # cambio este a archivo
git diff         # lo que aparece con menos son las lineas que previamente se han sustituido
                 # cuando aparece un + son las nuevas lineas que sustituyeron la anterior
                 # reviso los cambios si estoy deacuerdo con estos cambios que hago: un git commit
                 # si no estoy deacuerdo tendre que seguir editando mi codigo fuente hasta que este deacuerdo
git diff         # sobre ficheros binarios no nos v a dejar.                 
                # al ser binarios si yo hago un cat de ellos puede salir mucha info, un chorizo un fumable
                # otro metodo es el forking work flow : le pido a una persona que meta mis cambios, es en repositorios remotos que he clonado.
                # aqui podria parecer que yo no tengo permisos para hacer algo
                # pero yo quiero contribuir y este es un proyecto OPEN source 
                # y quiero enviar ejemplos a la gente de open bootcamp
                # y yo quiero enviar un cambio "un commit al proyecto de Java basico(repositorio gitHub)"
                # pero no tengo permisos para hacerlo, que tengo que hacer.
                # pues tengo que forkearlo, hacele un "FORK"
                # hacer un fork significa que yo voy a clonar el repositorio en mi cuenta de usuario
                # se crea un repositorio del mismo nombre en mi cuenta de usuario github.
                # clonar el vuestra propia cuenta de usurio el repositorio de otra persona a la cual vosotros no tenies privilegios pero al cual queres contribuir
git clone repo  # una vez ya hecho el FORK de ese repositorio melo voy a bajar a mi ordenador con un git clone.
cd repo         #
vi ignore.lo    # voy a modificar este fichero para no perjudicar mucho a alam
git commit gitignore.lo -am "Metos los ficheros .c"
git push        # lo estoy enviando a mi cuenta de usuario, me dice que debo usar un token personal que no tengo para poder hacer el push
git push https://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  
git config --local user.name "okmiguel@noreply.user-github.com"
                # el caso es enviar el push al servidor
# :25) 21/08/2023 ,  # time video, Start: 1:39:17 , Stop: 1:50:56 , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
git cherry-pick -h       # la ayuda al comando cherry-pick, consultando otra fuente
                         # git cherry pick 💻 (ejemplo en ESPAÑOL), canal: Terminal Life 2.2K subscribers
                         # otra esplicacion cherry-pick https://www.youtube.com/watch?v=wIRufAeRntA
                         # es una herramienta de git que significa: coger ceresas 
                         # te permite aplicar commits de otras ramas en una rama principal
                         # puedes tener las siguientes ramas a lo mejor: 
                         # Ramas destinadas a unas cosas, ej:
                         # rama: estable, v1.1 de tu proyecto, base 
                         # imaginate que estas creando la version 2.0 de tu priyecto
                         # decubres un fallo de seguridad el la version 2.0 
                         # y te das cuenta que tambien afecta a la version 1.1
                         # bueno puedes aplicar ese parche de seguridad a la version 1.1 tambien
                         # simplemente cogiendo el commit(cambio, parche) de la rama parche-fix con un cherry-pick para integrarlo em la rama master o en la rama de la version deseada.
                         # en la rama base pongo el core de un proyecto, es como el corazon, la base fundamental delproyecto, es una rema con todo lo que es la estructura base.
                         # por si depronto quiero crear proyectos similares puedo reutilizar la rama base del proyecto. 
                         # y ya con la estructura base empieso hacer otro proyecto de una forma mas rapida.     
                         # feacture-plugis, caracteristica que me permite en este core, en este nucleo instalar plugings
                         # es un ejemplo real                        
git log --oneline  -10   # que remos mostras los commits de feacture-plugins (osea es una rama), no todos                
                         # asi te muestra 10 commits
                         # escoger los que queremos poner since 6am te mostrara todos los commits de ese dia desde las seis am.
                         # se han hecho estos tres commits
git log --oneline since="6am" feacture-plugins  -10           # muestrame todos los commits que se han hecho en feacture-plugins desde hoy apartir de las 6 am
                         # visualiza que se han hecho 3 commits
git log since="6am" feacture-plugins  -10   # quito el oneline para ver completo que se han hecho los cambios.
                         # reviso la descripcion de los commits: 
                         # commit: arreglar un bug, 
                         # commit: arreglar otro bug,
                         # commit: intalacion de paquete nuevo.
                         # commit: la estructura tal cual he añadido una nueva funcion
                         # pues todo esto lo uiero aplicar.
git log since="6am" feacture-plugins | cat : para que quede en pantalla para evitar regresar a colsultar nuevamente.                         
                         # como voy a ponerlos todos y no voy a tener que filtrar pongo --oneline
git log since="6am" --oneline feacture-plugins | cat                         
                         # ahora si procedemos con el cherry-pick : 4:34 minitos video time.
git cherry-pick  id-primerCommit^..Id-ultimoCommitAplicar       # combinacion de teclas (Al tGr + tilde + espaciadora): ^^  
                        # le estoy diciendo al cherry-pick que me aplique los cambios de le los commits incliyendo los commits de los extremos
                        # en este caso no ha habido confligto, de haber habido confligto 
                        # simplemente te vas al archivo y corriges el conflicto, asi de sencillo no tiene mas.
                        # la qente que usa git no la usa mucho, esta funcionalidad.
                        # pero es muy util porque te permite llevar distintas ramas 
                        # que unas no tienen los mismos commits que otras 
                        # sino que coinciden en cierta parte de la funcionalidad.
                        # y asi puedes estrapolar cambios, como lo camente antes.
                        # pierdele el miedo a los conflictos en git, eso es una chorradita.
# :25) 21/08/2023 ,  # time video, Start: 1:39:17 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
# :25) 21/08/2023 ,  # time video, Start: 1:28:36 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
                                   # cherry-pick: de una serie de commits yo voy a escoger el que mas se ajuste a mis necesidades.
                                   # git fixUrgente12345       # error: # no es un comando de git. es de donde voy a tomar los cambios         
git checkout fix-urgente12345      # cambio de rama
git log                            # en que rama se introdujo el cambio fix1.txt, cual es su ID-de-commit, copio mi hastash
                                   # abro el explorador de ficheros la carpeta mia app
git checkout master                # me cambio a mi rama master                 
                                   # en esta rama no esta el fichero fix1.txt, osea el parche para reparar una vulnerabilidad.
git cherry-pick  ID-COMMIT-CAMBIO_que_le indico     # y lo mete en mi rama actual 
                                                    # esa confirmacion de otra rama la ha metido en mi rama actual.                     
                                                    # y solamente esa cambio
git checkout   feacture-fixurgente12345
ls                                                  # hay fix1.txt, fix2.txt y fix3.txt , no he cogido todos los cambios para fusionarlo con otra rama, solo tome un cambion un commit, que poseeia un archivo. 
                                                    # Recomendacion para facilidad 
                                                    # en la la plicacion de fusiones de cambios, que los commits representes entidades de archivos completas.
                                                    # no un solo archivo que crese en tamaño de cambios internos o cambios de nombres en los archivos si es por versiones si es el caso que este inclopleto aun el archivo para cerrarlo. 
                                                    # de esta manera se prueden apreciar visualmente y no hay necesidad de introducirnos en el archivo para ver que se ha cambiado.
                                                    # que las fusiones esten representadas por entidades completas.
git log 
                                                    # podria cojer multiples hashes, si con el cherry-pick. representadas en varios archivos de entidad commit al pretender ralizar una fusion y no este tan oculta.                                                     
                                                    # una fusion debe de representar archivos nuevos en la rama en la que se va a fundir, los cuales no estaban antes de la fusion
git log --oneline | cat                             # | cat : los voy a pasar aqui para tenerlos en pantalla                                                    
checkout master                                     # como haria un cherry-pick de multiples commits, multiples archivos a fusionar en una rama nueva.
                                                    # identificar nombres de archivos con referencia a si rama origien en sus nombres, para cuando esten fusionados en la rama master sepas de que rama fue generado.
git cherry-pick ID-CommitAAplicar1  ID-CommitAAplicar2  # fusionar multiples commit 2 o hasta mas elegidos   
                                                    # puedo cojer un intervalo de commmits SI.
reset --hard  HEAD~2                                # he revertido el historial 
git log 
git checkout fix-urgente12345                       # sigo teniendo esta rama.
git checkout master
git cherry-pick ID-CommitAAplicar1  ID-CommitAAplicar2 
git checkout fix-urgente12345   
git log --oneline | cat
git checkout master 
git checkout fix-urgente12345 
touch fix3.txt
git add fix3.txt
git commit -am "fix3.txt"
git log --oneline | cat                              # tengo tres cambios en esta rama
git checkout master                                  # ma voy a mi rama master y voy aplicar un cherry-pick por rango para fusionar varios commit de la rama enterior a mi rama master, estos commit estan unificados en archivos.
                                                     # cada commit a fusionar en la master que proviene de otra rama esta referenciado a un archivo entero como minima unidad completa de fusion.
git cherry-pick  id-primerCommit*..Id-ultimoCommitAplicar  # pongo el primer comit que quiero aplicar el mas profundo en la pila de commits de la rama dedonde los voy a extraer.                
                                                      # y luego el ultimo commit que quiero aplicar, eso me toma los commits en el medio de esos dos extremos, seria por fusion rango.                      
                                                      # error
git cherry-pick  --abort                              # no habias terminado los de antes, por eso el error      
git cherry-pick  --quit
git cherry-pick  id-primerCommit*..Id-ultimoCommitAplicar  # ahora si ahi estan los archivos adicionados directorio ruta master : fix1.txt, fix2.txt y fix3.txt
git cherry-pick  --quit                               # ya esta el cherry pickeado
                                                      # que mas podemos hacer aplicar los mismos cambios pero sin incluir el inicial y el final
git checkout fix-urgente12345 
git log --oneline | cat                                   # Aplicar fusion,parches sin elegir el parche commit que hay en los extremos, sin incluirlos.                                                     
git cherry-pick  id-primerCommit..Id-ultimoCommitAplicar  # igual pero no se coloca el asterisco circomplejo, lo que valla entre los dos commits pero sin incluir ninguno de los dos.
git cherry-pick  id-primerCommit*..Id-ultimoCommitAplicar # lo que valla d este commit al otro incluyendo los dos.
                                                          # es solo cuention de cogerle el gustillo, porque es curioso
git reset --hard HEAD~2                                                          
git cherry-pick  id-primerCommit..Id-ultimoCommitAplicar  
                    # como es un cherry-pick a nivel grafico, no lo esta mostrando el app fork.
                    # si generamos habitualmente parches para diferentes versiones es comun usar el cherry-pick
                    # ramas de mantenimiento como se suelen llamar
                    # ir moviendo parches de una parte a otra.
                    # el cherry-pick es muy potente por esta rason de ejemplo que si entiendo: 
                    # time video: 1.39.0. y tiene muchisimo uso.
                    # para que utilizamos cherry-pick:
                    # si generamos habitualmete parches en lugar de una rama de parches
                    # ese parche se tiene que aplicar a cuatro o cinco ramas a una version 
                    # es un parche para el que afecta alas versiones 1.0, 1.1, 1.2, 1.3, 1.4, 1.5 las cuales son commits
                    # constantemente estoy haciendo una nueva version para venderla de mi software, estilo windows. 
                    # pues iremos utilizando en esas ramas especiales ramas de mantenimiento "ramas de creacion de fix de parches para la aplicacion"
                    # pues el chery-pick para ir moviendo parches de una cosa a otra.
                    # imaginate tambien que estas desarrollndo la version 2.0
                    # y al mismo tiempo la version 1.1 de vuetro software
                    # ha vez lanzado al mercado la version 1.0
                    # el desarrollo sigue, la version 1.1, 1.2 etc..
                    # y al mismo tiempo que haz lanzado la version 1.0 
                    # comensais la rama de desarrollo de la version 2
                    # resulta que hay un cambio de lesgislacion 
                    # y tenes que meterle nueva funcionalidad en la version 1 
                    # para no dejar a vuestros clientes colgados. 
                    # inicias una nueva rama de desarrollo, la rama 1.1  tipo fix parche.
                    # y en esta rama 1.1 añadis esta nueva funcionalidad
                    # y vas corrigiendo otras series de parches, de cambios, corrigiendo bugs 
                    # que han podido solucionarse o introducirse nuevos.                                     
                    # bueno como en la version 1.1 hemos introducido nueva funcionalidad. 
                    # posterior al lanzamiento de mi rama 2.0
                    # yo no puedo tener una version 2.0 que elimine funcionalidad previa.
                    # seria de locos que tubiera una version 2.0 con menos funcionalidades que la version 1.0
                    # bueno pues tendria que irme mirando en mi historial de comfirmaciones de la version 1.1
                    # que cambios añaden que funcionalidad
                    # para hacer un cherry-pick de esos cambios y meterlos en la rama 2.0
                    # para que la rama 2.0 tenga esa funcionalidad nueva,
                    # pero que no importe(envie) otras cosas de la version 1.1 que podremos haber solventado.
                    # o que ni siquiera estarian en la 2.0 porque esos fallos no se han introducido en la version 2.0
                    # por eso es tan importante utilizar el cherry-pick
                    # algo diferente al cherry-pick es:
                    # editar el codigo fuente a mano buscar las diferencias a mano
                    # y mover los cambios a mano.
                    # cuando hacemos esto como todo humano nos equivocamos mucho
                    # es mas facil si una maquina lo hace por nosotros
                    # cherry-pick : nos permite hacerlo de una form mucho mas automatica.
                    # la verdad es que es muy potente el cherry-pick
                    # y tiene muchicimo uso
                    # dicho esto vamos a irnos a cosas mucho mas sencillitas.                                    
# :24) 20/08/2023 ,  # time video, Start: 1:28:36 , Stop: 1:39:17 , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
git help     
                  # usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]     
                  #          [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]    
                  #          [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
                  #          [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]       
                  #          [--super-prefix=<path>] [--config-env=<name>=<envvar>]
                  #          <command> [<args>]
                  # These are common Git commands used in various situations:
                  # start a working area (see also: git help tutorial)
                  #  clone     Clone a repository into a new directory
                  #  init      Create an empty Git repository or reinitialize an existing one   
                  # work on the current change (see also: git help everyday)
                  #  add       Add file contents to the index
                  #  mv        Move or rename a file, a directory, or a symlink
                  #  restore   Restore working tree files
                  #  rm        Remove files from the working tree and from the index
                  # examine the history and state (see also: git help revisions)
                  #  bisect    Use binary search to find the commit that introduced a bug       
                  #  diff      Show changes between commits, commit and working tree, etc       
                  #  grep      Print lines matching a pattern
                  #  log       Show commit logs
                  #  show      Show various types of objects
                  #  status    Show the working tree status
                  # grow, mark and tweak your common history
                  #  branch    List, create, or delete branches
                  #  commit    Record changes to the repository
                  #  merge     Join two or more development histories together "Unir dos o más historias de desarrollo."
                  #  rebase    Reapply commits on top of another base tip "Volver a aplicar confirmaciones encima de otra punta base"
                  #  reset     Reset current HEAD to the specified state
                  #  switch    Switch branches
                  #  tag       Create, list, delete or verify a tag object signed with GPG
                  # collaborate (see also: git help workflows)
                  #  fetch     Download objects and refs from another repository "Descargar objetos y referencias desde otro repositorio"
                  #  pull      Fetch from and integrate with another repository or a local branch "Obtener desde e integrar con otro repositorio o una rama local"
                  # push      Update remote refs along with associated objects "Actualizar referencias remotas junto con los objetos asociados."
                  #  'git help -a' and 'git help -g' list available subcommands and some concept guides. See 'git help <command>' or 'git help <concept>' to read about a specific subcommand or concept. See 'git help git' for an overview of the system.
                  # {"practica-estudio" :"1 hora repaso contenido hasta lo presente observacion"}
git status                  
git add EXP-WORKPACE-DICC.md
git status
git commit -am "transaccion"
git push
                  # "fatal: No configured push destination.", no existe repositorio centrar remoto.
                  # Either specify the URL from the command-line or configure a remote repository using
                  # git remote add <name> <url>
                  # and then push using the remote name
                  # git push <name>
                  # Ruta repo bare: D:/acumulacion-ftp/repositorios/exp-git/
git clone  D:/acumulacion-ftp/repositorios/exp-git/ miapp           # crea carpeta miapp he introduce el repo ahi.
git clone  D:/acumulacion-ftp/repositorios/exp-git/ .               # no crea crpeta, en la ruta en la que estas crea el repositorio                  
git remote add exp-git D:/acumulacion-ftp/repositorios/exp-git/     # repositorio bare
git push          
                   # "fatal: The current branch master has no upstream branch."
                   # To push the current branch and set the remote as upstream, use
                   #     git push --set-upstream exp-git master
                   # To have this happen automatically for branches without a tracking 
 git push --set-upstream exp-git master             # Done
                   # Enumerating objects: 13, done.
                   # Counting objects: 100% (13/13), done.
                   # Delta compression using up to 4 threads
                   # Compressing objects: 100% (13/13), done.
                   # Writing objects: 100% (13/13), 24.38 KiB | 242.00 KiB/s, done.
                   # Total 13 (delta 3), reused 0 (delta 0), pack-reused 0
                   # To D:/acumulacion-ftp/repositorios/exp-git/
                   # * [new branch]      master -> master
                   # branch 'master' set up to track 'exp-git/master'.
git push           # Everything up-to-date                   
                   # Se vinculo un repositorio local a uno central "remoto" (bare)
                   #
touch fix1.txt 
git add fix1.txt
git commit -am "fix1.txt"                   
touch fix2.txt 
git add fix2.txt
git commit -am "fix2.txt"                   
git checkout 
checkout master             # me vualvo al master, y mi desarrollo va a seguir avanzando de for ma virtual
touch master2.txt 
git add master2.txt
git commit -am "master2.txt"                   
touch master3.txt 
git add master3.txt
git commit -am "master3.txt"
# :24) 20/08/2023   # time video Start: 1:28:36  Stop: --:--:--  Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
                        # muy usada en entornos profesionasles, la caracteristica git STAGED
ls altr            
vi otrofichero.txt      # Estoy cambiando este texto 
vi branch1.txt          # tambien estoy cambiando este texto "ajusto documentacion etc.."
git status              # me lista ficheros modificados, pero que de repente no he terminado de modificar, de repente suena el telefono y le alejo de ellos
                        # me mandan un caorreo urgente, y me dicen: tio, tio, tio urgente te tienes que poner 
                        # y arreglar el fichero branch2.txt es urgentisimo tienes que comitearlo lo antes posible 
                        # da igual lo que estubieras haciendo tienes que pararlo para hacer esto que es mas importante. 
                        # vale, no he terminado de modificar estos ficheros 
                        # y ya me estan pidiendo que modifique otros porque es urgente
                        # y aqui me surge el problema, pierdo lo que estaba adelantando por hacer lo urgente.
                        # puedes solicionarlo de dos formas la cambona es que copias lo que ya tienes hecho 
cp -prf miapp miapp2
cd miapp2 
git status 
git reset --hard            # pierdo mis cambios 
                            # hago aqui los cambios los commiteo, soluciono lo que hera urgente 
                            # hago una copia de mis ficheros que ya estaban modificados aqui.
cp ../miapp/branch1.txt .                        
cp ..miapp/otrofichero.txt .
                            # y sigo trabajando, pero esto no es practico, y menos en repositorios grandes.
rm -rf miapp2               # es un muy mal ejemplo
clear                       # como se debe hacer.
git status                  # igual caso anterior
                            # resulta que: 
                            # yo no puedo hacer un commit de esto
                            # porque no lo he terminado, y podria romper el trabajo de otros 
git reset --hard            # pero no quiero hacer esto, porque perderia todos mis cambios                
                            # bueno como se hace.
git stash                   # me deja un directorio de trabajo limpio.          
git status                  # limpio, nothing to commit, working tree clean.
                            # lo que he hecho previamente no esta commiteado pero tampoco esta perdido
                            # esto es trabajo paralelo. 
                            # esta stasheado en una estructura de pila en memoria.
                            # aqui yo ya puedo trabajar en la urgencia solicitada. 
vi branch2.txt              # arreglalo es muy importante "cambio Hiper urgente".   y en cuanto lo tengas tienes que commitearlo.                     
git add branch2.txt
git commit -am "branch2.txt cambio super urgente"
git log                     # listo aqui esta mi cambio super urgente.
                            # y como puedo yo ahora volver a donde estaba? a lo previo que no podia commitear porque no lo habia terminado.
git stash apply             # aplica los cambios que no tenia commiteados sobre los cambios que tengo actualmente.                            
git log                     # commit cambio super urgente sigue ahi.
                            # pero ya puedo seguir trabajando con lo que estaba haciendo antes. 
vi otrofichero.txt          # sigo pretendiendo terminar lo que estaba haciendo antes para poder comitearlo.
                            # "texto ahora si que me han dejado termino de hacer mi trabajo comodamente"
git commit -am "cambio cierto texto"                            
git log                     # ya esta no he perdido ningun cambio
                            # esta muy bien porque yo puedo tener estas interrupciones y no quiero commitear algo porque no esta terminado.
clear
                            # podes tener multiples stashes SI, estos son apilables.
git stash list              # para ver que staches tengo.                            
                            # stash #(0) MIP on master: idCOMMIT merge branch 'nueva rama' 
                            # el nombre del stash se lo puedo dar yo, pero por defecto 
                            # es el nombre del ultimo commit
git satash apply            #                            
git stash clear             #                            
git stash list              # aqui no pone nada.
git stash save "Estoy creando el login"   # crear un stash con nombre concreto.
git merge
git reset --hard
clear
git stash save "Estoy creando el login"   # no lo puedo hacer porque no hecho cambios, no hay cambios locales 
echo texto > vacio.txt 
git status
git stash save "Estoy creando el login"   # crear un stash con nombre concreto. OK
git stash list                            # 
ls                                        # estoy haciendo otros cambios super importantes cuando me piden otro mas super importante 
vi otrofichero.txt
git stash save "algo mas importante que lo anterior importante :-)"   # crear un stash con nombre concreto. OK
git stash list                            # stash #(0) MIP on master: algo mas importante que lo anterior importante :-) 
                                          # stash #(1) MIP on master: Estoy creando el login 
                                          # es como una pila de folios.
git stash pop                             # aplicariamos el actual de la cabeza de la pila de satsh., lo saca de la pila de stash.
git stash list                            # stash #(0) MIP on master: Estoy creando el login              
git stash pop 
git stash list                            # no visualiza nada ya no hay stash.
                                          # cuando uso el pop no tengo que hacerle el clear.
git stash apply -h                        # ayuda, manual de git stash apply --index  (0, 1, 2, 4), eliges el que quieres dentro de la pila de stash
                                          # con este apply luego tendras que hacer un clear para eliminar la pila de stash.
                                          # que mas les vamos a contar (Tenemos mucho).
                                          # bueno resumen:
                                          # ya sabemos como trabajar con:
                                          # ramas, merge, rebase, stash
                                          # vamos a hacer cosas chulas vamos a la rama
clear                                     # cherry picking, recogida de ceresas, consiste en lugar de fucionar ramas enteras, 
                                          # voy a fucionar commits concretos     
                                          # ejemplo concreto: los famosos parches de seguridad de windows.
rm -rf * .git                             # y
                                          # vamos a crearnos otra estructura git para practicar este ejemplo                                          
git init .
touch master1.txt
git add master1.txt                                          
git commit -am "master1.txt"
git checkout -b fix-uergente12345
touch fix1.txt
# :23) 19/08/2023 ,  # time video start: 1:01.23 , Stop: 1:28:36,  Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
               # hayg gente que considera que estos commit autogenerados con el merge son superfluos, no les gusta ver esos commits.
               # que herramiente nos permite hacer un merge re-escribiendo el historial de confirmaciones "git rebase".
               # objetivo del revase: cuando hagamos el MERGE, el commit del HEAD no se vea afectado por otro commit automatico. 
               # vamos hacerlo
rm -rf * .git  # empiezo desde cero me cargo todo.
ls
               # ESTAS SON LAS MEJORES PARTES DE GIT
git init . 
git status
clear
touch master1.txt
git add master1.txt
git commit -am "master1.txt"   # mi primer puntico
git checkout -b feacture-primeraRama
touch branch1.txt 
git add branch1.txt 
git commit -am "branch1.txt "   
touch branch2.txt 
git add branch2.txt 
git commit -am "branch2.txt "   
git checkout master           # regreso a mi rama master a crear otro puntico de commit 
touch master2.txt 
git add master2.txt 
git commit -am "master2.txt "   
                                  # Ojo, vamos ha hacer un MERGE una Union de ramas pero:
                                  # No queremos que nos genere un nuevo commit, por ser un commit superfluo, solo me dice que se a mergeado una rama nada mas.
git rebase feacture-primeraRama   # seguido de la rama que vamos a re-basear.  y ya esta.        
                                  # rebobinando la cabeza "HEAD" para cumplir unir los cambios commits que has hecho, applying master2.txt
                                  # al ir a fork mi historial ahora es totalmente plano, lineal.
git log                           # ya no hay ningun commit que me ponga mege branch       
                                  # esto se llama historico lineal, es muchas veces lo que queremos.
                                  # rebase, siempre lo vamos a intentar utilizar siempre en nuestro repositorio local.
                                  # cuando trabajemos con compañeros con proyectos grandes vamos a trabajar siempre con ramas
                                  # las ramas cuando las trabajemos para nosotros mismos de manera local las vamos a trabajar con rebase
                                  # MERGE en remoto, REBASE en local
                                  # el historial de un proyecto open source no se puede rescribir.
                                  # por razonas de al hacer un rebase nos carguemos codigo importante, por hacer un replay del historial.
                                  # REBASE tambien nos permite cometer errores y borrar cosas sin quererlas
rm -rf .git 
                                  # copy-paste   igual que el anterior                                  
git merge feacture-primeraRama    # nos queda en el fork un dibujito perfecto, las dos ramas se unen en una sola que representa ser la rama master, se fusiona la rama con el la master.
rm -rf .git                       # para utilizar un merge.
ls -altr
rm -rf * .git  
copy and past "script commits"
git rebase feacture-primeraRama   # el historial es plano, linea recta no hay figura unificada en el head del master
                                  # puede pasar que yo quiera hacer cambios en mi rama, bueno mi rama sigue existiendo 
                                  # al hacer rebase o el merge, las ramas siguen existiendos, no he eliminado esas ramas
                                  # asi que puedo cambiarme de nuevo a esa rama. 
                                   # git branch feacture-primeraRama                                  
git checkout feacture-primeraRama  # Como yo estoy en esta rama puedo seguir tranajando en esta rama.
                                  # vamos a crear nuevo fichero.                                
touch branch3-nuevo.txt                                   
git add branch3-nuevo.txt                                   
git commit .am "modifico mas caosa branch3-nuevo.txt"
                                  # y me vuelvo a mi git master
git checkout master               # de forma visual en fork puedo ver que he vuelto a bifurcar mi codigo                                  
                                  # puedo hacer exactamente lo mismo tengo dos opciones git merce o rebase.
                                  # al yo saber que mi rama merge nadie mas ha tocado yo podria hacerle un merge y va aparecer lineal, fost forward
                                  # ho no me deja hacer un fast fordware, bueno pues nada hagamoslo de la otra forma
merge branch                                   
git log 
                                  # el el divujito de fork volvemos a ver como se fusiona la rama y cierra la figura no lineal.
git log --oneline --graph         # formato de reporte git mas bonito, grafico dibujo
                                  # voy a mover miapp.old
mv miapp miapp.old                                   
cp -pr miapp-ramas miapp          # voy a copiarlo para que no se borre
cd miapp
ls -altr
                                  # yo puedo fusionar ramas tambien
git rebase feacture-rama-mejora   # o merge            
                                  # y aqui me aparece como secuencial 
git merge nueva-rama              # y ahora no lo hago secuencial
git log --oneline --graph         # tambien podemos ver las cosas que estamos haciendo.
# :22) 18/08/2023 ,  # time video: 1:01.23 , Stop: 01:15:06 , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
                                      # no lo voy hacer porque no tengo configurado ningun ORIGIN, ruta del servidor remoto en la configuracion de mi .git
                                      # pero suponiendo que si, haria: ORIGIN es el repositorio remoto: GitHub, GitLab, -Bare  ETC..
git pull origin  nombreDeLaRama                
git checkout nombreDeLaRama         # asi es como trabajarias con una rama que no estubiera en tu repositorio, que estubiera en otra parte.
cd ..
mv miapp miapp.rama                 # voy a renombrar mi carpeta, para empezar con una cosa llamada Branching 
                                    # BRANCHING(hacer un monton de ramas), ramificacion y unificacion
                                    # cuando yo termino de desarrollar una rrama feacture quiero que los cambios (commit), se pasen al HEAD de la rama MASTER.
                                    # quiero unificar la rama feacture en la rama master, como lo vamos hacer.
                                    # cuandro trabajamos nosotros mismos usamos git revase,
                                    # cuando trabajemos para una corporacion usamos git MERGE
                                    # voy a crearme un repositorio nuevo.
mkdir miapp
cd miapp
git init .                          # voy a inicializar el repositorio                                    
touch master1.txt 
git add master1.txt
git commit -am "master1.txt"
touch master2.txt 
git add master2.txt
git commit -am "master2.txt"
clear
                                    # voy a trabajar en algo nuevo que me han pedido, pero como no me gusta contaminar mi rama principal.
                                    # no me gusta contaminar mi rama principal.
git checkout -b featurePrimeraRama  # Lo que hago es crearme una rama adicional, una rama extra.
                                    # si no existe la rama la crea, si existe se cambia de rama.
rm add                              # elimino este fichero que he creado sin querer.
ls                                     
touch branch1.txt                   # vamos a crearnos ficheros aqui tambien en esta rama.
git add branch1.txt
git commit -am "meto branch1.txt"   # BRANCHEADO es crear ramas, osea que hemos brancheado.
touch branch2.txt                   # vamos a meter otro punto historico mas, osea hacer otro commit.
git add branch2.txt
git commit -am "meto branch2.txt"
                                    # FUSIONAR MIS CABIOS, ahora quiero fusionar mis cambios. 
                                    # miro el fork 
                                    # cambiar de rama, voy ha hacerme otro checkout master, en master no estan los ficheros que tenia en la rama anterior.
git merge feacture-primeraRama      # me hapuesto los archivos de la otra rama 
                                    # en mi rama master a fusionado la rama feacture-primeraRama
                                    # utilizando el metodo fast forwared, ademas me dice que me ha ceado estos dos ficheros.
git log                             # no parece que halla hecho nada. porque hemos hecho un merge por fast foward, este me da un historial plano       
                                    # fast foward es como i nunca hibiese existido una rama para unirla con master, es como si todo ubiese sido creado en la rama master incluyendo los commits de la rama que habia sido creada.
                                    # esto ocurre porque en mi ama master no he realizado ningun cambio, commit, lo contrario a esto crea un merge de otra forma diferente a fast foward      
                                    # el merge por fast fowar es el meger ideal, pero no siempre se crea asi, pero es muy raro su aplicacion (Que este trabajando en una rama y no halla cambios en master).
                                    # los merges hacen avanzar a una posicion es un commit mas pero implicito.
rm -rf * .git                       # voy a borrar todo esto, me lo cargo enterito                                    
git init .
touch master1.txt 
git add master1.txt
git commit -am "master1.txt"
git checkout -b feacture-primeraRama
touch branch1.txt
git add branch1.txt
git commit -am "branch1.txt"
touch branch2.txt
git add branch2.txt
git commit -am "branch2.txt"
git checkout master 
touch master2.txt                    # lo diferente, ahora voy a crearme otro fichero en master para que impedir que el metodo de merge sea "fast foward"
git add master2.txt
git commit -am "master2.txt"         # ya el MERGE no lo puedo hacer directamente sobre el HEAD de master por que el HEAD ha avanzado un commit mas del commit en donde se genero una rama que se desea mergear (unificar con el master en su head).
clear
git merge feature-primera-rama       # no ha dicho nada de fast forward, de hecho me esta diciendo que me va a generar un nuevo commit
                                     # me ha puesto como mensaje: merge branch "feacture-primeraRama"    , le digo que si.                                         
git log                              # ha cambiado, en este caso no ha podido aplicar el mergen sobre el origen de la rama, porque la rama master ha estado creciendo en su historico de commit, gracias a otros programadores.                                     
                                     # genera un commit nuevo en la rama master a unificar, y en este comnit nuevo es donde va estar el contenido de mi raa ahi la he metido.
                                     # informa: merge made by 'recursive' strategy, lo ha aplicado de forma recursiva de una rama sobre otra.
                                     # antes era mas simple me habia puesto: fast foward, porque habia podido hacer el merge directamente sobre la babecera, no habian commits nuevos en  la rama master.
                                     # la rama master ha sigido evolucionando creciendo su historico de commits de cambios.
                                     # la otro forma de unificar es: revase, son dos formas, 
git commit -am "transacción commit"  # cuando no sabes que nombre ponerle a tu commit, solo es transaccion de contenido diario o por evento.                                     
# :21) 17/08/2023 ,  # time video: 31.17 , Stop: 1:01:23 , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
                                    # Estamos ubicados en la rama: NombreDeLaRama
touch branch1.txt   
git add branch1.txt                 # se vanañadiendo los archivos a la carpeta 
git commit -am "branch1.txt "
touch branch2.txt   
git add branch2.txt                 # se vanañadiendo los archivos a la carpeta 
git commit -am "branch2.txt "       # En la rama: NombreDeLaRama, a esta rama la he aumentado dos puntos en si historico de commit.
git checkout master                 # Como puedo cambiar de la rama: NombreDeLaRama a otra rama diferente. 
                                    # parece que desaparece los archivos que cree en mi rama: NombreDeLaRama, pero no es solo que estoy en una rama en donde esos archivos no fueron creados, no existen, esos doscommit cambios no pertenecen a la rama master. 
git checkout NombreDeLaRama         # al volver a cambiar a esta rama: NombreDeLaRama, los archivos vuelven a aparecer, porque esos dos commit que crearon esos dos archivos fueron hechos en esta rama.                                               
ls 
git checkout master
ls                                   # vuelven a desaparecer, aqui en esta rama no se ven esos dos archivos. 
touch master1.txt 
git add master1.txt
git commit -am "master1.txt"
echo mensaje > master1.txt
git commit -am "meto texto en master1.txt"   # hemos puesto otro puntico, otro paso en el historico de cambios del repositorio local, en la rama master. 
                                    # yo sigo dearrolando en paralelo, al disponer de dos ramas(la master y NombreDeLaRama )
                                    # En cada rama veo las cosas totalmente independiente a la anterior o entre ellas.
                                    # git fork, si nos fijamos en el cliente grafico de git "Fork"                                    
                                    # ya el el arbol se ve de una manera distinta, visualiza dos ramas y mus puntos de cambios, commits en su historico.
                                    # vamos a crear otra rama mas pero la craremos de otra forma
git branch nombreRama                                    
git chekout nombreRama
git checkout -b nombreDeLaRama-Fix12345      # otra forma de crear rama, como si estubieramos creando un fix (reparacion, arreglo)
                                    # cambia ala rama: nombreDeLaRama-Fix12345, si la rama no existe la crea, gracias al -b "flag", no se puede cambiar una rama que no existe.
                                    # he creado esta rama desde la rama master, en la que estoy ubicado.
                                    # vamos a meter un par de commits en esta rama.
touch nombreDeLaRama-Fix12345.txt   #
git add nombreDeLaRama-Fix12345.txt
git commit -am "nombreDeLaRama-Fix12345.txt"
echo "Esto lo arregla" > nombreDeLaRama-Fix12345.txt
git commit -am "meto texto nombreDeLaRama-Fix12345.txt"     # hemos hecho dos commits
git checkout featura-demo           # me cambio a la rama: featura-demo (nombreDeLaRama, se usa un nombre diferente)
git checkout master                 # me cambio a la rama master.
git checkout master nombreDeLaRama-Fix12345  # me cambio a la rama: nombreDeLaRama-Fix12345
                                    # puedo crearme una rama de un commit previo al HEAD de la rama en la que me encuentre, elegido si.
git checkout master                                    
git checkout ramaQueNoExiste        # No se puede sale error
                  # Lo primero a hacer es elegir mi commit de inicio del cual deseo que brote una nueva rama que quiero crear.
git log --oneline --graph           # selecciono cual va ha ser mi commit en el que deseo sembrar una rama       
git branch nueva-rama ID-commit-desdeDondeVaSurguirLaRama    # Commit ID 
git checkout neva-rama
touch otro-fichero.txt
git add otro-fichero.txt
git commit -am "Meto otro fichero otro-fichero.txt"
echo hola > otrofichero.txt
git commit -am "Meto texto en otro-fichero.txt"  # de una misma rama podemos ir llendosnos al infinito y mas aya.
                # tambien podemos crear una rama dentro de otra rama
git checkout master 
git checkout feacture-demo
git checkout -b feacture-demo-mejorada
touch texto.txt
git add touch texto.txt
git commit -am "Meto texto texto.txt"     # y nos hemos creado dos commit en esta rama que deriva de otra rama
                                          # Podemos crear ramas de ramas y de ramas y de ramas, etc...
                                          # el numero al que podemos llegar es increible
                                          # fork muestra como esta cada una de las ramas en el tiempo con crecimiento en forma de pila hacia arriba
                                          # una rama hereda los comentarios de su rama anterior 
git log
git checkout master
ls
echo mensaje > master1.txt                 
git add master1.txt                         
git commit -am "Cambio texto en master1.txt"  # lo comun no es que desarrolles en master 
                                              # lo comun es que cada vez que vallas a inexar un cambio crees una rama
                                              # y despues de crearos una rama, fusiones (merge) los cambios en la rama principal, que es la rama master.
                                              # que es esto de fusionar cambios: es metertodos los cambios de una rama (sus commits de historico) 
                                              # SIempre que sea posible en otra rama.
                                              # como podemos utilizar las ramas de forma remota, hasta hora solo la hemos utilizado en mi repositorio local, mi carpeta .git.
                                              # comopodemos trabajar con los remotes, de momento se que tengo toda mi copia de trabajo en local, .git.
                                              # como ya sabemos git es "un sistema de ficheros distribuidos" 
                                              # es decir hasta que yo no henvie mis cambios a mi repositorioremoto si es que lo ubiera.
                                              #solamente van a permanecer en mi carpetica.
                                             # time video: 31.17 , Stop: 46.25 , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
                      # :20) 16/08/2023 Miercoles
git commit -am "textos 2"
echo mas lineas 3 >> fichero1.txt
git commit -am "textos 3"                 # fijaros que el historial de confirmaciones va avanzando, punto a punto, en fork hacia arriba, los ultimos commit van a lo mas profundo de la pila.
                                          # com buscamos aqui los fallos
git log                                   # no me dice mucho , no lo tiene muy claro, quien ha metido un bug, un error.                                          
                                          # biseccionar los cambios entre dos commit, (un commit mas actual "Que no funciona porque tiene un error" con otro commit mas antiguo que di funciona ).
                                          # cojemos el ultimo commit bueno conocido: id de commit: 14fAb45  
clear
git bisect start                           # Empieza la biseccion, parece que no pasa nada pero si esta pasando.                                           
git bisect good 14fAb45
git bisect bad  af234f                     # el commit en el que dejo de funcionar id: af234f esta mas certa al HEAD 
                                           # he puesto pocas revisiones.
ls
cat mifichero1.txt                          # solo tengo dos lineas.                                           
git bisect bad                              # si yo creo que este es el fichero que que esta mal, hago este comando y ya esta
                                            # el commit actual es el primero de los commits malos
                                            # me saca otro commit mas, como lo miro
ls
cat mifichero1.txt 
git bisect good                             # este funciona bien, tenia que haber creado un commit mas al haber uno no lo puedo hacer.                                            
                                            # Es solo para marcar cuales son los buenos y cuales son los malos commits
clear                                            
ls                                          # nos permite saber quien ha hecho que, este comando es muy potente.
git blame mifuchero1.txt
cat mifichero1.txt
git blame mifichero1.txt                    # en que commit, quien, en que fecha y hora metio ese cambio
                                            # blame en english es culpa
                                            # voy a tomar otro repositorio que ya tengo preparado, lo he escogido porque es un repositorio immenso, tiene mucho codigo fuente.
git blame mode.py                           # escojemos cualquier fichero, el aveces tarda un rato porque tiene que recorrer un monton de historia que ha pasado, este comando es muy intensivo a nivel de disco duro..                                            
                                            # para ver el historico del fichero mode.py, demanera que si debo preguntar a alguien que me explique cierto cambio que introdujo lo puedo hacer, porque se hace tal cosa asi o lo que sea..
                                            # regresamos a nuestro repositorio
rm -rf  miapp                               # empezando a trabajar con las ramas, aqui git brilla, es una bifurcacion de mi historial de transacciones, de confirmaciones, de commits.
                                            # de forma que yo pueda tener varios historiales de confirmacion paralelos y no mexclados entre ellos.                                            
                                            # se usan para tener multiples veriones de desarrollo, tambien podemos creanos una rama para corregir un error..
                                            # y luego meter esos cambios que hemos hecho en nuestro codigo principal, nuestra rama principal, el tronco del arbol, la rama master por defecto, es nuestro tronco del arbol. 
git init .                                  # inicializa mi repositorio en master.                                             
git status                                   # podes var en que rama estas: On branch master, no commits yet
git branch                                  # Como podemos ver las ramas que yo tengo, muestra nuestras ramas actuales, hactualmente no tengo nada de nada , no tengo ramas, estoy en el tronco del arbol.
git branch nombreDeLANevaRamaHaCrear        # Como puedo crear una rama, hay dos formas 1 usar git branch
                                            # Error, no es un objeto valido, pasa cuando no tnes ningun commit previo en vuestra rama de trabajo en la rama master.
                                            # y se solventa de manera rapida con
touch vacio.txt  
git add vacio.txt
git commit -am "creo fichero vacio"                                            
git branch nombreDeLANevaRamaHaCrear        # ahora si ya no se queja, ya me deja crear la rama nueva
git branch                                  # mirar las ramas que tengo: estoy en rama master y tengo una rama que se llama: nombreDeLANevaRamaHaCrear
git status                                  # para saber en que ramas estamos ubicados, en que rama estamos trabajando 
                                            # On branch master  
git branch                                  # tambien lo podemos usar para esto. * master
git checkout NombreDeLaRama                 # y como cambio yo de una rama de trabajo a otra.
git status                                  # On branch NombreDeLaRama
git branch                                  # *NombreDeLaRama, cada vez que haga un cambio estos cambios van a estar en esta raama y no en la rama master.
                                            # vamos hacer unos cuantos cambios, unos cuantos commits y utilizamos fork tambien
                                            # rama NombreDeLaRama a un no posee su primer commit
                                            # time video: 16.56 , Stop: 31.17 , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
                      # :19) 15/08/2023

git log --oneline            # ver registro historico y quiero volver al commit o estado: id#_commitElegido, me pongo a contar las posisiones que quiero retroceder al pasado, el numero de commit a los que deseo ignorar, cuento del head, de arriva hacia abajo, voy a desacer tres cambios, tres confirmaciones, tres commits, para ubicarme en el cuerto commit y que mi HEAD se ubique en este cuarto commit, porque los otros 3 (commits) los considero que fueron errores. 
git reset --soft HEAD~3      # elimino tres commits, para quedar ubicado en el cuarto commit con el HEAD.  la tilde (~) mas el numero de cabeceras hacia atras, en el pasado del historico de commits.
git commit -am "cambios"     # fme hecho los ficheros hacia atras, los saco del staged.
git log
git log --oneline            # te das cuenta que desecha el historial hacia atras, hacia el pasado, pero no ha borrado los archivos.    
                             # los ficheros no se han eliminado (NO), Pero mi historias de commits si ha re-escrito (NO eliminado, pero si RE-escrito), se eliminaron tres, ubo un retroceso en el pasado de tres puntos de commits, se viajo el pasado eliminando tres cambios lineales en cadena del mas reciente hasta llegar al tercer commit en la secuencia.
                             # lo unico que ha hecho es meter el puntero del HEAD hacia tras tres posiciones de commits. 
                             # hemos vuelto hacia atras.
                             # hemos reseteado el HEAD, se ha ubicado en la cuarta picicion, las posiciones (5,6,7) ya no existen, esta historia ya no existe, hemos eliminado la historia de tres commits. 
                             # nosotros podemos ir hacia atras en el pasado o hacia adelante no futuro pero si que haya sido presente.
git status                             
                             # directorio de trabajo limpio es lo mejor que podemos tener en git (no hay nada que commitear "Nothing to commit Working tree clean")
                             # podemos modificar el historial(sin borrar nada), lo que hacemos no siempre tiene que desaparecer en el mundo.
                             # El --HARD "Hay que tener cuidado"
git log --oneline                             
git reset --hard HEAD~2      # retroceder dos posiciones hacia atras, aqui si que me han desaparecido los ficheros.
                             # me ha desaparecido todo lo que no conocia git en el commit 3 en el que se ha ubicado, inclusibe afecta lo que no habia afectado --soft, practicamente es como no importa si ubo un --soft.
git log --oneline | cat      # ejecute despues uel comando linuz cat, primero el git 
                             # hemo hido hacia tras dos posiciones.                             
                             # no solo se ha movido la historia hacia tras, tambien nos hemos cargado todo el sistema de ficheros. 
                             # el --soft, bueno no pasa nada estan ahi, no los toco, sinembargo el hard si elimina, al modificar la historia si elimina todo lo que no conoce en esa historia, en ese pasado.
                             # a nivel de historia es exactamente igual 
                             # otro uso del --hard, me pongo ha hacer cosas
touch add.cosa                              
vi fichero.c                 # adiciono texto desde el editor vi, cambiamos muchisimas cosas..
                             # y de repente digo, si es que lo que he hecho no vale para nada.
git add .                             
git diff                     # veo que no tengo nada raro el el servidor 
git status                   # me aparecen ficheros no trazados en la zona de preparacion git o staged
                             # En mi carpeta si me aparecen aunque no los tenga en mi repositorio local carpeta .git
git reset --hard             # resetea mi copia de trabajo, mi directorio, al ultimo escalon conocido en mi carpeta .git                            
                             # hace desaparecer las cosas que no han sido commiteadas, debes de actualizar la carpeta para que se reflejen los cambios de las eliminaciones. 
vi mifichero1.txt            # Introduzco datos: lhfdhhñklhñds  hjhdhñlkasñkhkñh   hhdasñlk pa pa pa...
git add .
git diff                     # me visualiza las diferencias entre el repositorio y mi carpeta contenedora del repositorio incluyendo el contenido de sus archivos.         
                             # me muestra los cambios que no he commiteado. 
git reset --hard             # HEAD is now at ID#COMMIT783AB94..                              
git diff                     # muestra en blanco no hay cambios hefectuados porque los ha eliminado
                             # para que se puedan eliminar debes de haber traquedo, adicionado con el add.
                             # --HARD, es un modo de descarte, puedes usarlo para realizar ensayos pruebas de librerias que vas ha improvisar con su uso pero no saber si te resulte o no.
                             # entonces programas el uso de --hard con esa prueba de descarte.
                             # de otra maneda tenes que ir haciendo git diff
git diff                              
git diff 4c5646574..6d36784 
vi mi fichero1.txt           # hlokhadjsjh 2lorem 
git diff                     # debes ir viendo que haz cambiado en cada fichero, y esto es incomable.
pwd                          # me muestra la ruta en la que estoy, comando linux
ls .git
git diff                     # Muestra las diferencias entre vuestra copia de trabajo, es decir mi carpeta, y vuestro repo local .git, es decir la subcarpeta .git 
git diff                     # cuando no sabes que han cambiado sabes que han estado trabajando en tonces haces un gti diff.
git reset --hard 
git diff                     # en blanco, he perdido los cambios o lo que halla creado.
                             # es un problemon. 
                             # Otro comandillo que esta muy chulo.
                             # que commit ha podido romper algo, para eso sirbe, podemos fallar los test de integracion, se rompio, las pruebas de integracion, y llega el momento en el que el temita senos fastidea.
git bisect                   # usage: git bisect [help|start|bad|good|new|old|terms|skip|next|reset|visualize|view|replay|log|run]           
vi fichero1.txt              # La primera linea
git commit -am "textos"
echo mas lineas >> fichero1.txt 
git commit -am "textos 2"
*                                        # Stop: time video 16.56 , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
                      # :18) 14/08/2023
git init  .
ls 
git status                               # Estamos en la rama master, recien creado el repositorio en X carpeta esta vacio,
                                         # Todavbia no tenemos ningun commit, Estamos en el HEAD master, principal que es implicito y es el inicio vacio.
touch fichero1.txt                       # creacion de fichero vacio .txt     # aun no esta añadido 
git add fichero1.txt                     # Asi lo añado a una parte del reposotorio que es llamada Staged       
git commit -am "Meto fichero1.txt"       # Lo comiteo aqui ya entro a git, a el historico de git.
echo datos > fichero1.txt                # comando linux para introducir informacion al archivo fichero1.txt
git commit -am "Cambio los datos"        # Este va a ser mi segundo commit el que esta mas actual el que esta mas reciente el que es la cabeza (HEAD) o encabeza todos los otros git.
                                         # cada commit es un escalon hacia la cima que representa lo que estoy levantando o construyendo.
                                         # Mi historial de transaccion se le añaden los commit van realcionados con la linea de tiempo.  
git log                                  # Me visualiza mi historial de transacciones de commits que he efectuado y en donde me encuentro.                                         
git log --oneline                        # De forma corta me visualiza mi historico de commits.
                                         # Respuesta:
                                         #   85804f7 (HEAD -> master, origin/master, origin/HEAD) Cambio usuario 1
                                         #   0f8dbcb hago varios cambios
                                         #   49898ad (tag: v1.0) primer codigo
                                         #   acaad34 mi primer commit, el import inicial
                                         # vamos a crear unos cuantos commits mas, inventados. 
echo mensaje > fichero2.txt              # crear nuevo fichero y adicionarle mensaje, comando linux
echo otromensaje > fichero3.txt          # crear nuevo fichero y adicionarle otromensaje, comando linux
git add fichero2.txt fichero3.txt        # añadir los dos ficheros
git commit -am "Meto mi fichero2.txt y mi fichero3.txt"    # los voy a comitear, con esto hemos puesto otro punto mas en que (HEAD)encabeza el estado actual de nuestro commits, es como una pila, los ultimo cambio el mas reciente, el commit mas reciente es el primero en la pila de commits o de confirmaciones de cambios. 
clear                                    # borrar pantalla
echo mastexto > mifichero4.txt           # vamos a meter otro cambion, otra confirmacion otro commit otro punto nuevo que encabezara nuestra pila del historico ca cambios o comfirmaciones o commits, graficamente es como un tronco que va creciendo en vertical hacia arriba y a un de el no salen ramas en x altura o tiempo de crecimiento, su naturaleza es el crecimiento atravez del tiempo.
git add mifichero4.txt                   # agrego area de preparacion de git staged
git commit -am "Meto mi fichero4.txt"    # hago el commit, nuevo punto de progreso, nuevo punto de crecimiento del historico de mi pila git, nueva version de encabezado de lo que hago o construyo.  
                                         # Mi ultima confirmacion siempre se llamara el HEAD (Cabeza de lo desarollado, Tope), la posicion de cabecera.
                                         # La posicion de CABECERA, so lo quieres ver como una lista horizontal que incia con puntos de izquierda a derecha, la ultima del extremo derecho siempre se llamara HEAD.
                                         # metamos otro commit para mover nuestra cabecera a nuestro commit mas reciente.
git log                                  #       
echo cambiotexto > mifichero4.txt        #
git commit -am "cambio de texto en fichero4.txt"    # lo que hago es insertar otro commit mas en mi historial de commits (o confirmaciones), y el HEAD se mueve automaticamente a la posicion del nuevo commit, a crecido su historico en el tiempo.
open .                                   # Comando linux para abrir carpeta actual mediante la interfaz grafica linux de la ubicacion de la carpeta que lo contiene.
fork .                                   # abrir carpeta contenedora con fork para visualizar el repositorio desde fork. 
                                         # fork, nos visualiza nuestra secuencia de commits con tendencia a crecimiento lineal, fork lo visualiza como si la estructura fuera una pila, crecimiento de abajo hacia arriva, el de arriba es la cabecera el comit mas reciente. 
                                         # yo podria viajar en el tiempo pasado, yo podri desacer los cambios que he hecho, si. 
clear
git log --oneline                        # estoy viendo mi historial de cambios.
                                         # por alguna razon tengo que volver hacia atras por cosas que me he equivocado. 
git reset                                # este comando me permite desaser cosas ya hechas posee dos formas de operar (dura y ligera)                                       
git reset --hard                         # forma dura
git reset --soft                         # forma ligera, apunta el HEAD a otro commit mueve el HEAD a otro commit del pasado. 
git log --oneline                        # como hago para saber a donde quiero volver, con git log historico de commit
git reset --soft HEAD~3                  # desde la punta actual HEAD, desde el actual HEAD quiero desacer tres cambios, retroceder en el tiempo. 
*                                        # Stop: time video 9.19 , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
                      # :18) 13/08/2023
git checkout v1.0     # Cambios de ramas cambio de tags, cambio de commits viajar al pasado y regresar al presente.       
git checkout v1.1     #
git checkout master   # 
git log               # listar log, historico de commits, estas en una especie de viaje al pasado, lo que haz creado en el presente no existe en el pasado(archivos, codigos etcc. ). 
                      # cuando hago un got chekout de una etiqueta, veo como estaba mi codigo en ese momento del pasado, es una foto, para eso sirben las etiquetas "tags".  
                      # viajar al pasado en git de otra forma
git log                      
                      # commit 585fb10c31ee279581c5d687d6ad7f6483ea25d4    # por regla general no cojemos todo el numero, solo los 4 primeros o los 6 primeros.
                      # commit 585fb1
git revert 585fb1     # para volver al pasado, para viajar a la epoca pasada   del commit id: 585fb1.               
                      # Te sale un aviso que esto revierte los cambios debes darle en guardar. 
git log               # para que veamos                       
                      # en Git esta muy mal visto que se toque el historico, que se manipule. 
                      # un revert añade una nueva confirmacion  "commit" informando que en esa confirmacion se habian eliminado cosas que habian ocurrido anteriormente. 
                      # pero no se elimina ningun commit del historioco, con el ojeto de poder arrepentirnos y hechar para tras ese revert. 
                      # hay ciertas sircunstancias en las que si se toca el historico. 
git push 
ls -altr                      
git rm demo.js       # eliminar fichero de git y acontinuacion un git commit
git rm cosa.c
ls
git pull              # revierte los cambios por que no se ha heco commit
                      # todo lo que este en mi indice que no hay enviado lo puedo revertir, siempre y cuando no haga un commit previamente. 
git reset --hard 
ls                    # vuelve aparecer el archivo cosa.c
git push              # me voy al fork IDE, refresco cambios a visuaizar recientes
                      # todo en git son confirmaciones, commits. 
                      # Historial de confirmaciones, historial de commits, por mucho rm que hagas y utilizas muchas cuentas de usuarios, seguiran presentes en el historial de confirmaciones. 
                      # con el historial de confirmaciones se puede recuperar cualquier fichero que halla sido eliminado.
git rm cosa.c
git commit cosa.c -a -m "cosa.c archivo eliminado"       
git push 
                      # voy a FORK a mirar
                      # ojo con los ficheros con usuarios y contraseñas, mucho cuidado con los ficheros que metemos al GIT, al repositorio, add, preferiblemente debe estar ignorados en el repositorio. 
                      # todo lo que este en el historial de comfirmaciones se puede recuperar. 
git log 
git revert  ID_COMMIT # Viajar al pasado en donde si existia el archivo que esta en el presente eliminado (head). 
                      # commit y mensaje del git revert mas guardar
ls                    # cosa.c          # y de nuevo el fichero cosa.c ha aparecido                      
                      # lo que pasa en el historial se queda en el historial
git rm                # no lo elimina de git simplemente le dice que no voy a seguir usando ese fichero.                       
                      # estamos en conceptos basicos 
                      # debes jugar con: 
git init .                      
cd ..
cd repositories
git init --bare mio2
cd 
git clone ruta-bare-repositorio-central-remoto
cd mio2
touch fichero                                   # Generacion de cambios
git add fichero 
git commit -am "mi primer commit fichero"       # jugueis con el historico
git log 
git rm fichero 
git push 
                      # :17) 12/08/2023
                      # con IntelliJ se puede hacer exatamente los mismo que visual code. y es muy usado en los cursos de JAVA.
                      # hay tambien clientes de escritorio, que no son entornos de desarrollos dedicados a GIT el mejor de todos es FORK pero es pago $50 US, es un cliente muy visual, se puede navegar en la aplicacion se ve como virfurcan las ramas.  
                      # con clic se puede hacer un reset maste    # nos dice que se va a resetear el repositorio.          
                      # se pueden apreciar de manera visual los estados de los dos repositorios el remoto y el local.
                      # cuando trabajas con muchas repoes es recomendable usar estar herramientas y si posees muchos cambios tambien. 
                      # Otras herrrmientas muy buenas, similares :  GitKraken, tortoisegit(añade opciones al boton derecho git en windows, no es ul cliente git comoo tal pero ayuda) 
                      # a las clientes de escritorio Git hay que derles refrescar para que los cambios sean reflejados visualmente. 
                      # refrescar en fork para ver la informacion 
git tag -a v1.1 -m "Version 1.1"         
git push origen v1.1  # enviar tag al git central romoto o bare.
git log               # me visualiza las etiquetas los tags existentes: v1.0   v1.1    etc...
clear 
ls 
git checkout v1.0     # checkout significa: Cambia a una rama o etiqueta(tag), Me informa que he cambiado a la rama v1.0 o al commit etiquetaco con la tag v1.0 "Note: switching to 'v1.0'  " 
                      # me informa que: HEAD is now at ID-commit-number "Mensaje de ese commit"
ls                    # al principio esta el fichero js, ahora no exite porque en este commit o etiqueta no se habia creado tal fichero, pero no se ha elimidado es como si hubieras viajado al pasado, Git te permite viajar al pasado y regresar al presente. pero el futuro no te lo permite, solo es con historiales de cambios de commits.                      
git branch -l         # para saber el nombre de mi rama principal o listarla (-l)   
git checkout master   # Como puedo volver a mi rama principal a mi al presente, actual de mi repositorio local.
                      # Mi rama principal se llama master como puedo volver. 
                      # "Switched to branch 'master'  "
                      # Stop: time video 53.53 Link: https://www.youtube.com/watch?v=y6n4u2Ncm1M&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=5
          # :16) 11/08/2023
          # Cosas maravillosas de Git:
          # No nos va a dejar hacer cambios, si tenemos cambios pendientes por ser obtenidos.
          # osea no nos permitira hacer push, si tenemos cambios pendientes por ser obtenidos, si estamos desactualizados de los cambios recientes en el servidor remoto. 
          # Aqui queria ir OJO:
          # Cuando dos personas cambian lo mismo en el repositorio, la primera que manda el cambio al repositorio gana. 
          # Y la segunda cuando haga un pull, se va a comer un mensajito de este estilo ("Conflicto") que ya veremos como resolverlo.
          # A esto se le denomina un:
          # "CONFLICTO"
          # Dos usuarios modificando un mismo archivo, entonces ha habido un pequeño problemon aqui.
          # por que dos personas distintas hemos intentado cambiar la misma parte del codigo. 
          # Hay momentos en donde estos problemas son tribiales de resolver hay otros que no, (Lo veremos en otra seccion (Seccion dedicada a MERGE)). 
          # Para que veas que GIT no es maravilloso de la muerte tampoco:
          # Osea funciona muy bien pero:
          # si dos personas trabajamos en la misma porcion del codigo, con un repositorio compartido (Con un remote)    
          # Podemos seguir teniendo estos problemas 
          # Tengo el conflicto, no lo voy a resolver, voy a hechar para tras lo que he modificado, de hecho voy a dejarlo tal cual estaba. 
          # y voy hacer el pull: 
git pull         
git commit
git rm casa.c 
clear 
          # ya esta. 
          # Mi solucion fue:  es el id del commit local mas actual, elimine esta confirmacion de modificaciones con:  
git reset 2164aaa272        
          # Despues hise un git pull para jalar confirmaciones del servidor remoto que no poseeo en mi repositorio local
          # para de esta manera poder proceder a realizar ccomfirmaciones de nuevos cambios o generacion de contenido de codigo por mi para poder posterior mente pushearla (enviarla al remoto, si es que Git me deja).
git status        
          # Changes not staged for commit:
          # (use "git add <file>..." to update what will be committed)
          # (use "git restore <file>..." to discard changes in working directory)
          #     modified:   LICENCIA
git restore LICENCIA              # "Aplique esta alternativa y funciono"
git rm LICENCIA                   # "Esta es otra alternativa que no aplique pero que deberia funcionar tambien" requiere l abandera force -f
git status 
          # On branch master
          # Your branch and 'origin/master' have diverged,
          # and have 2 and 1 different commits each, respectively.
          #  (use "git pull" to merge the remote branch into yours)
          # nothing to commit, working tree clean
          # "Esto parece que resuelve el problema ahora hare un git pull haber si me deja Git"
git pull          
          # Auto-merging LICENCIA
          # CONFLICT (content): Merge conflict in LICENCIA
          # Automatic merge failed; fix conflicts and then commit the result.
          # No me dejo, usare la opcion del git rm licencia.
git reset 2164aaa272                  
git rm LICENCIA 
          # Error: 
          # error: the following file has local modifications:
          # LICENCIA
          # (use --cached to keep the file, or -f to force removal)
git rm -f LICENCIA        
          # Ahora si lo borro.
git status
          # On branch master
          # Your branch and 'origin/master' have diverged,
          # and have 2 and 1 different commits each, respectively.
          # (use "git pull" to merge the remote branch into yours)
          # Changes to be committed:
          # (use "git restore --staged <file>..." to unstage)
          #    deleted:    LICENCIA
          # Me esta pidiendo hacer un commit de este cambion en mi repositorio local, lo deberia de hacer para que al intentar hacer un pull del remoto git se de cuenta que ya no hay conflicto.
          # y me permita hacer el pull.             
          # pero hare el pull primero haber si me permite, creo que no me lo permitira porque no he efectuado una confirmacion un commit de este cambio al eliminar el archivo el el reposotorio local que daba conflicto con el repositorio remoto.
          # pero miremos. 
git pull          
          # Error: 
          # error: Your local changes to the following files would be overwritten by merge:
          #  LICENCIA
          # Merge with strategy ort failed.
          # ahora si hare el commit y despues el pull y no debe de havber errores: 
git status      
          # On branch master
          # Your branch and 'origin/master' have diverged,
          # and have 2 and 1 different commits each, respectively.
          #  (use "git pull" to merge the remote branch into yours)
          # Changes to be committed:
          #  (use "git restore --staged <file>..." to unstage)
          #        deleted:    LICENCIA
git commit -am "Eliminacion del archivo licence"                  
          # [master 585fb10] Eliminacion del archivo licence
          # 1 file changed, 5 deletions(-)
          # delete mode 100644 LICENCIA
          #Commit exitoso, ahora procedere con el git pull y no debe de haver errores          
git status           
         #   On branch master
         #   Your branch and 'origin/master' have diverged,
         #   and have 3 and 1 different commits each, respectively.
         #     (use "git pull" to merge the remote branch into yours)
         # nothing to commit, working tree clean
git pull            
         # Error: 
         # CONFLICT (modify/delete): LICENCIA deleted in HEAD and modified in 85804f7866e3a2c16aa6632a0671fbebd0d7b814.  Version 85804f7866e3a2c16aa6632a0671fbebd0d7b814 of LICENCIA left in tree.
         # Automatic merge failed; fix conflicts and then commit the result.
         # Bueno me permitio extraer los comit del servidor remoto (repositorio remoto publico para dos programadores)
         # pero al mismo tiempo me informa que en mi repositorio local de mi carpeta del proyecto me ha llegado informacion que fue eliminada lo cual es verdad
         # antes no me funcionaba el git pull, no me llegaba los commits remotos.
         # ya me llegan pero me dice que no estan stageados (no estan en la zona de preparacion) hare git status:
git status        
         # On branch master
         # Your branch and 'origin/master' have diverged,
         # and have 3 and 1 different commits each, respectively.
         # (use "git pull" to merge the remote branch into yours)        
         # You have unmerged paths.
         # (fix conflicts and run "git commit")
         # (use "git merge --abort" to abort the merge)
         # Unmerged paths:
         # (use "git add/rm <file>..." as appropriate to mark resolution)
         #       deleted by us:   LICENCIA
         #
         # no changes added to commit (use "git add" and/or "git commit -a")
         #
         # hare un git add y otro y otro git commit, haber si ya se resuelve y se sincroniza 
git add -A        
         # On branch master
         # Your branch and 'origin/master' have diverged,
         # and have 3 and 1 different commits each, respectively.
         #   (use "git pull" to merge the remote branch into yours)
         #
         # All conflicts fixed but you are still merging.
         #  (use "git commit" to conclude merge)
         # Changes to be committed:
         #     new file:   LICENCIA
         #
         # OK ya esta estachado (Staged, En el area de prepara cion para confirmar)
         # ahora procedera hacer un git commit:
git commit -am "archivo licence del remoto ya esta de nuevo en el repositorio local"                  
      # OK reporte
      # [master 295b9de] archivo licence del remoto ya esta de nuevo en el repositorio local
      #
      # Ahora realizare un push y git no me debe mostrar errores (enviar mis cambios, confirmaciones mis commits al remoto)
git push      
      # Ok
      # Enumerating objects: 13, done.
      # Counting objects: 100% (13/13), done.
      # Delta compression using up to 4 threads
      # Compressing objects: 100% (9/9), done.
      # Writing objects: 100% (9/9), 1.03 KiB | 211.00 KiB/s, done.
      # Total 9 (delta 4), reused 0 (delta 0), pack-reused 0
      # To D:/acumulacion-ftp/practica-diaria/2-programacion/repositorios/aplication/
      # 85804f7..295b9de  master -> master
      #
      # Ahora hare un git pull
git pull     
      # Ok: sincronizado, nuevamente, "Se acaba la hora de git de hoy justamente al finalizar el conflicto y el trater de entenderlo" . 
      # Already up to date. 
      #
      # Conclusiones Cada repositorio maneja su propio estados son entidades diferentes y hay que rendir esplicaciones a cada una de ellas. 
      # Repositorio local1 programador1.
      # Repositorio Local2 Programador2.
      # Repositorio remoto o centrar.
      # Git es el intermediarion entre estos y si algo esta mal te lo hara saber para que lo corrijas.
      # el tema se da mas que todo cuando se toca un solo recurso que pretende ser personalizado por varios usuarios.
vi cosa.c       # Editor de text "vi" abriendo el archivo cosa.c
        # Error de conflito: 
        # No git no me permite hacer un PUSH, alimentar el servidor remoto, enviar mis commits mis cambios, mis conformaciones al servidor remoto, solo poseeo los cambios en el repositorio local. 
        # causas: pretendo modificar informacion que ya ha sido modificada por otro usuario, lo cual git lo rechaza debido a que el primero que hace el push es quien tiene mas derechos sobre el que intenta enviar un push en segundo turno.
        # El que primero envia o hace el push mas resiente a la fecha es quien lidera.
        # el usuario de segundo turno debe hacer un pull actualizarse con lo del usuario quien lidera y si el hace un push primero que el que lideraba ya sera el que lidera y el otro usuario pasa a segundo puesto.
        #
        # En resumen git no me permite dañar la informacion que otros usuarios han pushiado enviado al repositorio remoto,
        # El me dice haz un pull actualizate, jala la informacion del servidor remoto y suma pero sin alterar lo hecho por otro usuario.
        # 
        # ! [rejected]        master -> master (fetch first)
        # error: failed to push some refs to 'D:/acumulacion-ftp/practica-diaria/2-programacion/repositorios/aplication/'
        # hint: Updates were rejected because the remote contains work that you do
        # hint: not have locally. This is usually caused by another repository pushing
        # hint: to the same ref. You may want to first integrate the remote changes
        # hint: (e.g., 'git pull ...') before pushing again.
        # hint: See the 'Note about fast-forwards' in 'git push --help' for details.
        #
        # Traduccion:
        # ¡![rechazado] master -> master (buscar primero)!
        # Fallo al enviar algunas referencias a 'D:/acumulacion-ftp/practica-diaria/2-programacion/repositorios/aplicacion/'
        # pista: Las actualizaciones fueron rechazadas porque el repositorio remoto contiene trabajo que tú haces
        # pista: no tener de forma local. Esto suele ser causado por otro repositorio haciendo push(empujando).
        # pista: hacia la misma referencia. Es posible que desees integrar primero los cambios remotos.
        # pista: (por ejemplo, 'git pull ...') antes de hacer push nuevamente.
        # Pista: Consulta la sección 'Nota sobre avances rápidos' en 'git push --help' para más detalles.
            #
            # ! [rejected]        master -> master (non-fast-forward)
            # error: failed to push some refs to 'D:/acumulacion-ftp/practica-diaria/2-programacion/repositorios/aplication/'
            # hint: Updates were rejected because the tip of your current Branch is behind
            # hint: its remote counterpart. Integrate the remote changes (e.g.
            # hint: 'git pull ...') before pushing again.
            # hint: See the 'Note about fast-forwards' in 'git push --help' for details.
            #
            # ! [rechazado]        master -> master (no avance rápido)
            # error: no se pudieron subir algunas referencias a 'D:/acumulacion-ftp/practica-diaria/2-programacion/repositorios/aplicacion/'
            # pista: Las actualizaciones fueron rechazadas porque la punta de tu rama actual está atrasada
            # pista: su contraparte remota. Integrar los cambios remotos (por ejemplo,
            # pista: 'git pull ...') antes de hacer push nuevamente.
            # Pista: Consulta la 'Nota sobre avances rápidos' en 'git push --help' para obtener más detalles.
git pull        # Auto-merging LICENCIA
                # CONFLICT (content): Merge conflict in LICENCIA
                # Automatic merge failed; fix conflicts and then commit the result.
                # Fusión automática de LICENCIA.
                # CONFLICTO (contenido): Conflicto de fusión en LICENCIA
                # La fusión automática falló; soluciona los conflictos y luego realiza el commit del resultado.
git fetch                 # Es la otra forma del git pull, si no hay nuevos cambios en el servidor remoto obviamente no los vamos a ver, no va a pasar nada.
git pull                  # jalar los cambios del remoto al mi repositorio local "carpeta del proyecto que contiene .git" :15 :  09/08/2023 )
git tag -a v1.0  [numero de confirmacion o numero de commit ]       # Esta estiqueta va unida a una corfirmacion especifica "etiquetas  gordas o completas mas metadatos que describen", Autor, el email, fecha de creacion, para uso publico externo.  
git tag -a v1.0                       # esta estiqueta va unida al mi version actual a la del HEAD, cuando no se le hace referencia a un ID commit puntual . "etiquetas  gordas o completas mas metadatos que describen", Autor, el email, fecha de creacion, para uso publico externo.  
git tag "etiquetas ligeras sin -a"    # continen menos informacion que las gordas, solo para uso interno.  
git tag -a v1.0  49898adf87fad5560865e902dec988ac1c13c661
                                      # Escribir mensaje "Esta es la version 1.0" guardar y cerrar archivo
git log 
git commit -am "Vesion 1.0"
git push origin v1.0      # "para enviar la nueva etiqueta al servidor remoto", sino quiero enviarlo a mi repositorio remoto no hacemos el push y ya 
                          # Acordaros estamos utilizando dos repositorios 
                          # el de mi carpeta o la carpeta del proyecto 
                          # y el remoto (nube o carpeta local remota en mi equipo   (repositorio bare copia de seguridad))
              # Ingresa a herramienta visual Fork 
              # Git en visualstudio code
              # Cambios staged     :    YA se han adicionadanos al area de preparacion para poder ser luego commiteados
git pull      # lo que haces es obtener los cambios del repositorio remoto 
              # session dedicada a merge: 
              # resolucion de conflictos para poder unir codigo de varios programadores   :14)
              # Cuando no empiezo el repositorio de cero, giteo en una carpeta que ya tenga existentes. 
              # problema me cargo la carpeta miapp, no hay mas no hay solucion, esta es 
              # la opcion A.   
git init . 
git add . 
git commit -am "Version actual de mi proyecto"
             # La opcion B: 
git init --bare aplication 
             # Creo un repositorio bare "un servicio de git completo en una crpeta diferente del proyecto", estos repositorios no estan hechos para trabajar sobre ellos directamente se debe clonar el repositorio a una carpeta donde yo si voy a trabajar con ellos y no olvidar el push para proteger mi repositorio 
             # los commits se almacenan en la carpeta pero como yo tengo un servidor central de git no se me debe olvidar hacer el push de los commit para que queden registrados en el remoto los commits efectuados o los cambios confirmados que he realizado (git push)
             # los commits solo sequedan en la carpeta del proyecto la local y punto, si se borra esa carpeta se pierde todo, debes hacer el git push para enviarlo al repositorio centrar remoto ubicado en otra carpeta. 
             # por defecto se envia al por defecto: [remote "origin"] url : "a esta ruta puede ser github gitlab carpeta local(bare) " 
             # git commit lo confirmo localmente en mi carpeta claro. 
             # git push, confirmo a nivel de servidor, a nivel remoto, envio los commit a servicor de git remoto(local o internet)    :13 -08/082023)
git clone  D:/acumulacion-ftp/practica-diaria/2-programacion/repositorios/aplication/ .          # "Clonar un repositorio del remoto"
                                      # Error:  fatal: destination path '.' already exists and is not an empty directory. Carpeta ya existe y no esta vacia, yo tengo que clonar el repositorio que acabo de crear en una carpeta vacia, como convierto miapp a un repositorio nuevo   
                                      # Solucion o truco:, renombra la carpeta original: 
miapp> cd ..                          # salir de una carpeta
miapp> mv miapp miapp.original        # mover toda la informacion de una carpeta a otra comando linux
                                      # ruta> -->    D:\acumulacion-ftp\practica-diaria\2-programacion\angular\exp-proyectos\workspace-exp>
ruta> git clone  D:/acumulacion-ftp/practica-diaria/2-programacion/repositorios/aplication/ miapp       
cd miapp                              # entrar a la carpeta miapp
miapp> ls D:/acumulacion-ftp/practica-diaria/2-programacion/repositorios/aplication/       # listar contenido, ruta del repositorio centrar remoto en mi equipo de local 
miapp> ls -al                         # comando de listar linux mas sus flags "banderas"
                                      # .git                # lo listado, "ha creado un repositorio remoto apartir de uno en una carpeta remota pero en el mismo pc(local) "
cat .git/config                       # ver contenido del archivo config que esta dentro de la carpeta oculta .git
                                      # [remote "origin"]                        # "Ha creado un remote"
                                      # url = D:/acumulacion-ftp/practica-diaria/2-programacion/repositorios/aplication/
                                      # Como gitealizo la carpeta de antes, como la hemos copiado a mi app.original, copiamos a git todo su contenido  
miapp> cp -prf ../miapp.original/*    # "Es igual a copiar todo el contenido de miapp.original a miapp desde windows"
miapp>ls                              # "visualiza los archivos y carpetas"
miapp>git status
                                      # miapp/
..\miapp> git add .
rutaX/> git commit -a -m "mi primer commit el import inicial"     # menos de 80 caracteres el mensaje -m
rutaX/> git log
                                  # commit acaad348124a28990393d0175787fb0e3390bd05 (HEAD -> master)
                                  # Author: Miguel Gutierrez <miguelepst@hotmail.com>
                                  # Date:   Mon Aug 7 22:39:15 2023 -0500
                                  # mi primer commit, el import inicial
                                  # +OK
rutaX/> git push                  # "Coje mis cambios locales y me los envia a mi remote (Para este caso la carpeta remota en el mismo pc)"
                                  # Enumerating objects: 90, done.
                                  # Counting objects: 100% (90/90), done.
                                  # Delta compression using up to 4 threads
                                  # Compressing objects: 100% (81/81), done.
                                  # Writing objects: 100% (90/90), 297.58 KiB | 541.00 KiB/s, done.
                                  # Total 90 (delta 29), reused 0 (delta 0), pack-reused 0
                                  # To D:/acumulacion-ftp/practica-diaria/2-programacion/repositorios/aplication/
                                  #   * [new branch]      master -> master
                                  # +OK "Funciaona a la primera"
                                  # Bueno entonces yo de repente tengo un mal dia y digo a la mierda todo esto que no va aninguna parte, fuera!.
                                  # y borro la carpeta miapp
rutaX/> cd ..
rutaX/> clear                     # "Limpir pantalla"
rutaX/> rm -rf miapp
                                  # Y me lo he cargado, No, Pues no te lo has cargado, porque tu puedes hacer un git clone ya que lo posees en un repositorio remoto.
rutaX/> git clone  D:/acumulacion-ftp/practica-diaria/2-programacion/repositorios/aplication/ miapp    
                                  # programacion/repositorios/aplication/ miapp
                                  # Cloning into 'miapp'...
                                  # done.
                                  # Aqui vuelvo a tener las cosas necesarias, maravilloso, pero si te cargas el repositorio "ahi si no olvidatede las cosas necesarias que de verdad ya no existen te toca empezar de cero otra vez"
git init .                        # repositorio normal lo que hace es convertir mi carpeta en un repositorio git, pero solo mi carpeta no podria compartirla facilmente.  
                                  # Repositorio bare contiene el historico de conformaciones pero no voy a poder trabajar con el solo, debo clonarlo para poder trabajar con el. 
git commit -a -m "Mensaje"        #   
rm -rf .git                       # "borrar toda la informacion de git ya no esta metido en git asi de sencillo ya no hay repositorio"
git init --bare aplication        # "Es como inicializar un repositorio remoto pero en local en otra carpeta defirente a la del projecto en tu mismo pc"  Initialized empty Git repository in D:/acumulacion-ftp/practica-diaria/2-programacion/repositorios/aplication/ 
                                  # la carpeta es como un colector de informacion, Contiene informacion git pero no es la carpeta sobre la que trabajaremos. es similar a un remote la diferencia es que no esta en internet esta en una carpeta diferente al proyecto 
                                  # Initialized empty Git repository in 
                                  # D:/acumulacion-ftp/practica-diaria/2-programacion/repositorios/aplication/
git commit -m “Initial Commit”    #
git commit -a                     # "la bandera(or flag) -a Significa todo"  :12)
git reset simple.py               # Eliminando archivos del área de preparación especifico solo uno el: simple.py
git reset                         # Eliminando archivos del área de preparación todos (staged)
git add -A                        # "adiciona todo tambien"
git add .                         # "adiciona todo es como un all carpetas archivos al staged o zona de preparacion lista para cimmitear "
git add .gitignore                # "asignacion de un archivo especifico .gitignore al area de preparacion del repositorio " :11)
git status                        # "comando visualiza el estado del repositorio" :10)
touch .gitignore                  # "Crear archivo que contiene lo que va a ser ignorado o no incluido en el repositorio"
                                  # .project  *.java   /carpeta  "/carpeta Ignora carpeta y su contenido total"  ".project ignora archivo .project"  "*.java -  ignora todos los nombres de archivos con extencion .java no los incluye en el repositorio" :9.1)
git init                          #  
git init .                        # : Crear primer repositorio    :9)
git config --help                 # :8)   ayuda de git online te lleva al sitio web     :7)
git config --global user.email “miguelepst@hotmail.com”    # :6) : asignacion del email de usuario
git config --global user.name “Miguel Gutierrez”           #    : asignacion de numbre de usuario
cat $home/.gitconfig              # Variable de entorno $home sistema operativo global, versu contenido
cat .git/config                   # "Comando linux para ver contenido del archivo config"
git config --list --local         # tercer grado de permisos, varias veces por que en siertos repositorios vas a usar vuestro email del trabajo y en otras tu email personal, o proyectitos vuestros por ahi.
git config --list --global        # segundo grado de permisos es sobre escrita por system pero esta se sobre escribe a local, lo vas a usar una vez configuracion inicial, nombre de usuario e email de usuario.
git config --list --system        # system es la zona que quiero mostrar, esta opcion raremente se modifica. nunca lo vas a utilizar
git config                        # Sirbe para cambiar la configuracion de git  "tres configuraciones: --system --global --local "
                                  # :5)     
git -v                            # :4) version de git instalada
git --version                     # :4) version de git instalada
mkdir nombreCarpeta               # :3) crear carpeta 
cd d:                             # :2) Cambiar de unidad de disco 
rm -r nombreCarpeta               # :1) borrar carpetas y su contenido",
  },

}

START


```



```json DICCIONARIO DE EXPERIENCIAS practicas    "conceptos"

El Manual Esencial de Git
https://www.freecodecamp.org/espanol/news/el-manual-esencial-de-git/

Estados: 
Informacion sin seguimiento (Carpetas archivos).
Area de preparacion (Lo que sea a añade al repositorio creado) Agregando archivos al área de preparación (staging area)


´´´


``` TS EXP 31, Video 11: Angular Avanzado sesión 10 - Parte 1, keyword: A2v11 
 // PWA : app sirve para navegador y para aplicaciones de dispositivos no realmente nativa del SO del dispositivo x(celular, pc de escritorio, laptop, etc..)  es una App web solucion alternativa multiplataforma

 {Herramientas:" " ,}


```






```json EXP 30, Video 10: Angular Avanzado sesión 9, keyword: A2v9  "proyecto: AngularAvanzadoSesion9"
 // Libreria RXJS     //PIPES 
 {Herramientas:" https://rxviz.com/ " ,}


```

```json DICCIONARIO DE EXPERIENCIAS practicas
{
  {"comandos FIFO": "
   :16)
   :15)
   :14)
   :13)
   :12)
   :11)
   :10)
    :9)
    :8)
    :7)
    :6)
    :5)
ng g c components/A2v9/ShoppingListA2v9 --project AngularAvanzadoSesion9    :4) 
ng g s services/A2v9/shopping/shoppingA2v9 --project AngularAvanzadoSesion9     :3) 
ng g c pages/HomePage --project AngularAvanzadoSesion9    :2) 
ng g application AngularAvanzadoSesion9 --routing --style scss    :1) ",
  },

}

```



```HTML EXP 29, Video 9: Angular Avanzado sesión 8, keyword: A2v9
<!-- A2v9 -->
<!-- Angular Avanzado sesión 8 --> <!-- keyword: A2v9, Video 9, EXP 29 -->
<!-- ANGULARWORKSPACE, con varios proyectos, un proyecto que cargue otros proyectos(A,B,C...)  -->
<!-- HUB de proyectos, para los ADMIN y los accesos a los proyectos -->
<!-- Tener un proyecto de proyectos -->
<!-- Crear un WorkSpace sin proyectos para iniciar -->
<!-- Toca empezar un nuevo proyecto y separarnos de este peara este ejemplo -->

```

```json DICCIONARIO DE EXPERIENCIAS practicas
{
  "comandos FIFO": "
  npm run start:app3 ,
  ng --version : para saber la version de Angular CLI Global :16)
  npx ng --version : para saber la version de Angular CLI local :15)
  npx  serve  :para comprovar si esta el serve instalado de manera local :14)
  npm install --save-dev serve  :servidor para desplegar build port:3000   :13)
  ng g c pages/SettingsPage --project app2  :12)
  ng g c pages/HomePage --project app2    :11)
  ng g c components/nav --project app2    :10)
  ng g c components/nav --project app1      :9)
  ng g c pages/SettingsPage --project app1     :8)
  ng g c pages/HomePage --project app1     :7)
  npm run start:app0  :6)
  ng add @angular/material --project app0   :5)
  ng g application app2 --routing --style scss   :4) 
  ng g application app1 --routing --style scss  :3) 
  ng g application app0 --routing :2) 
  ng new 0workspace --create-application false :1) ",
}

```

```json
"defaultProject": "app0", // No se permite la propiedad defaultProject  Angular 14 la descontinuo 
```

