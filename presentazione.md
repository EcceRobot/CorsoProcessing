Possiamo suddividere il primo incontro in tre fasi:
1. Grafiche statiche
2. Grafiche in movimento
3. Grafiche interattive


``
// Esempio_1.00
// Si lancia applicazione vuota e si descrive cosa si vede e cosa viene messo realmente in atto
``


// Esempio_1.02
// Si cambia dimensione, si spiega cosa è una funzione, la sintassi, l'IDE, i commenti   
/*
size(x,y);
*/


// Esempio_1.03
// Andare a schemo intero   
/*
fullScreen();
*/




// Esempio_1.04 
// Si mostra la funzione background, le sue possibili varianti e il tool "Color Selector"
/*
size(500,500);
background(#RGB);
background(grey);
background(R,G,B);
*/

// Esempio_1.05 
// Si usa background due volte per mostrare l'ordine di esecuzione dei comandi 
/*
background(R,G,B);
background(R,G,B);
*/


// Esempio_1.06 
// Il punto, le dimensioni in pixel, l'orientamento degli assi 
/*
size(500,500);
background(0,200,0);
point(50,50);
*/

// Esempio_1.07 
// Dimensione del tratto, oridne di esecuzione anche qui! 
/*
size(500,500);
background(0,200,0);
point(50,50);
strokeWeight(5);
*/


// Esempio_1.08 
// Colore del tratto 
/*
size(500,500);
background(R,G,B);
strokeWeight(5);
stroke(R,G,B);
point(x,y);
*/


// Esempio_1.09 
// Disegno più punti 
/*
size(500,500);
background(R,G,B);
strokeWeight(5);
stroke(R,G,B);
point(x,y);
point(x,y);
*/


// Esempio_1.10 
// Disegno più punti, di colori diversi: ordine di esecuzione! 
/*
size(500,500);
background(R,G,B);
strokeWeight(5);
stroke(R,G,B);
stroke(R,G,B);
point(x,y);
point(x,y);
*/


// Esempio_1.10 
// Disegno più punti, equidistanti: formule! 
/*
size(500,500);
background(R,G,B);
strokeWeight(5);

point(x,y);
point(2*x,y);
point(3*x,y);
*/



// Esempio_1.11 
// Linee
/*
size(500,500);
background(R,G,B);
line(x1,y1,x2,y2);
*/



// Esempio_1.12 
// Rettangoli. Posizione x,y del vertice in alto a sinistra. Quadrato se l=a
/*
size(500,500);
background(R,G,B);
rect(x,y,l,a);
*/

// Esempio_1.13 
// Quadrato se l=a
/*
size(500,500);
background(R,G,B);
rect(x,y,200,200);
*/


// Esempio_1.14 
// Ellissi. Posizione x,y del centro. Larghezza e altezza (come il rettangolo)
/*
size(500,500);
background(100);
ellipse(100,100,100,50);
*/


// Esempio_1.15 
// Circonferenza. Ellissi con larghezza=altezza
/*
size(500,500);
background(200);
ellipse(100,100,100,100);
*/


// Esempio_1.16 
// Fill, riempimento delle figure chiuse
/*
size(500,500);
background(100);
fill(R,G,B);
ellipse(100,100,100,50);
*/


// Esempio_1.17 
// noFill, riempimento delle figure chiuse
/*
size(500,500);
background(100);
noFill();
ellipse(100,100,100,50);
*/

// Esempio_1.18 
// noStroke, riempimento delle figure chiuse
/*
size(500,500);
background(100);
fill(R,G,B);
ellipse(100,100,100,50);
*/



// Esempio_1.19 
// strokeWeight
/*
size(500,500);
background(100);
strokeWeight(n);
ellipse(100,100,100,50);
*/


// Esempio_1.20 
// stroke
/*
size(500,500);
background(100);
stroke(R,G,B);
ellipse(100,100,100,50);
*/

// Esempio_1.21 
// stroke
/*
size(500,500);
background(100);
noStroke();
ellipse(100,100,100,50);
*/




// Esempio_1.22 
// text
/*
size(500,500);
background(100);
text("TEST", 100, 200);
*/


// Esempio_1.23 
// textSize
/*
size(500,500);
background(100);
textSize(30);
text("TEST", 100, 200);
*/


// Esempio_1.24 
// colore del testo
/*
size(500,500);
background(100);
textSize(30);
fill(200,200,0);
text("TEST", 100, 200);
*/

