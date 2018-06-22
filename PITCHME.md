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
