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























### Esempio_3.01
Strutture condizionali IF con tempo (second())

```cpp
void setup(){
 size(600,600);
 textSize(30);
 }
 
 void draw(){
 
 background(0);
 
 text(millis(),50,100);
 
 if( second() == 30 ){
 fill(255,0,0);
 ellipse(300,300,100,100);
 }
 
 }
 ```



### Esempio_3.02
Strutture condizionali IF con tempo (millis)

```cpp
void setup(){
 size(600,600);
 textSize(30);
 }
 
 void draw(){
 
 background(0);
 
 text(millis(),50,100);
 
 if( millis() > 5000 ){
 rect(100,100,100,100);
 }
 
 }
 ```


### Esempio_3.03
Strutture condizionali IF con mouse

```cpp
void setup(){
 size(600,600);
 textSize(30);
 }
 
 void draw(){
 
 background(0);
 
 text(mouseX,100,50);
 
 if(mouseX > 300){
 rect(100,100,100,100);
 }
 
 }
 ```






### Esempio_3.04
Strutture condizionali IF con mouse e linea

```cpp
void setup(){
 size(600,600);
 textSize(30);
 }
 
 void draw(){
 
   background(0);

   text(mouseX,100,50);

   stroke(255,0,0);
   line(width/2,0, width/2, height);

   if(mouseX > width/2){
      rect(100,100,100,100);
   }
 
 }
```

### Esempio_3.05
Test: scrivere con il testo dove si trova il mouse
```cpp
void setup(){
 size(600,600);
 textSize(30);
 }
 
 void draw(){
 
 background(0);
 
 stroke(255,0,0);
 line(width/2,0, width/2, height);
 
 if(mouseX > width/2){
 text("DESTRA",400,50);
 } 
 
 if(mouseX > width/2){
 text("SINISTRA",100,50);
 }
 
 }
```



### Esempio_3.06
Operatori logici. AND 
```cpp
 void setup(){
 size(600,600);
 textSize(30);
 }
 
 void draw(){
 
 background(0);
 
 stroke(255,0,0);
 
 line(width/2,0, width/2, height);
 line(0, height/2, width, height/2);
 
 if(mouseX > width/2 && mouseY<height/2){
 text("ALTO DESTRA",350,50);
 }
 
 }
 
```



### Esempio_3.07
Operatori logici. OR 
```cpp
void setup(){
 size(600,600);
 textSize(30);
 }
 
 void draw(){
 
 background(0);
 
 text(millis(),100,100);
 
 if(millis() < 5000 || millis() > 10000){
 ellipse(300,300,100,100);
 }
 
 }
```



### Esempio_3.08
Operatori logici. NOT 
```cpp
void setup(){
 size(600,600);
 textSize(30);
 }
 
 void draw(){
 
 background(0);
 
 text(millis(),100,100);
 
 if( !(millis() < 5000 || millis() > 10000) ){
 ellipse(300,300,100,100);
 }
 
 }
 ```

### Esempio_3.09
mousePressed 

```cpp
void setup(){
 size(600,600);
 }
 
 void draw(){
 
 background(0);
 
 if( mousePressed == true ){
 ellipse(300,300,100,100);
 }
 
 }
 ```


### Esempio_3.10
mousePressed, esercizio di lasciare un ellipse solo quando clicco 

```cpp
void setup(){
 size(600,600);
 background(0);
 }
 
 void draw(){
 
 
 if( mousePressed == true ){
  ellipse(mouseX,mouseY,100,100);
 }
 
 }
 ```


### Esempio_3.11
mouseButton, LEFT

```cppvvvvvvvvv
void setup(){
 size(600,600);
 background(0);
 }
 
 void draw(){
 
 
 
 if( mousePressed == true && mouseButton == LEFT ){
 ellipse(mouseX,mouseY,100,100);
 }
 
 }
 ```


### Esempio_3.12
mouseButton, RIGHT

```cpp
void setup(){
 size(600,600);
 background(0);
 }
 
 void draw(){
 
 if( mousePressed == true && mouseButton == LEFT ){
 ellipse(mouseX,mouseY,100,100);
 }
 
 if( mousePressed == true && mouseButton == RIGHT ){
 background(0);
 }
 
 }
 
 ```

### Esempio_3.13
mouseButton, CENTER

```cpp
void setup(){
 size(600,600);
 background(0);
 }
 
 void draw(){
 
 if( mousePressed == true && mouseButton == LEFT ){
 ellipse(mouseX,mouseY,100,100);
 }
 
 if( mousePressed == true && mouseButton == RIGHT ){
 background(0);
 }
 
 if( mousePressed == true && mouseButton == CENTER ){
 fill(  random(255)  );
 }
 
 }
 
```



