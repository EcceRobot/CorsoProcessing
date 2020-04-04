### Esempio_1.00
Applicazione senza codice
```cpp

```
### Esempio_1.01
Dimensioni della schermata
```cpp
size(800,600);
```

### Esempio_1.02
Commentare il codice
```cpp   
//size(800,600);
```
### Esempio_1.03
Schermo intero   
```cpp
fullScreen();
```
### Esempio_1.04 
Sfondo
```cpp
size(500,500);
//background(#RGB);
//background(grey);
//background(R,G,B);
background(200,0,0);
```
### Esempio_1.05 
Ordine di esecuzione 
```cpp
background(200,0,0);
background(0,200,0);
```
### Esempio_1.06 
Il punto
```cpp
size(500,500);
background(0,200,0);
point(50,50);
```
### Esempio_1.07 
Dimensione del tratto
```cpp
size(500,500);
background(0,200,0);
point(50,50);
strokeWeight(5);
```
### Esempio_1.08 
Colore del tratto 
```cpp
size(500,500);
background(200,0,0);
strokeWeight(5);
stroke(200);
point(x,y);
```
### Esempio_1.09 
Disegnare più punti 
```cpp
size(500,500);
background(200,0,0);
strokeWeight(5);
stroke(200);
point(100,100);
point(200,100);
```
### Esempio_1.10 
Disegnare più punti, di colori diversi
```cpp
size(500,500);
background(200,0,0);
strokeWeight(5);
stroke(0,200,0);
point(100,100);
stroke(0,0,200);
point(200,100);
```
### Esempio_1.11
Disegnare più punti equidistanti 
```cpp
size(500,500);
background(200,0,0);
strokeWeight(5);

point(100,100);
point(100*2,100);
point(100*3,100);
```
### Esempio_1.12 
Linee
```cpp
size(500,500);
background(200,0,0);
line(100,200,400,400);
```
### Esempio_1.13 
Rettangoli
```cpp
size(500,500);
background(200,0,0);
rect(100,100,300,200);
```
### Esempio_1.14 
Quadrato
```cpp
size(500,500);
background(200,0,0);
rect(100,100,300,300);
```
### Esempio_1.15 
Ellissi
```cpp
size(500,500);
background(100);
ellipse(100,100,100,50);
```
### Esempio_1.16 
Circonferenza
```cpp
size(500,500);
background(200);
ellipse(100,100,100,100);
```
### Esempio_1.17 
Riempimento delle figure chiuse
```cpp
size(500,500);
background(100);
fill(200,0,0);
ellipse(100,100,100,50);
```
### Esempio_1.18 
Nessun riempimento delle figure chiuse
```cpp
size(500,500);
background(100);
noFill();
ellipse(100,100,100,50);
```
### Esempio_1.19 
Nessun tratto delle figure chiuse
```cpp
size(500,500);
background(100);
noStroke();
fill(200,0,0);
ellipse(100,100,100,50);
```
### Esempio_1.20 
Spessore del tratto delle figure chiuse
```cpp
size(500,500);
background(100);
strokeWeight(3);
ellipse(100,100,100,50);
```
### Esempio_1.21 
Colore del tratto delle figure chiuse
```cpp
size(500,500);
background(100);
stroke(200,0,0);
ellipse(100,100,100,50);
```
### Esempio_1.22
Testo
```cpp
size(500,500);
background(100);
text(123456, 100, 200);
```
### Esempio_1.23 
Dimesioni del testo
```cpp
size(500,500);
background(100);
textSize(30);
text(123456, 100, 200);
```


### Esempio_1.24 
Colore del testo
```cpp
size(500,500);
background(100);
textSize(30);
fill(200,200,0);
text(123456, 100, 200);
```

### Esempio_1.25 
Gradazione di colore
```cpp
size(500,500);
background(100);
textSize(30);

fill(50,0,0);
text(111, 200, 50);

fill(100,0,0);
text(222, 200, 100);

fill(150,0,0);
text(333, 200, 150);

fill(200,0,0);
text(444, 200, 200);

fill(250,0,0);
text(555, 200, 250);
```

### Esempio_2.01 
Sorgente di dati casuali
```cpp
size(500,500);
background(100);
textSize(30);
text(random(300) , 100, 200);
```

### Esempio_2.02
Posizionare grafiche in posizioni casuali
```cpp
size(500,500);
background(0,200,0);
strokeWeight(10);
point(random(500),50);
```

