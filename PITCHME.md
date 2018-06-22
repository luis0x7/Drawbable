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
#### Shape
```     
        android:shape= “oval”
        android:shape= “line”
        android:shape= “rectangle”
        android:shape= “ring”
```
#### Corner
```
        android:radius=”20dp”
        android:bottomLeftRadius=”10dp”
    
```
#### Gradient or solid color

#### Stroke 
```
        android:width=”1dp”
        android:color=@color/your_color  
    
```
#### 
<br>
<span class="aside"></span>

---

### 

![Logo](https://cdn-images-1.medium.com/max/800/1*m34HiIdSPlDPYXnq4cYJsg.png)
<br>

<span class="aside"></span>
---
#### Animation-list 
```
    <animation-list android:id="@+id/selected" android:oneshot="false">
    <item android:drawable="@drawable/wheel0" android:duration="50" />
    <item android:drawable="@drawable/wheel1" android:duration="50" />
  />
 </animation-list> 
```

#### Layer-list

#### State Drawable
```
  <item android:drawable="@drawable/button_checked"
        android:state_checked="true" />
        
```

<span class="aside"></span>
---

#### <span class="gold">Vector Drawable</span>

### pathdata 
##### M o m (X,Y)+ :Mueve el cursor a la pocicion.
##### Z o z:Dibuja la line desde el cursor hasta el punto de inicio.
##### L o l (X,Y)+ :dibuga una line desde el punto especificado en (X,Y)
##### H o h (X)+ :dibuja un linea linea desde el cursor hasta el punto especificado (X)
##### V o v (Y)+ :dibuja un linea linea desde el cursor hasta el punto especificado (Y)

```
 android:pathData="M100,100 L300,100 L200,300 z"
```

<span class="aside"></span>
---

#### <span class="gold">Pathdata ejemplo  </span>

### pathdata 
```
 android:pathData="M100,100 L300,100 L200,300 z"
```

![Logo](https://cdn-images-1.medium.com/max/800/1*VqVwZg20dWFj1Ix2vapUAA.png)
<br>

<span class="aside"></span>

Note:https://materialdesignicons.com/ POOP 💩
---

#### <span class="gold">Animaciones con vectores  </span>

#### Rotation animation 

#### Trimming stroked

#### Morphing paths




<span class="aside"></span>
---
