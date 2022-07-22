# Ai-robotics-week-2-tasks
**Task 1: Installing Ubunto and ROS in a virtual machine**  

**1. Install Oracle VM virtual box: https://www.virtualbox.org/wiki/Downloads**

choose the latest version and click on Windows Hosts 

![image](https://user-images.githubusercontent.com/108147030/180487488-dcfe3d5d-ff50-417b-8be7-dbb464b2acc8.png)

**2. Download Ubuntu 16.04.7 LTS (Xenial Xerus): https://releases.ubuntu.com/16.04/**

Choose 64-bit PC (AMD64) desktop image

![image](https://user-images.githubusercontent.com/108147030/180487843-c348c078-a376-4c49-b17f-3ef900461afd.png)

**3. Steps on installing Ubunto with ROS on the virtual machine:**

  1) From the Virtual box software, click on NEW.
  
  ![image](https://user-images.githubusercontent.com/108147030/180488271-dcc03e6b-ce42-49a8-ac4c-59909567d162.png)

  2) Choose the name and destination folder after that click on Next: 
  
  ![image](https://user-images.githubusercontent.com/108147030/180488658-8338fafa-5aa5-4089-aa31-28d8b7765748.png)
  
  3) Choose the maximum amount of memory from the green bar (do not pass through the green bar to the orange/red) then click Next:
  
    ![image](https://user-images.githubusercontent.com/108147030/180489550-13e3d47d-ee61-4beb-990d-19d87fa1fde6.png)
    
  4) Keep clicking Next until you get to the virtual hard disk size, its recommend to have it at 32GB then click on create:
  
  ![image](https://user-images.githubusercontent.com/108147030/180489852-35507ef6-acc8-4874-a480-784006d84575.png)
  
  5) Now click on your virtual machine then click on settings:
    
    ![image](https://user-images.githubusercontent.com/108147030/180490460-5ef1ce76-c402-4ed4-aa99-a018e2039fef.png)

  6) From settings go to system > processor and choose the maximum amout of CPU with only the green bar:
  
 ![image](https://user-images.githubusercontent.com/108147030/180490984-8c9242e9-004c-4412-83af-34dd1a61ce0a.png)




    i. Breadboard (small)
    
    ii. Arduino uno r3
    
    iii. DC Motor
    
    iv. npn transistor
    
    v. two resistors
    
    vi. push button
  
  3) Connect the circuit as shown below:
    
  4) use the following code to simulate the ON/OFF button circuit:
 
```ruby
int preState = 0;
int ledState = 0;
int pulsador = 7;
int motor = 3;
void setup()
{
  pinMode(pulsador,INPUT);
  pinMode(motor,OUTPUT);
  Serial.begin(9600);
  
}

void loop()
{
  int bState = digitalRead(pulsador);
  if((bState == 1) && (preState == 0)){
    
    if(ledState == 0){
      ledState = 1;
    }else if(ledState == 1){
      ledState = 0;
    }
  }
   digitalWrite(motor,ledState);
     Serial.print(preState);
     Serial.print(" ");
     Serial.println(bState);

     preState = bState;
      
}  
  ```
 
5) Click on start Simulation if you click on the push button the motor will start working and if you click on the push button again the motor will stop working.