### Esempio_2.03
Muovere grafiche in funzione del tempo
```cpp
size(500,500);
background(0,200,0);
strokeWeight(10);
point( second() , 500/2 );
```

### Esempio_2.04 
L'orologio "rotto"
```cpp
size(500,500);
background(100);
textSize(30);
text(hour() , 100, 200);
text(minute() , 150, 200);
text(second() , 200, 200);
```


### Esempio_2.05
Il primo programma ciclico, ma "difettoso"
```cpp
void setup(){
  size(500,500);
  background(100);
}

void draw(){
  textSize(30);
  text(hour() , 100, 200);
  text(minute() , 150, 200);
  text(second() , 200, 200);
}
```


### Esempio_2.06
Il secondo programma ciclico, ma ancora "difettoso"
```cpp
void setup(){
  size(500,500);
  background(200,0,0);
}

void draw(){
  strokeWeight(10);
  point( second() , 500/2 );
}
```

### Esempio_2.07
Il primo programma ciclico corretto
```cpp
void setup(){
  size(500,500);
}

void draw(){
  background(100);
  textSize(30);
  text(hour() , 100, 200);
  text(minute() , 150, 200);
  text(second() , 200, 200);
}
```


### Esempio_2.08
Il secondo programma ciclico corretto
```cpp
void setup(){
  size(500,500);
}

void draw(){
  background(200,0,0);
  strokeWeight(10);
  point( second() , 500/2 );
}
```


### Esempio_2.09
Contare il tempo dall'avvio del programma
```cpp
void setup(){
  size(500,500);
}

void draw(){
  background(200,0,0);
  textSize(30);
  text(millis() , 100, 200);
  strokeWeight(10);
  point( millis(), 500/2 );
}
```


### Esempio_2.10
Medesimo parametro su più elementi
```cpp
void setup(){
  size(500,500);
}

void draw(){
  background(200,0,0);
  textSize(30);
  text(millis()/10 , millis()/10, 200);
  strokeWeight(10);
  point( millis()/10, 500/2 );
}
```


### Esempio_2.11
Circonferenza parametrica

```cpp
void setup(){
  size(500,500);
}

void draw(){
  background(200,0,0);
  textSize(30);
  text(millis()/10 , 100, 200);
  strokeWeight(10);
  ellipse( millis()/10, 500/2, millis()/100, millis()/100 );
}
```



### Esempio_2.12
Misuratore di livello

```cpp

void setup(){
  size(500,500);
  textSize(30);
}

void draw(){
  
  background(200,0,0);
  strokeWeight(1);
  line(95, 100, 95,  400);
  
  text(0 , 50, 400);
  text(15 , 50, 325);
  text(30 , 50, 250);
  text(45 , 50, 175);
  text(60 , 50, 100);
  
  strokeWeight(5);
  line(100, 400-second()*300/60, 100, 400); 
  text(second() , 100, 400-second()*300/60);
  
}
```


### Esempio_2.13
Grafiche NON parametriche: diagonali e centro dello schermo
```cpp
void setup(){
  size(500,500);
}

void draw(){
  
  background(200,0,0);
  strokeWeight(1);
  line(0, 0, 500, 500);
  line(0, 500, 500, 0); 
  ellipse(500/2,500/2,50,50);

}
```


### Esempio_2.14
Grafiche parametriche: diagonali e centro dello schermo

```cpp
void setup(){
  size(700,500);
}

void draw(){
  
  background(200,0,0);
  strokeWeight(1);
  line(0, 0, width, height);
  line(0, height, width, 0); 
  ellipse(width/2,height/2,50,50);

}
```


### Esempio_2.15
mouseX e mouseY

```cpp
void setup(){
  size(700,500);
}

void draw(){
  
  background(200,0,0);
  
  ellipse(mouseX, mouseY, 50, 50);

}
```


### Esempio_2.16
Una sorta di Paint

```cpp
void setup(){
  size(700,500);
}

void draw(){
  
  //background(200,0,0);
  
  ellipse(mouseX, mouseY, 50, 50);

}
```



### Esempio_2.17
Una sorta di Paint, con variazioni

```cpp
void setup(){
  size(700,500);
}

void draw(){
  
  //background(200,0,0);
  fill(millis()/100);
  ellipse(mouseX, mouseY, 50, 50);

}
```
