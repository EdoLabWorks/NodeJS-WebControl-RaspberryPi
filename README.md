## NodeJS-Raspberry-WebControl

A start-up web control project for Raspberry Pi 3 using array-gpio, express, angular and socket.io.

Turn ON/OFF actuators/peripherals using your mobile device.

Note:
 
Works on node v5.0 LTS or v6.5 latest and above.

### Raspberry Pin Setup

Using the GPIO physical pin number, choose the pins (6 max.) you want to use as inputs and outputs.

Configure the pins in the app.js file as shown below. 
~~~~
gpio.setInput(pin1, pin2, ... pin6); // input
gpio.setOutput(pin1, pin2 ... pin6); // output
~~~~

### Features

- Real-time update of GPIO pin state.
- Control remote devices from within your private network using your mobile device browser.  
- Get real-time update during loading or refreshing of your browser everytime.
- You can also control your Raspberry Pi from your laptop or desktop PC using the IO-ControlModule-Raspberry utility. 

### Installation 

Git clone or download the application from your Raspberry Pi computer.

In the root folder, install all dependencies.
~~~~
$ npm install
~~~~

Run the application as shown below. 
~~~~
$ node app
~~~~

Enter the `ip address` of your Raspberry Pi as shown below to start your web control from your mobile device. 
~~~~
http://<ip address of your raspberry Pi>:3000/
~~~~
e.g.
~~~~
http://192.168.1.125:3000/
~~~~

### License

MIT