### Esempio_3.14
keyPressed


```cpp
void setup() {
 size(600, 600);
 background(0);
 }
 
 void draw() {
 
 if ( mousePressed == true && mouseButton == LEFT ) {
 ellipse(mouseX, mouseY, 100, 100);
 }
 
 if ( keyPressed == true ) {
 background(0);
 }
 
 if ( mousePressed == true && mouseButton == CENTER ) {
 fill(  random(255)  );
 }
 }
```




### Esempio_3.15
key

```cpp
void setup() {
 size(600, 600);
 background(0);
 }
 
 void draw() {
 
 if ( mousePressed == true && mouseButton == LEFT ) {
 ellipse(mouseX, mouseY, 100, 100);
 }
 
 if ( keyPressed == true && key == 'c') {
 background(0);
 }
 
 if ( mousePressed == true && mouseButton == CENTER ) {
 fill(  random(255)  );
 }
 }
```



### Esempio_3.16
key
```cpp
void setup() {
 size(600, 600);
 background(0);
 }
 
 void draw() {
 
 if ( mousePressed == true && mouseButton == LEFT ) {
 ellipse(mouseX, mouseY, 100, 100);
 }
 
 if ( keyPressed == true && key == 'c') {
 background(0);
 }
 
 if ( keyPressed == true && key == 'r' ) {
 fill(  255, 0, 0  );
 }
 
 if ( keyPressed == true && key == 'g' ) {
 fill(  0, 255, 0  );
 }
 
 if ( keyPressed == true && key == 'b' ) {
 fill(  0, 0, 255  );
 }
 }
 
```



### Esempio_3.17
// keyCode
```cpp
void setup() {
 size(600, 600);
 strokeWeight(5);
 }
 
 
 void draw() {
 background(200);
 
 
 if ( keyPressed == true && keyCode == UP ) {
 line(width/2, height/2, width/2, 0);
 }
 
 if ( keyPressed == true && keyCode == DOWN ) {
 line(width/2, height/2, width/2, height);
 }
 
 if ( keyPressed == true && keyCode == LEFT ) {
 line(width/2, height/2, 0, height/2);
 }
 
 if ( keyPressed == true && keyCode == RIGHT ) {
 line(width/2, height/2, width, height/2);
 }
 
 }
 
```




### Esempio_4.01
// Due circonferenze concentriche ed una linea che passa per il centro. Senza variabile utente.

```cpp
void setup() {
 size(600, 600);
 }
 
 void draw(){
 background(150);
 
 ellipse(200,200,100,100);
 
 ellipse(200,200,50,50);
 
 line(200,0, 200,height);
 
 }
```



### Esempio_4.02
// Due circonferenze concentriche ed una linea che passa per il centro. Con variabile utente.

```cpp
int posizione_x;
 
 void setup() {
 size(600, 600);
 }
 
 void draw(){
 background(150);
 
 ellipse(posizione_x,200,100,100);
 
 ellipse(posizione_x,200,50,50);
 
 line(posizione_x,0, posizione_x,height);
 
 }
```



### Esempio_4.03
// Due circonferenze concentriche ed una linea che passa per il centro. Con variabile utente. Assegnazione statica.

```cpp
int posizione_x;
 
 void setup() {
 size(600, 600);
 posizione_x = 500;
 }
 
 void draw(){
 background(150);
 
 ellipse(posizione_x,200,100,100);
 
 ellipse(posizione_x,200,50,50);
 
 line(posizione_x,0, posizione_x,height);
 
 }
 
```





### Esempio_4.04
// Due circonferenze concentriche ed una linea che passa per il centro. Con variabile utente. Assegnazione dinamica.

```cpp
int posizione_x;
 
 void setup() {
 size(600, 600);
 posizione_x = 300;
 textSize(30);
 }
 
 void draw(){
 background(150);
 
 ellipse(posizione_x,200,100,100);
 
 ellipse(posizione_x,200,50,50);
 
 line(posizione_x,0, posizione_x,height);
 
 posizione_x = posizione_x + 1;
 
 text(posizione_x, 50,50);
 
 }
```




### Esempio_4.05
// Variazione del colore, con reset della variabile

```cpp
int colore;
 
 void setup() {
 size(600, 600);
 colore = 0;
 textSize(30);
 }
 
 void draw(){
 
 background(255,0,0);
 
 colore = colore + 1;
 
 if (colore == 255){
 colore = 0;
 }
 
 fill(colore);
 
 ellipse(300,300,400,400);
 
 text(colore, 50,50);
 
 }
 
```




### Esempio_4.06
// Variazione della posizione, con reset della variabile

