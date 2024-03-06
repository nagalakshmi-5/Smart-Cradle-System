int soil=A0;
int buz=D1;
int relay=D5;
int light=D2;
int threshold=1024;
void setup(){
pinMode(soil,INPUT);
pinMode(buz,OUTPUT);
pinMode(relay,OUTPUT);
pinMode(light,INPUT);
Serial.begin(9600);
}
void loop(){
int m= analogRead(soil);
Serial.println(m);
if(m<threshold){
  Serial.println("wet soil");
  digitalWrite(buz,1);
  delay(500);
}
else{
  Serial.println("dry soil");
  digitalWrite(buz,0);
  delay(500);
}
int m1=analogRead(light);
if(m1>90){
  Serial.println("darkness");
  digitalWrite(relay,0);
  delay(500);
}
else {
  Serial.println("Brightness");
  digitalWrite(relay,1);
  delay(500);
}
}
