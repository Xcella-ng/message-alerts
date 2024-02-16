# Message Alerts
****

__An Xcella Plugin for displaying error and success messages__
### Developed by the Xcella Dev Team.

****
#### Features
****
* Add Message title
* Add type of message display
* Add displaying mode.

***
### Version
***
_message-alerts version 1.0_

### Usage
****
__Include the css file.__

~~~
<link rel="stylesheet" href="src/css/style.css"/>
~~~

__Include the js file.__

~~~
	<script src="dist/main.js"></script>
~~~

__Create a div with any class of your choice. This will be your message holder Egs;__

~~~
	<div class="your-class"></div>
~~~

__You can select your div class or pass in the class name directly as a string into the Msg class like so:__

~~~
	const holder = document.querySelector('.your-class');
	const msg = new Msg(holder);
~~~
or
~~~
	const msg = new Msg('.your-class');
~~~
__After passing in your message holder to the class as an argument, you will need to call the function ```init();```.  This init function takes in a config parameter which is an object. If you pass in an empty object, it means you want the default message configurations.__

**This config object takes some certain properties like so.**

~~~
	msg.init({
		msg: 'Hey this is a success message!!',
		type: 'success',
		mode: 'light',
		duration: 3000
	});
~~~
**The following properties and their neccesities are explained below.**

**```type```**: This is the most important property of all. It specifies if it is an error message or a success message. If this property is not found when trying to use your configurations. An error will be returned.

**```msg```**: This property specifies the message being displayed. i.e. the text to be shown.

**```mode```**: This property specifies the mode as shown in the example above! If you use a dark mode theme, message-alerts got your back. The default mode is the light mode by the way. This property is not important unless you want to specify a dark theme otherwise there's no need to pass in this property.

**```duration```**: This property specifies how long you want the message to show for as explicity shown by the name of the property! Just needed to say that. The default duration is 5000 miliseconds essentially 5 seconds

__Future Updates__
****
This is not the final working version of ```message-alerts```. This is ```version 1.0```. It's the first stable version. There will be more versions. Do checkout for more. 

_Thank you for checking out message-alerts 💜_

### Developed by the Xcella Dev Team.	


