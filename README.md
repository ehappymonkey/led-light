# led-light intensity
import RPi.GPIO as GPIO
from time import sleep

GPIO.setmode(GPIO.BOARD)
GPIO.setup(37,GPIO.OUT)
#利用pwm调节亮度
pwm = GPIO.PWM(37,100)  
pwm.start(50)
while True:
#change this number to change the intensity
   pwm.ChangeDutyCycle(1)
   
   
#led time
import RPi.GPIO as GPIO
from time import sleep

GPIO.setmode(GPIO.BOARD)
GPIO.setup(37,GPIO.OUT)

while True:
   GPIO.output(37, GPIO.HIGH)
#change this number to change the lighting time   
   time.sleep(10)
   GPIO.output(37,GPIO.LOW)
   time.sleep(1)

   
