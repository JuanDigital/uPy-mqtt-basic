# uPy-mqtt-basic

Iot 
esp32 enviar y recibir datos por mqtt con micro python y mosquitto

editar broker mosquitto en windows 10

Abrir como administrador -> cd c:\program files\mosquittomosquitto.conf
editar
# =================================================================
# Listeners
# =================================================================
listener 1883 0.0.0.0
allow_anonymous true

iniciar broker

cd c:\program files\mosquitto

mosquitto -c mosquitto.conf

escuchar esp32

mosquitto_sub -h 192.168.43.113 -t pl1\Zoe

escribir en esp32

mosquitto_sub -h 192.168.43.113 -t Server -m 1

en en su caso 

mosquitto_sub -h 192.168.43.113 -t Server -m 0
