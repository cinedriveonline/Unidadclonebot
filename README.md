<h1 align="center">⚛️ Unidadclonebot - Heroku version ⚡<br></h1> 

<br />

<p align="center">Telegramclonebot Te permmite copiar carpetas y archivos individuales a carpetas especificas en tu Team Drive, superando el limite de transferencia con cuentas de servicio<p/>

<!-- > ## A simple bot to copy and duplicate team drives -->
<p align="center">
  <img src="https://i.imgur.com/QkxmCOp.png" />
</p>

<br />

#### ✅ Ventajas de este bot
- La copia se realiza en cuestion de segundos o minutos para ser Terabytes
- Su velocidad es Sorprendente
- No hay limite de Transferencia si agregas mas cuentas de servicio
- Puedes agregar varios destinos en los Team Drive


#### ❌ Desventajas y limitaciones del bot
- Solo funciona con Team Drives
- Para un solo usuario ya que si agregas mas, usuarios ellos tienen que realizar las configuraciones posteriores que son : Agregar cuentas de servicio y configurar sus Directorios, y asi cada quien tener acceso al bot, con sus propias configuraciones, sin necesidad de tener las mismas cuentas de servicio, y seleccionando sus propios Team Drives, el problema y limitacion es que esta configuracion se hace una sola vez, si aumentas usuarios desde heroku, se resetea la configuracion de todos y se necesitara que vuelvan a iniciarla (agregar cuentas de servicio y los directorios o carpetas destino cada uno de los usuarios).
- Al parecer los accesos directos en un directorio a copiar pueden causar problemas, por lo tanto no es recomendado para grupos telegram a menos que hagas agreges a todos los usuarios (ids) y ya no volver a tocar nada en heroku.

⚫ Aqui el tutorial completo [Unidadclonebot Telegram bot para clonar directorios o Team drives completos Gdrive](https://uniq.edu.mx/unidadclonebot-telegram-bot-para-clonar-directorios-o-team-drives-completos-gdrive) - [Aqui el video](https://www.youtube.com/c/UNIQedumx)
- [x] Crear bot en telegram y obtener "telegram_token"
- [x] Obtener "user_ids" , nuestro ID telegram.
- [x] Crear Grupo en telegram y Obtener "group_ids" 
- [x] Deploy a Heroku,Configurar las variables  y Activar Free dynos
- [x] Crear cuentas de servicio en google console
- [x] Enviar las cuentas de servicio al bot y configurar Team Drive destino o directorio.
- [x] Clonar carpetas o Team Drive completo

## Crear bot en telegram y obtener "telegram_token"
- Busca @BotFather en telegram e inicialo con `/start` 
- Create un nuevo bot con `/newbot` 
- Copia el HTTP API  que sera tu  "telegram_token"

## Obtener "user_ids" , nuestro ID telegram.
- Busca @userinfobot e inicialo con `/start` te arrojara un ID , ese es "user_ids"

## Crear Grupo en telegram y Obtener "group_ids" 
_El grupo telegram puedes omitirlo si no vas a usar grupo telegram_
- Create un nuevo grupo en telegram 
- Agrega el bot @MissRose_bot a tu grupo y dale `/id`
- Agrega tu bot al grupo tambien y promuevelo como administrador

## Deploy a Heroku,Configurar las variables  y Activar Free dynos
- Dale click ene este boton 

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/cinedriveonline/Unidadclonebot)


- Ponle un nombre y Configura las variables con los datos anteriores
- Cuando termine el proceso ve a la pestaña `resources` y activa Dynoss

## Crear cuentas de servicio Google console
- Ve a [Crear cuentas de servicio y grupo google](https://github.com/abdiasriver/CuentasGooglegroups) proceso para crear cuentas de servicio y grupo google
- Quita el script `rename.py` de la carpeta accounts y comprimela en zip
- Ve a tu bot en telegram, inicialo y dale `/help` 
- Enviale el `accounts.zip` como documento y en `caption` coloca `/sa`  o bien envia `/sa` y despues el `accounts.zip`
- Se subiran las cuentas de servicio
- Despues dale `/folders` y Agrega un folder favorito a donde llegaran los archivos, puedes agregar hasta 10

## Clonar carpetas o Team Drive completo

- Copia la url o link de la carpeta a clonar o copiar
- envialo como mensaje normal solo pegandolo y dandole enter
- Te preguntara a que carpeta o unidad quieres enviarlo de tus "folders favoritos"
- El proceso empezara y terminara pronto.

[Fork de Msgsuite](https://github.com/MsGsuite/CloneBot_Heroku)
