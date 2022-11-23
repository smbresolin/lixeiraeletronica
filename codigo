## Alunas: Scheila Bresolin, Dandara Mascarenhas e Josiéli de Souza de Ramos ##


#include <Servo.h>

int distancia = 0;
int const echo = 5;
int const trig = 6;
int const servo = 9;

Servo servo_9;

void setup()
{
  pinMode(echo, INPUT);
  pinMode(trig, OUTPUT);
  Serial.begin(9600);
  servo_9.attach(9, 500, 2500);
}

long movimento(){
if(distancia <= 50) {
    servo_9.write(110);
    delay(2000);
    servo_9.write(0);
    delay(2000);
    servo_9.write(0);
    delay(2000);
}}

void loop()
{
  delay(1000);
  distancia = leitura();
  movimento();
  Serial.println(distancia);
}

long leitura()
{
  digitalWrite(trig, LOW); 
  delayMicroseconds(2);
  digitalWrite(trig, HIGH);
  delayMicroseconds(10);
  digitalWrite(trig, LOW);
  long duracao;
  duracao = pulseIn(echo, HIGH); 
  return ((duracao/2)/29.1); 
}
