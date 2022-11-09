# UnitreeMotorSDK_M80106
To control the M80106 motor, you need to prepare a `Unitree USB to RS485 module`.

- System Requirements  
Ubuntu 18.04 recommended, not a virtual machine.
- Development Environment Requirements  
`sudo apt install git build-essential cmake` 
## Select Your Platform
If your platform is arm64(like RaspberryPie.)  
Please edit `CMakeLists.txt` At line:`10`  
`target_link_libraries(motorctrl libUnitreeMotorSDK_M80106_amd64.so)`  
Modify `amd64` to `arm64`.

## SDK using example  
`git clone https://github.com/OnlineMC/UnitreeMotorSDK_M80106.git`  
`cd UnitreeMotorSDK_M80106`  
`mkdir build`  
`cd build`  
`cmake ..`  
`make`  

## Motor Running  

Now, access to motor power supply and communication lines.  
`sudo ./motorctrl`  
