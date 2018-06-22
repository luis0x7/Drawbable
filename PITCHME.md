@title[Introduction]

##  <span class="gold">Presentación Drawbables </span>

<br>
<br>


---

@title[PITCHME.md]

#### Patrón RxMVP  <span class="gold"></span>
#### Patrón DI
#### y Patrón Observador
<br>
<span class="aside"></span>
Note: patron diseño solucion de problemas,patron arquitectura Mvp patron diseño singleton :exsistencia unica ejemplo multiples conexciones, Mvp modelo define datos mostrar ,presentador logica ,vista interface grafica. Rx (Reactive extention),dependencia , P ovservador uno a muchos avisa  V≤-P->M
---

#### <span class="gold">Librerias Utilazadas</span>
#### AWS(Amazon web service) <span class="gray"></span>
#### Butherknife  <span class="gold"></span>
#### Dagger2  <span class="gold"></span>
#### Rxjava2  <span class="gold"></span>
#### Rx Android  <span class="gold"></span>
#### Librerias de utilidad  <span class="gold"></span>



<br>

Note:dagger:modelo Rxjava presentador butterkinfe view
---

@title[Step 2. Git-Commit]

####   <span class="gold">RxJava</span>

<span class="aside"> Programación reactiva</span>
<br>


![Logo](http://reactivex.io/assets/operators/legend.png)

Note:es programacion con flujo de datos asincronos. stream secuensia de elementos. asincrono eventos independientes. reaction.............http://www.philosophicalhacker.com/wp-content/uploads/2015/06/rxjava_prezi_define_observer_subscriber-1024x791.jpg
---


@title[Step 2. Git-Commit]

#### <span class="gold"> Programacion orientada a objetos </span>

![Logo](http://2.bp.blogspot.com/-0_vBJM9OxiM/VYLBqC8TQ0I/AAAAAAAAAFQ/NqKqRCHAgGE/s640/POO.png)
<br>

Note:La encapsulación  organizar datos y métodos de una estructura, conciliando el modo en que el objeto se implementa,evitando el acceso a datos por cualquier otro medio distinto a los especificados.polimorfismo a la capacidad que tienen los objetos de una clase de responder al mismo mensaje o evento en función de los parámetros utilizados durante su invocación. Un objeto polimórfico es una entidad que puede contener valores de diferentes tipos durante la ejecución del programa.Diferencias simula objetos del mundo real y reactiva reaciona la los sucesos errores y fallos 
---

@title[Step 3. Done!]

###   <span class="gold">Observable</span>
<span class="gray">Definicion</span>
<br>
<br>
<br>
<span class="gray">Unsubcribe</span>

Note:observable se subscrive a observador y reaciona a lo que el obsevable emite. .subcripcio(myOnnext).unsubripcion le dice a los observables que no esta interesado lo que pude crear cascada de problemas  
---

@title[Step 3. Done!]

####    <span class="gold">Operadores para crear Observable</span>

##### Create
##### Defer 
##### Empty/Never/Throw 
##### Interval 
##### Just
##### Range
##### Repeat
##### Start 
##### Timer 

<br>
<br>



---

@title[Feature Rich]

###  <span class="gold">Tipos de Obserbables</span>
<br>
#### Observable
#### Flowable
#### Single
#### Maybe
#### Completable
#### Subject
Note: subjet ejemplo convertir obserbable externo de cold a hot   observable cold espera y hot no 
---
@title[Step 3. Done!]

###   <span class="gold">Backpressure</span>
<br>
#### BackpressureMode.NONE
#### BackpressureMode.ERROR
#### BackpressureMode.BUFFER
#### BackpressureMode.DROP
#### BackpressureMode.LASTES
<br>
<br>
<br>



---
### <span class="gold">Análisis en Android Studio</span>

<br>

```
Observable<IDrawerItem> observarDrawer(){
        return Observable.create(consumer ->
                d.withOnDrawerItemClickListener((view, position, drawerItem) -> {
                    consumer.onNext(drawerItem);
                    return false;
                })
        );
    }
    
```
@[1](Se le asigna el tipo IDrawerIteam al observable  )
@[2](Se crea el observable con el subcriptor )
@[3](Llamamos el evento custom click del drawer para obtener los datos    )
@[4](Obtiene el valor que el observable emite)

note: Flowvable o obsevable , rxjava1 y rxjava2
---

