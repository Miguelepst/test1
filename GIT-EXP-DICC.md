Lo mas reciente arriba "HEAD"
Lo mas antiguo en lo profundo del fondo.

# :28) 24/08/2023 ,  # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp

```json DICCIONARIO DE EXPERIENCIAS practicas    "ENTENDIENDO GIT"
{
  {"comandos FIFO": 04/08/2023"   *--------# Start (HEAD):   



# :28) 24/08/2023 , # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
                    #----------------------------------------------------
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
git branch -M main          # Cambio el nombre del <oldbranch> to <newbranch> con force, master to main.
git push -u origin main     # crea una rama de seguimiento en remoto de la rama local main y envia los commits.
                            # otra opcion es importar un repositorio de otro repositorio online.
                            # …or import code from another repository
                            # You can initialize this repository with code from a Subversion, Mercurial, or TFS project.
                            #Git Bash Here   Consola de Git ubicada en la carpeta local
                            #----------------------------------------------------

                            
git config --global -l      # git config --global --list    
                            # cuando es un comando reducido se pone un igual ejemplo: 
                            # --list seria igual a: -l
ls -all                     # ver todos los archivos inclusive los ocultos 
pwd                        # ubicacion de mi repositorio      
                           # local se utiliza para un proyecto git ya iniciado
                           # y queremos mostrar que lo que hallamos aportado fuimos nosotros
git config --global user.email none                             
                           #satge area
                           # todo en git se basa en confirmaciones commits
                           # Retomar clase :https://www.youtube.com/watch?v=y6n4u2Ncm1M&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=3
                           # time video: 5:42 / 1:03:31
                           # pequeña configuracion en git
                           # por norma general las confirmaciones en git 
                           # van asociadas a un nombre y a un correo electronico
                           # como le digo a GIT que utilice mi nombre y mi direccion de correo electronico 
                           # para asociarlas a los commit que yo realice.
git config                 # esta en tres partes: la podemos cambiar en tres partes
                           # la primera utilizada a nivel de sistema operativo : system
                              # SYSTEM      # raramente utilizada.                        
                           # la siguiente es la opcion global se aplica a todos los repositorios de mi usuario: global     
                              # GLOBAL  
                              # es decir todos los repositorios que esten dentro de la carpeta de mi usuario
                              # es decir los repositorios que esten dentro de mi carpeta de usuario 
                           # por ultimo la zona de configuracion LOCAL 
                              # LOCAL
                              # los cambion de mi configuracion local 
                              # se aplica a la configuracion de mi repositorio actual 
                           # como puedo modificar unas u otras    
git config  --zonaAModificar 
git config --system 
git config --global       # modificaria mi fichero de usuario
git config --local        # modifica la configuracion de mi repositorio actual
                          # si yo tengo un unico repositorio 
                          # mis cambios de configuracion serian para ese unico repositorio
git config --global       # y como usuario tengo multiples repositorios 
                          # todos mis repositorios van a tener la misma configuracion
                          # no tengo que ir uno por uno                          
                          # cual es la que manda, cuanto mas cerca de repositorio mas mandamos.
                          # emprimer lugar estaria SYSTEM 
                          # las opciones de SYSTEM serian sobre escritas con las opciones GLOBAL.
                          # y las opciones GLOBAL serian sobre escritas con las opciones LOCAL.
                          # LOCAL es lo mas cerca al repositorio.
git config --list --system    # para ver mi configuracion actual (system).
                              # parametrizar git a nivel de sistema es raro.
git config --list --global 
git config --list --local     # A nivel local dentro de la carpeta .git hay un fichero que se llama config 
                              # y de ahi es donde sale esta informacion
                              # cuando modificamos local, 
                              # lo que estamos modificando es ese fichero: .git/config
cat .git/config               # esta es la configuracion local 
cat $HOME/.gitconfig          # esta es la global, 
                              # que es cuando usamos un: git config global
                              # estamos modificando el fichero gitconfig
                              # dentro de nuestro directorio de usuario
                              # en windows sera: c:/user/nombreDeUsuario     
                              # "C:\\Users\\Equipo\\AppData\\Local\\Programs\\Microsoft VS Code\\bin\\code\"                          
                              # y cuando estamos modificando el --system 
cat /etc/gitconfig            # cuando estamos modificando --system
                              # que directamente no esta definido no esta, no lo tengo.                     
                              # system : lo vas autilizar cero veces.
                              # global : lo vas a utilizar una vez, configura opciones por defecto del usuaro del sistema operativo para sus todos sus repositorios
                              # local : lo vas a utilizar mas veces porque: 
                                # en ciertos repositorios tenes que usar vuestro email del trabajo, si son cosas de trabajo 
                                # y en otras tener que usar/mostrar vuestro email real 
                                # si son cosas  de bueno pues proyectos open source que pueden ser vuestros 
                                # o proyectillos que tenes por ahi.
                              # como cambio yo una opcion  
git config --list --global                               
git config --global user.name "Jose test"     # nombre de la opcion seguido del valor de la opcion 
git config --global user.name                 # visualiza opcion nombre
git config --global user.name " "             # user espacio en blanco " "
git config --global user.name none            # usar none
cat $HOME/.gitconfig 
git config --list --global  
                                              # que quiero cambiar las opciones 
                                              # referentes a un repositorio especifico, a uno particular 
                                              # quiero que se salga de la configuracion general:
git config --local user.email "vroman@noreply.users.github.com"
cat .git/config                                # "vroman@noreply.users.github.com"
git config --list --local                      # "vroman@noreply.users.github.com"
                                              #  cuando se va a utilizar este email 
                                              # cuando yo haga un commit o una corfirmacion 
                                              # dentro de este repositorio particular
                                              # Cuando se va a utilizar el otro email el global 
                                              # cuando haga una confirmacion 
                                              # fuara de este repositorio (que posee email en su configuracion local)
                                              # en cualquier otro repositorio relacionado a la cuenta usuario y su contenido
git config --global user.name                                            
git config --global --remove-section user.name ='off'         # NO funciono, eliminar al usuario
git config --global --remove-section user.name                # no funciono.  
git config --global --unset-all user.name                     # este si funciono
git config --global --replace-all user.name "New User Name"   # otros comandos
git config --global -e                        # Este comando abrirá el editor GNU nano con lo que está esperando.
git config --global --remove-section user     # si ok
git config --local --remove-section user      # ok
git config --global --unset-all user.name     
git config --global --add user.name <whatever>
git version                                   # git version 2.38.1.windows.1
                                              # The latest version is 2.42.0.
                    ### Haz tus mensajes de GIT Commit PROFESIONALES con CONVENTIONAL COMMITS
                      # https://www.youtube.com/watch?v=SigVVJmUGv8 
                      # cuando no sabes que mensajes ponerles a tus commits 
                      # https://www.conventionalcommits.org/en/v1.0.0/
                      # El mensaje de confirmación debe estructurarse de la siguiente manera:
                      # <type>[optional scope]: <description>
                      # [optional body]
                      # [optional footer(s)]
                      # Los tipos:
                      # fix 
                      # feat: nueva funcionalidad que se esta añadiendo al proyecto 
                      # BREAKING CHANGE: 
                      # types other than fix : recommends build:, chore:, ci:, docs:, style:, refactor:, perf:, test:, and others.
                      # footers other than BREAKING CHANGE
                      # Ej:
                      # feat: allow provided config object to extend other configs
                      # BREAKING CHANGE: `extends` key in config file is now used for extending other config files
                       # Error 
git remote add origin https://github.com/Miguelepst/test1.git  # Error: ya existe
git branch -M main
git push -u origin main                      
                        ### Solucion:
git remote set-url origin https://github.com/Miguelepst/test1.git        # repositorio GitHub Internet
git config user.password ghp_mgv007r0v3Q1DrGiVQlVPSDWUWURafcJrZPs1fNbcU  # token de acceso x 7 dias caducidad.
git remote -v   # verificar las direcciones remotas
git config --local --remove-section user
git config --local user.name "Miguel Cartagena"
git config --local user.email miguel@noreply.com
cat .git/config
git config --global --list
git add .
git commit -am "doc: "
git push
                                            # consulta: git version 1.7.9.5
# :27) 23/08/2023 ,  # time video, Start: 1:50:56 , Stop: --:--:-- , Link: https://www.youtube.com/watch?v=PBk7OjXcQ2E&list=PLkVpKYNT_U9fFT8xjHVevZI8tWWnnIN0d&index=4 , Title: Curso Git - Sesión 4 - OpenBootcamp
            # Fork :
            # Es copiar y pegar, Duplicar un proyecto.
            # yo me quiero hacer una copia de un proyecto de otra persona para poder trabajar en el.
            # porque quiero contribuir a ese proyecto.
            # pero quiero hcer cambios sin afectar a ese proyecto todavia, es un duplicar.
            # la ventaja de fork:
            # cualquier cambio que realices sobre el proyecto ya no va afectar al otro proyecto,
            # tu te haz hecho tu copia, tienes tu copia y puedes generar alteraciones generar cambios, 
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
            # en el repositorio central principal desde don de lo bifurcaste
            # y esto se los podria yo enviar a mis compañeros de trabajo y decirles 
            # oye estoy haciendo estos cambios que te parecen, y me podrian dar citas, sugerencias.
            # y coloborar entorno a ella
            # es muy sencillo El FORK, hacer un duplicado una copia de un repositorio externo el tu yo
            # y una vez haz hecho el fork, 
            # se comporta como un repositorio como otro cualquiera que tubieras en tu cuenta de gitHut
          ### Access token: para conectar nuestros repositorios locales con nuestros repositorios remotos 
            # debemos generas un ACCESS TOKEN politica got 2021
            # para poder acceder alos repositorios remotos.
            # nueva politica de seguridad conocida como access token
git init    # inicializar el repositorio 
            # lo siguiente configuraciones de identidad 
git config user.name Miguelepst                          # coloco el usuario que tengo asociado en GitHut             
git config user.email  miguelepst@hotmail.com            # aqui debe ir el email que tengamos asociado a nuestra cuente de GitHub
git config user.password ghp_mgv007r0v3Q1DrGiVQlVPSDWUWURafcJrZPs1fNbcU  token 
git remote add origin https://github.com/Miguelepst/git-exp-dicc.git             # url del repositorio 
           # ya esta todo configurado, provemos hacer un git add y un git push
git add .  # para agregar todo 
git commit -am probandoPat           
git push -u origin master 
            git push https://token: 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  
git config --local user.name "okmiguel@noreply.user-github.com"





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

