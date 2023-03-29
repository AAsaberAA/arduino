```int beforeState = 0;
int presstime = 0;
void setup() {

  Serial.begin(9600);

  pinMode(7, INPUT);
}


void loop() {

  int buttonState = digitalRead(7);
  if(buttonState==1 and beforeState==0){
    presstime=presstime+1;
  Serial.println("hi~");
    Serial.println(presstime);}
  if(buttonState!=beforeState){
    delay(50);}
  beforeState=buttonState;
  delay(1); 
}
```
