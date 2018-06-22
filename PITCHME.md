@title[Introduction]

##  <span class="gold">Presentación Drawables </span>

<br>
<br>


---

@title[PITCHME.md]

####   <span class="gold"></span>
#### Shape Drawable
#### Vector Drawable
<br>
<span class="aside"></span>

---

#### <span class="gold">Librerias Utilazadas</span>
#### AWS(Amazon web service) <span class="gray"></span>




<br>

Note:dagger:modelo Rxjava presentador butterkinfe view
---

@title[Step 2. Git-Commit]

####   <span class="gold">RxJava</span>

<span class="aside"> Programación reactiva</span>
<br>


![Logo](http://reactivex.io/assets/operators/legend.png)

---


@title[Step 2. Git-Commit]

#### <span class="gold"> Programacion orientada a objetos </span>

![Logo](https://github.com/alexjlockwood/ShapeShifter/raw/master/art/playpausestop.gif)
<br>

---

@title[Step 3. Done!]

###   <span class="gold">Observable</span>
<span class="gray">Definicion</span>
<br>
<br>
<br>
<span class="gray">Unsubcribe</span>

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

