Mostrar la configuracion guardada:
    
    show running-config  

CCopiar una configuración al archivo de inicio:
    
    copy running-config startup-config

Para no tener que ir hasta el R#:

    R1(config-if)#do show ip interface brief  ó #do sh ip int br

Borra ip de una interfaz:

    int f0/0
    no ip add


-----------------------------

RIP:

    R1(config)#router rip

Las redes que conozco o de las interfaces:

    R1(config-router)#network 172.30.1.1
    R1(config-router)#network 172.30.1.2
Tambien se podria darle de frente las redes como 172.30.1.0

Atajo para el show running:

    R#sh run | begin router
    R#sh run | section rip ó R#sh run | se rip

Borrar configuracion rip:

    no router rip

Tabla de enrutamiento:

    show ip route
