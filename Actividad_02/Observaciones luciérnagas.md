Observaciones luciérnagas.

En el modelo de sincronización de luciérnagas, la entropía de Shannon nos sirve para medir qué tan desordenado está el sistema. Cuando las luciérnagas están prendiendo y apagando sin coordinación, hay más incertidumbre sobre el estado de cada una, y por lo tanto la entropía es alta. En cambio, cuando todas se sincronizan y están casi todas prendidas o casi todas apagadas al mismo tiempo, la entropía baja mucho y puede acercarse a cero. Esto tiene sentido porque ya no hay “sorpresa”: el comportamiento es casi el mismo para todas.

Algo que noté es que, sin importar la cantidad de luciérnagas, cuando los parámetros están en valores mínimos es muy difícil que la entropía llegue a cero. Las luciérnagas no logran sincronizarse bien y el sistema se mantiene con bastante desorden. Es decir, no basta con tener muchas luciérnagas; si no interactúan lo suficiente, no aparece la sincronización.

También observé que cuando el umbral es más alto, la entropía parece volverse más estable, en el sentido de que no sube y baja tanto, sino que se mantiene más constante. Esto puede deberse a que las luciérnagas tardan más en llegar al punto donde se prenden, lo que hace que los cambios sean menos bruscos.

El parámetro min_luces_reset tiene un efecto claro: cuando lo aumentamos, la entropía baja. Esto pasa porque se necesita que más luciérnagas estén prendidas para que las demás reinicien su reloj, lo que ayuda a que se sincronicen mejor. Algo parecido ocurre con el radio_vision: cuando es mayor, las luciérnagas “ven” a más vecinas y eso facilita que se coordinen. Por eso, al aumentar el radio de visión, la entropía tiende a disminuir.

Desde mi punto de vista, el parámetro ventana introduce un poco de inestabilidad. Cuando es grande, la entropía puede subir a un pico y luego bajar otra vez. Parece que este parámetro retrasa el efecto de sincronización y hace que el sistema tarde más en estabilizarse. En cambio, cuando la ventana es cero, la entropía llega más rápido a cero porque la sincronización ocurre antes.

Finalmente, cuando todos los parámetros están en valores altos, la entropía generalmente tiende a cero, aunque esto depende bastante del valor de la ventana. En general, el modelo muestra que mientras más interacción haya entre las luciérnagas, más fácil es que se sincronicen y que el sistema pase de un estado desordenado (alta entropía) a uno ordenado (baja entropía).



