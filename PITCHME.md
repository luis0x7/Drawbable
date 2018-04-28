@title[Introduction]

## Presentacion  <span class="gold"></span>


<br>
<br>


---

@title[PITCHME.md]

#### Patrón RxMVP  <span class="gold"></span>
#### Patrón DI
#### y Patrón Observador
<br>
<span class="aside"></span>

---

#### Librerias Utilazadas<span class="gray"></span>.
#### AWS(Amazon web service) <span class="gray"></span>.
#### butherknife  <span class="gold"></span>.
#### Dagger2  <span class="gold"></span>.
#### Rxjava2  <span class="gold"></span>.
#### Rx Android  <span class="gold"></span>.
#### librerias de utilidad  <span class="gold"></span>.

<br>


---

@title[Step 2. Git-Commit]

#### RxJava 

<span class="aside"> Programación reactiva</span>
<br>




---


@title[Step 2. Git-Commit]

#### Programacion orientada a objetos

![Logo](https://image.slidesharecdn.com/presentacinpoo-120823191110-phpapp01/95/poo-programacin-orientada-a-objetos-14-728.jpg?cb=1345751433)
<br>




---

@title[Step 3. Done!]

### Observable  <span class="gold"></span>
<span class="gray">Definicion</span>
<br>
<span class="gray">Unsubcribe</span>

<br>
<br>
<br>


---

@title[Step 3. Done!]

### operadores para crear Observable  <span class="gold"></span>
#### Create
#### Defer 
#### Empty/Never/Throw 
#### Interval 
#### Just
#### Range
#### Repeat
#### Start 
#### Timer 
<br>
<br>
<br>



---

@title[Feature Rich]

### Tipos de Obserbables

#### 1.-Observable
#### 2.-Flowable
#### 3.-Single
#### 4.-Maybe
#### 5-Completable
#### 6-Subject

---
@title[Step 3. Done!]

### Backpressure  <span class="gold"></span>
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
@[3](llamamos el evento custom click del drawer para obtener los datos   )
@[4](obtiene el valor que el observable emite)
@[5]()

---

