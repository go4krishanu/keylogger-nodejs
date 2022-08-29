<h2> <b> KeyLogger </b> </h2>

<h2> <b> Install </b> </h2>

<code> npm install node-keylogger </code>

<h2> <b> Usage </b> </h2>

<code> 
var Keyboard = require('node-keylogger');

var k = new Keyboard('event0'); // 'event0' is the file corresponding to my keyboard in /dev/input/
k.on('keyup', console.log);
k.on('keydown', console.log);
k.on('keypress', console.log);
k.on('error', console.error);
</code>

<h2> <b> Events </b> </h2>

<code>
{ 
  timeS: 1347572085, // Timestamp ( Seconds part )
  timeMS: 741381, // Timestamp ( Microseconds part )
  keyCode: 17, // Keyboard code
  keyId: 'KEY_W', // Key ID /!\ Qwerty layout !
  type: 'keypress', // Event type
  dev: 'event2'  // Device
}
</code>
