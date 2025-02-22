# Smart-feu-rouge
create by hakim
// C++ code
int red=2;
int blue=4;
int green=3;
int detects=7;
int vv;
void setup()
{
  pinMode(red, OUTPUT);
    pinMode(blue, OUTPUT);
    pinMode(green, OUTPUT);
      pinMode(detects, INPUT);



}

void loop()
{  vv=digitalRead(detects);
  if (vv==1){
  digitalWrite(red, HIGH);
    digitalWrite(blue, LOW);
    digitalWrite(green, LOW);
    
  delay(5000);
    digitalWrite(red, LOW);
    digitalWrite(blue, HIGH);
    digitalWrite(green, LOW);
  delay(2000); 
  digitalWrite(red, LOW);
    digitalWrite(blue, LOW);
    digitalWrite(green, HIGH);
    delay(5000);}
  else {digitalWrite(red, HIGH);
    digitalWrite(blue, LOW);
    digitalWrite(green, LOW);
    
  delay(1000);
    digitalWrite(red, LOW);
    digitalWrite(blue, HIGH);
    digitalWrite(green, LOW);
  delay(1000); 
  digitalWrite(red, LOW);
    digitalWrite(blue, LOW);
    digitalWrite(green, HIGH);
    delay(6000);}
  // Wait for 1000 millisecond(s)
}
