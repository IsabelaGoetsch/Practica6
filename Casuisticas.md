# Casuísticas a probar en el testing

### DNI
Para el test de el DNI se probarán dos DNIs correctos, para comprobar si verdaderamente se ha programado bien la
clase, así como varios DNIs incorrectos. Entre estos, se han probado los tres que se definen como inválidos en 
el objeto Java y otros que no pueden ser correctos, uno con menos dígitos de los exigidos, otro con más letras 
de las posibles y, por último, un DNI configurado como sólo números, lo que haría imposible que fuese correcto.

### Teléfono
En el caso de teléfono es más fácil. Únicamente es necesario comprobar la longitud del teléfono y si son todo números. Para ello, y al igual que con DNI, se han probado dos correctos y alguno incorrecto. Entre los incorrectos están uno de menor longitud, uno de mayor longitud y uno que contiene letras.


### Process Controller
Por último, se ha hecho el testing de ProcessController, que tiene dos opciones posibles. Cada una de estas opciones la he dividido en dos, para probar las veces que ha sido correcto el E2E y para las veces que ha sido incorrecta.
Para el caso de /api/v1/process-step1 se ha necesitado comprobar simplemente si al introducir unos datos correctos se obtenía "OK" y para unos datos incorrectos se obtenía "KO"
Por último, para el caso de /api/v1/process-step1-legacy ha sido más difícil comprobar, ya que, al contrario que el anterior, no sabemos el mensaje exactamente, únicamente tenemos su código (message1, message2). Pero, al igual que con el anterior, es necesario comprobar la respuesta recibida al introducir unos datos correctos y unos incorrectos.