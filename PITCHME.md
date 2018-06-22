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
@title[PITCHME.md]

#### Shape Drawable <span class="gold"></span>
#### shape
```     
        android:shape= “oval”
        android:shape= “line”
        android:shape= “rectangle”
        android:shape= “ring”
```
#### corner
```
        android:radius=”20dp”
        android:bottomLeftRadius=”10dp”
    
```
#### corner
```
    
```
#### corner
#### corner
<br>
<span class="aside"></span>

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