// Esempio_1.25 
// gradazione di colore

/*
size(500,500);
background(100);
textSize(30);
fill(50,0,0);
text("ROSSO_UNO", 200, 50);
fill(100,0,0);
text("ROSSO_DUE", 200, 100);
fill(150,0,0);
text("ROSSO_TRE", 200, 150);
fill(200,0,0);
text("ROSSO_QUATTRO", 200, 200);
fill(250,0,0);
text("ROSSO_CINQUE", 200, 250);
*/




/* Fine prima parte: grafiche statiche

Riepilogo:

  - size(x,y);
  - background(R,G,B);
  
  - point(x,y);
  - line(x1,y1,x2,y2);
  - rect(x,y,l,a);
  - ellipse(x,y,l,a);
  
  - stroke(R,G,B);
  - strokeWeight(n);
  - noStroke();
  
  - fill(R,G,B);
  - noFill()

  - text(testo,x,y);
  - textSize(n);
  - fill(R,G,B);

*/







/*
Fino ad ora le funzioni utilizzate hanno sempre avuto un effetto a livello grafico:
- cambio dimensioni
- cambio colori
- primitive

ma le esistono funzioni che sono sorgenti di informazioni e possono essere utilizzate in alternativa un numero
*/



// Esempio_2.01 
// random() su text()
/*
size(500,500);
background(100);
textSize(30);
text(random(300) , 100, 200);
*/

// Esempio_2.02
// random() su point() 
/*
size(500,500);
background(0,200,0);
strokeWeight(10);
point(random(500),50);
*/

// Esempio_2.03
// second() su point() 
/*
size(500,500);
background(0,200,0);
strokeWeight(10);
point( second() , 500/2 );
*/



// Esempio_2.04 
// L'orologio rotto
/*
size(500,500);
background(100);
textSize(30);
text(hour() , 100, 200);
text(minute() , 150, 200);
text(second() , 200, 200);
*/


// Esempio_2.05
// Il primo programma ciclico (  Maiusc + AltGr + è ) ma ancora non corretto
/*
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
*/


// Esempio_2.06
// Il secondo programma ciclico (  Maiusc + AltGr + è ) ma ancora non corretto
/*
void setup(){
  size(500,500);
  background(200,0,0);
}

void draw(){
  strokeWeight(10);
  point( second() , 500/2 );
}
*/

// Esempio_2.07
// Il primo programma ciclico (  Maiusc + AltGr + è ) corretto
/*
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
*/


// Esempio_2.08
// Il secondo programma ciclico (  Maiusc + AltGr + è ) corretto
/*
void setup(){
  size(500,500);
}

void draw(){
  background(200,0,0);
  strokeWeight(10);
  point( second() , 500/2 );
}
*/


// Esempio_2.09
// millis() e mettiamo sempre un testo a schermo. Poi aumentiamo dimensioni della schermata. Poi riduciamo l'effetto con millis()/10
/*
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
*/


// Esempio_2.10
// Lo stesso parametro su più elementi
/*
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
*/


// Esempio_2.11
// Parametro su circonferenza

/*
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
*/



// Esempio_2.12
// Misuratore di livello con second() come input

/*

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
*/


// Esempio_2.13
// Grafiche NON parametriche: diagonali e centro dello schermo
/*
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
*/


// Esempio_2.14
// Grafiche parametriche: diagonali e centro dello schermo

/*
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
*/


// Esempio_2.15
// mouseX e mouseY

/*
void setup(){
  size(700,500);
}

void draw(){
  
  background(200,0,0);
  
  ellipse(mouseX, mouseY, 50, 50);

}
*/


// Esempio_2.12
// Una sorta di Paint

/*
void setup(){
  size(700,500);
}

void draw(){
  
  //background(200,0,0);
  
  ellipse(mouseX, mouseY, 50, 50);

}
*/



// Esempio_2.12
// Una sorta di Paint

/*
void setup(){
  size(700,500);
}

void draw(){
  
  //background(200,0,0);
  
  ellipse(mouseX, mouseY, 50, 50);

}
*/





/*

Riepilogo

abbiamo diversi ingressi:
 
 -random()

 -second()
 -minute()
 -hour()
 -day()
 -month()
 -year()
 
 -millis()
 
 -height
 -width
 -mouseX
 -mouseY

*/
