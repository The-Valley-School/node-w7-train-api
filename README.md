# WORKSHOP 7 - API de Trenes

Para este Workshop el enunciado no va a ser tan guiado como en otras ocasiones, pero no te preocupes, ¡aquí estamos para ayudarte! En el mundo profesional, cuando debes desarrollar una API, nadie te va a decir todo lo que debes hacer, pero no te preocupes, ¡aquí te lo indicamos!

Para empezar, debes hacer un API para una aplicación de venta de productos de segunda mano que tenga las siguientes funcionalidades:

**REGISTRO**

¡Para empezar a comprar, hay que registrarse! Un usuario debe poder registrarse indicando:

- Nombre
- Apellidos
- Email
- Contraseña
- DNI
- Nacionalidad
- Fecha de Nacimiento
- Tratamiento (SR. / SRA.)

![/assets/3_-_REGISTRO.png](/assets/3_-_REGISTRO.png)

**LOGIN**

Por supuesto, si hay un registro habrá un login. Un usuario podrá hacer login con su usuario y contraseña.

![/assets/Untitled.png](/assets/Untitled.png)

**BÚSQUEDA DE TRENES**

Independientemente de si el usuario está logado o no, podrá buscar viajes. Para buscar viajes debería indicar una ciudad de origen, una ciudad de destino y una fecha. Esto le devolverá los trenes que hacen ese recorrido en ese día:

![/assets/Untitled%201.png](/assets/Untitled%201.png)

Para simplificar podemos pensar que los billetes se reservan siempre de uno en uno.

**DETALLES**

Un viaje en sí tendrá los siguientes datos:

- Hora de salida
- Hora de llegada
- Ciudad origen
- Ciudad destino
- Precio
- Tren

**RESERVAR UN BILLETE**

Si el usuario está interesado podrá reservar un billete. Para reservarlo no será necesario pagar, ya que esto se hará en persona. Debes tener en cuenta que solo podrá reservar si quedan plazas suficientes en ese viaje.

![/assets/Untitled%202.png](/assets/Untitled%202.png)

Al reservar el billete al usuario se le mostrará un mensaje con un localizador, que debe ser un número aleatorio.

**MARCAR BILLETE COMO PAGADO**

Al entrar en el tren el revisor pedirá el localizador, con esto podrá buscar el billete asociado a ese localizador. Si lo encuentra le cobrará al usuario en persona el precio a pagar y podrá marcar como que ese billete está pagado.

**OTRAS CUESTIONES**

Ahora que ya sabes la operativa de nuestra aplicación, debes ocuparte de hacer el API lo mejor posible, ten en cuenta que debes controlar todas las situaciones posibles.

**EXTRAS**

- Crea un seed para rellenar ciudades, trenes y viajes.
- Añade en los trenes distintas secciones y precios: VIP, normal, business…
- Añade la posibilidad de dar de alta códigos promocionales, de manera que al asociarlos en la reserva se haga un descuento.