```cpp
int posizione_x;
 
 void setup() {
 size(600, 600);
 posizione_x = 0;
 textSize(30);
 strokeWeight(10);
 }
 
 void draw(){
 
 background(255,0,0);
 
 posizione_x = posizione_x + 1;
 
 if (posizione_x > width){
 posizione_x = 0;
 }
 
 point(posizione_x,300);
 
 text(posizione_x, 50,50);
 
 }
```


### Esempio_4.07
// Variazione della posizione_x, con inversione della direzione
```cpp

 int posizione_x;
 int variazione_x; 
 
 void setup() {
 size(600, 600);
 posizione_x = 0;
 variazione_x = 1;
 textSize(30);
 strokeWeight(10);
 }
 
 void draw(){
 
 background(255,0,0);
 
 posizione_x = posizione_x + variazione_x;
 
 if (posizione_x > width){
 variazione_x = -1 ;
 }
 
 if (posizione_x < 0){
 variazione_x = 1 ;
 }
 
 
 point(posizione_x,300);
 
 text(posizione_x, 50,50);
 text(variazione_x, 50,100);
 
 }
 
```






### vvvvvvvvvvvvEsempio_4.08
// Variazione della posizione, attraverso tasti direzionali

```cpp

 int posizione_x;
 
 void setup() {
 size(600, 600);
 posizione_x = 300;
 textSize(30);
 strokeWeight(10);
 }
 
 void draw() {
 
 background(255, 0, 0);
 
 if ( keyPressed == true && keyCode == LEFT ) {
 posizione_x = posizione_x - 1;
 }
 
 if ( keyPressed == true && keyCode == RIGHT ) {
 posizione_x = posizione_x + 1;
 }
 
 if (posizione_x > width) {
 posizione_x = width;
 }
 
 if (posizione_x < 0) {
 posizione_x = 0;
 }
 
 point(posizione_x, 300);
 
 text(posizione_x, 50, 50);
 }
 
```




### Esempio_4.09
// Rimbalzi

```cpp
int posizione_x;
 int posizione_y;
 int variazione_x;
 int variazione_y;
 
 void setup() {
 size(800, 600);
 posizione_x = 100;
 variazione_x = 1;
 posizione_y = 200;
 variazione_y = 1;
 textSize(30);
 strokeWeight(10);
 }
 
 void draw() {
 
 background(255, 0, 0);
 
 posizione_x = posizione_x + variazione_x;
 posizione_y = posizione_y + variazione_y;
 
 if (posizione_x > width) {
 variazione_x = -1 ;
 }
 
 if (posizione_x < 0) {
 variazione_x = 1 ;
 }
 
 if (posizione_y > height) {
 variazione_y = -1 ;
 }
 
 if (posizione_y < 0) {
 variazione_y = 1 ;
 }
 
 
 
 point(posizione_x, posizione_y);
 
 text("X", 50, 25);
 text(posizione_x, 50, 50);
 text(variazione_x, 50, 75);
 
 text("Y", 150, 25);
 text(posizione_y, 150, 50);
 text(variazione_y, 150, 75);
 
 }
```



### Esempio_4.10
// Pong
```cpp
int ball_pos_x;
int ball_pos_y;
int ball_var_x;
int ball_var_y;

int bar_pos_x;
int bar_len;

int score;

void setup() {
  size(800, 600);
  ball_pos_x = 100;
  ball_var_x = 1;
  ball_pos_y = 200;
  ball_var_y = 1;

  bar_pos_x = 200;
  bar_len = 100;

  score = 0;

  textSize(30);
  strokeWeight(20);
}

void draw() {

  background(255, 0, 0);

  ball_pos_x = ball_pos_x + ball_var_x;
  ball_pos_y = ball_pos_y + ball_var_y;

  if (ball_pos_x >= width) {
    ball_var_x = -1 ;
  }

  if (ball_pos_x <= 0) {
    ball_var_x = 1 ;
  }

  if (ball_pos_y >= height) {
    ball_var_y = -1 ;
  }

  if (ball_pos_y <= 0) {
    ball_var_y = 1 ;
  }


  if ( keyPressed == true && keyCode == LEFT ) {
    bar_pos_x = bar_pos_x - 1;
  }

  if ( keyPressed == true && keyCode == RIGHT ) {
    bar_pos_x = bar_pos_x + 1;
  }

  if (bar_pos_x > width) {
    bar_pos_x = width;
  }

  if (bar_pos_x < 0) {
    bar_pos_x = 0;
  }



  if (ball_pos_x > bar_pos_x &&  ball_pos_x < bar_pos_x + bar_len && ball_pos_y == height) {
    score = score + 1;
  }



  line(bar_pos_x, height, bar_pos_x + bar_len, height);
  point(ball_pos_x, ball_pos_y);

  text("SCORE:", 20, 30);
  text(score, 150, 30);
}
```
