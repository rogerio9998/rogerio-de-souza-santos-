# rogerio-de-souza-santos-#incluir <Ultrassônico.h>

#incluir <Servo.h>

#incluir "notas_musicais.h"

#definir pinoServo 7

#definir Trigonometria 2

#define Eco 3

#define B1A 8

#definir B1B 9

#definir A1A 10

#define A1B 11

InteirodistanciaD;

InteirodistanciaE;

Inteiropino de campainha =6;

flutuadordistancia0bstáculo =35;

Ultrassônicoultrassônico(Trig, Eco);

Serviço de serviço;

vazio configurar() {

Serial.começar (9600);

servo.anexar(pinoServo);

//pinos da ponte H Modo pin(B1A, SAÍDA); Modo pin(B1B, SAÍDA); Modo pin(A1A, SAÍDA); Modo pin(A1B, SAÍDA); Modo pin(buzzerPin, SAÍDA);

servo.escrever(90);

//Radar();vazio laço() {

Serial.imprimir (ultrassônico.Alcance(

se(ultrassônico. Alcance (CM) <= distar Andar(5);

Inteirostatus =Radar();

atraso (500);

se(estado ==1) {

Andar(2);

atraso (600);

Andar(4);

atraso (400);

Andar(5);

}

se(estado ==2) {

Andar(2);

atraso (600);

Andar(3);

atraso (400);

Andar(5);

}

se(estado ==0) {

Andar(2);

atraso (500);

Andar(4);

atraso (300);

Andar(5);

}

atraso (1000);

}

outro{

Andar (1);

}vazio Andar (Inteirodireção) {

se(direção ==1) {//anda pra frente Escrita digital (B1A, ALTO); Escrita digital (B1B, BAΙΧΟ); Escrita digital (A1A, ALTO); Escrita digital (A1B, BAΙΧΟ); }

se(direção ==2) {//anda pra trás Escrita digital (B1A, BAΙΧΟ); Escrita digital (B1B, ALTO); Escrita digital (A1A, BAΙΧΟ); Escrita digital (A1B, ALTO); }

se(direção ==3) {//faz curva pra dire Escrita digital (B1A, ALTO); Escrita digital (B1B, BΑΙΧΟ); Escrita digital (A1A, BAΙΧΟ); Escrita digital (A1B, ALTO); }

se(direção ==4) {//faz curva pra esqu Escrita digital (B1A, BAΙΧΟ); Escrita digital (B1B, ALTO); Escrita digital (A1A, ALTO); Escrita digital (A1B, BAΙΧΟ); }

se(direção ==5) {//FREIA Escrita digital (B1A, BAΙΧΟ); Escrita digital (B1B, BAIΧΟ); Escrita digital (A1A, BAΙΧΟ); Escrita digital (A1B, BAIΧΟ); r2D2();

}Inteiro Radar() {

atraso (1000);

servo.escrever (175);

atraso (1000);

distanciaD = ultrassônico.Alcance (CM)

atraso (1000);

servo.escrever(10);

atraso (1000);

distanciaE = ultrassônico.Alcance (CM)

atraso (1000);

servo.escrever (90);

se(distânciaD > distânciaE) {

retornar 1;//se tiver espaço na dir

}

se(distânciaD < distânciaE) {

retornar 2;//se tiver espaço na esc

}

se(distânciaD == distânciaE) {

retornar 0;

}

}

//Emite o som

vazio bip(Inteiroalto-falantePin, flutua {

Inteirox;

flutuadormicrossegundos PorOnda =10000

flutuadormilissegundos PorCiclo =1000/

flutuador loopTime = noteDuration * mj

para(x=0;x<tempo de loop; x++)atraso Microsegundos (micro

Escrita digital (speakerPi

atrasoMicrosegundos (micro

}

}

