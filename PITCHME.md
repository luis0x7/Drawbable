@title[Introduction]

##  <span class="gold">Presentación Rxjava2 Observables </span>

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
Note:
<br>


---

@title[Step 2. Git-Commit]

####   <span class="gold">RxJava</span>

<span class="aside"> Programación reactiva</span>
<br>


![Logo](https://cdn-images-1.medium.com/max/800/1*26WzvNZ6aQJFSG5A0MoTnA.png)


---


@title[Step 2. Git-Commit]

#### <span class="gold"> Programacion orientada a objetos </span>

![Logo](https://image.slidesharecdn.com/presentacinpoo-120823191110-phpapp01/95/poo-programacin-orientada-a-objetos-14-728.jpg?cb=1345751433)
<br>




---

@title[Step 3. Done!]

###   <span class="gold">Observable</span>
<span class="gray">Definicion</span>
<br>
<br>
<br>
<span class="gray">Unsubcribe</span>


<br>


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


---

