# DC-motor-implementation-with-H-bridge
//below is the code i have used to program the dc motors to it's full potential.

//Motor1
const int MotorPin1 = 5;
const int MotorPin2 = 6;
//Motor2
const int MotorPin3 = 10;
const int MotorPin4 = 9;

//adjusting the output pins for each motor 
void setup() {
  
  pinMode(MotorPin1, OUTPUT);
  pinMode(MotorPin2, OUTPUT);
  pinMode(MotorPin3, OUTPUT);
  pinMode(MotorPin4, OUTPUT);
}

void loop() {
  //both motors will work for full throtle
  //initiating the the rpm to it's potential for each individual motor.
  digitalWrite(MotorPin1, LOW);
  digitalWrite(MotorPin2, HIGH);
  digitalWrite(MotorPin3, LOW);
  digitalWrite(MotorPin4, HIGH);
delay(10);
