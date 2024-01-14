## Lab: Designing Complex Workflows

In this section we will develop a task bot that uses web browser.

So in this image we can see what our task bot will do.

![](./images/93.png)

So we'll be something like a clothing consultant.

So basically our bot will open the Google Chrome, the browser and search, for example, Lisbon weather

in Celsius.

So we'll obtain the temperature.

The Celsius in Lisbon can be other city and extract the value of the Celsius.

And let's say for example, the temperature, the Celsius, it's less than ten.

![](./images/94.png)

So if it's less than ten, the our bot will say to call.

Here's something.

For example, if the Celsius are between 10 and 25, our bot will display this message and if the temperature,

the Celsius are greater than 25.

So our bot will display this message saying that it's pretty hot outside to wear a shorts, for example.

And in the end we will close the browser and terminate the execution.



We did a quick overview about the Test squad that we will develop in the next labs.

And in this one we will create the Test squad and learn how to open the browser.

So.

So let's open the folder and for example, create the bot from here.

![](./images/95.png)

Let's say bot clothing consultant.

Now let's click on Create.

![](./images/96.png)

So, the broth is already created.

![](./images/97.png)

And our goal for this lab is to open the browser through the task bot.

So let's learn how we can make it happen.

So let's drag this more to the center and the action that will enable us to open the browser.

Is the action open from browser?

![](./images/98.png)

So let's click here and now just drag the action open.

So let's drag to here so we can see here by the properties that we have three ways to open a website.

![](./images/99.png)

For example, through a new window, a new Google Chrome application, a new tab or using existing tab.

So let's use the new window now browser.

Let's use the chrome and it's very important to always define the specific browser.

![](./images/100.png)

I just don't recommend to use the option default.

Always specify the browser that you want to use.

So let's say here Google Chrome and we want to open in the google.com.

So let's type here.

WW double.google.com.

So if you run our bot it should open a new Google Chrome application in Google.com.

So let's test.

So let's run here.

![](./images/101.png)

So the bot is already running.

And as you can see, the bot started a new Google Chrome in Google.com.

![](./images/102.png)

The URL that we indicated here on link to open property.

Lastly, we developed our taskbar to open the browser and it is one we will learn how we can

perform the search.

So to appear to us the temperature.

![](./images/103.png)

So let's search for the action capture from recorder, drag it after the open browser and this action

will allow us to type to the bot, type the text here and perform the search.

So now first we need to select where we want to perform certain action with this action.

So it's on the browser.

So click here on browser.

![](./images/104.png)

Now let's refresh Windows to appear this Google.com tab.

Make sure you have one new window in this URL.

So if you click here we can see.

![](./images/105.png)

So this one, let's just click so we can see here the link of the page.

Now we need to indicate the field where we want the bot to type the text.

So let's click on Capture object.

![](./images/106.png)

And now we can see here the red lines.

![](./images/107.png)

It's an area that we are indicating.

So let's indicate this area where the what should type the text.

So right click.

So the action already captured the field that we indicated.

So let's scroll a bit and now we need to choose the action.

So we will click here.

We can see some actions like get property, append, text, click, but the one that we want is to set

text.

![](./images/108.png)

So let's choose this one.

Now we can see here that appear these properties.

So here we indicate the text that we want the bot to type on the Google.com tab.

So here we just type, for example, Lisbon weather in Celsius.

![](./images/109.png)

So if you run right now, the bot, the bot should so open google.com tab and type this text on this

field.

So let's close the google.com.

This one.

And let's run the bot.

![](./images/110.png)

So the bot is already running.

As you can see, we got here a new Google.com tab and now the bot should type the text that we have

typed on the action.

So as you can see the bot set the text Lisbon weather in Celsius.

![](./images/111.png)

So now we just need to develop the bot, perform the search and we have two options we can indicate

to the bot to click on this button, the Google search button, or we can develop the bot to perform

the command enter.

So let's use the second option that I said the bot to perform the key enter.

So here, let's close this popup 

![](./images/112.png)

and now let's scroll a bit and here where we set the text that we want

the bot to type on the field, let's use click on this button where it appears when you over insert

keystroke and now let's click here on Enter.

![](./images/113.png)

So by this way, after the bot types the text set, the text will perform the key enter.

So let's test if it is working well.

So I will I will close again this tab.

And now let's run again the bot.

![](./images/114.png)

So the bot is already running.

So it's typing the text and now, as you can see, perform the search with success.

![](./images/115.png)


In the last lab we developed, our task was to perform the search on Google.com.

So basically it already types on this field, this text, and performs the search.

![](./images/116.png)

And in this lab we will develop the bot to extract the Celsius value the temperature in the city.

So the action that will allow us to extract the value is the action capture.

So let's search for capture action from recorder again and let's drag it after this capture action.

![](./images/117.png)


![](./images/118.png)

So now we need to set the browser.

So click here on browser and now make sure you have the browser on this page can be another city, but

make sure it's on this where appears so the temperature on the city.

And now let's refresh the windows.

![](./images/119.png)

And now we can see here the window Lisbon weather in Celsius.

So let's click here.

![](./images/120.png)

And now we need to capture the object.

So we need to indicate where we want to extract the certain value.

So let's click here.

So now we can see here the red line.

So the area that we are indicating.

So when appears like this here on the Celsius value, these red lines just to left click.

![](./images/121.png)

So we can see here the area that we indicated, the Celsius value, the temperature.

![](./images/122.png)

And now let's scroll a bit.

We need to indicate the action that we want to perform.

![](./images/123.png)

So let's click here.

And so the action that will allow us to extract the value is the action get property.

So let's click on this action.

![](./images/124.png)

And now we need, say, the property name where it contains the value that we want.

So the temperature.

So here we can see the properties.

![](./images/125.png)

And if we open so may appear to you like this, just click to open all properties we can see here.

So here Innerhtml contains the value 11 and as you can see, that means there we can get the temperature

value, the Celsius value.

So let's copy these property name Innerhtml And now let's paste it here on property name.

Uh, let's just clear these spaces.

And now after this, we need to create a variable that will contain the output.

So the output will be the value.

So let's create the variable.

![](./images/126.png)

Now let's give the name of temperature.

And it's of type string.

It's right.

So let's just create the variable.

![](./images/127.png)

So the value will be stored.

So the value extracted will be stored in this variable.

So to see if it's working well, let's use a message box.

![](./images/128.png)

And let's drag it after the capture action.

This one.

And now here in the message to display, let's type here temperature in Celsius.

And now let's call the variable temperature.

So by this way, the board should display here the extracted value.

So let's run our bot.

![](./images/129.png)

So I will just close this tab and let's run.

So we already got here the Celsius value.

So let's see if the bot will display the right value.

![](./images/130.png)

So as you can see here, temperature in Celsius nine.

As you can see, the bot is extracting well, the temperature, that's all for this lab.

![](./images/131.png)

Next we will take a look to exception that may appear to you if you try right now another city.

So we developed our bot to extract the Celsius value.

And in this one we'll know how to avoid exception that will appear to you if you try right now to search

another city.

So let's click first on the action that types into Google.com and performs a search.

![](./images/132.png)

And let's change the value of the city.

So let's change the city name.

So let's here select Lisbon and the type, for example, Madrid.

And let's run our test squad to see what will happen.

So let's click here.

![](./images/133.png)

So the bot is already running.

I'm typing the text.

![](./images/134.png)

So after some time we can see that the bot didn't show to us the six.

So the Celsius value.

![](./images/135.png)

Let's discover why.

So let's go to our bot.

So we can see here one exception on our task bot.

![](./images/136.png)

And we can see that says that cannot find window or application.

So let's cover why this exception happened and how to avoid it.

So, the way to solve this exception is very simple.

![](./images/137.png)

So if we go here to the recorder, capture action, the one that extracts the Celsius value, we can

see here the property browser title and we can see the value of Lisbon weather in Celsius, Google Search

and what that means.

![](./images/138.png)

That means that this action will always expect and wait to find a browser title with the name Lisbon

weather in Celsius.

So this title and if the action doesn't find this browser title, will give us an exception saying that

it didn't find a tab with this browser title.

So if we go here to google.com and search.

For, for example, Rio Janeiro.

Weather in Celsius.

![](./images/139.png)

We can see that the browser title is different, so we type another city.

![](./images/140.png)

The browser title will be another different.

And so by this way, we'll give here a error because isn't exactly this browser title that we are seeing

here.

So how we can solve that by using dynamic match.

So how we can do that.

We if we go here, uh, on browser title, let's click on browser to make this editable.

So let's click here.

![](./images/141.png)

And now let's refresh the windows.

Now let's.

So we are seeing here real generator is Celsius.

Let's select this one.

![](./images/142.png)

So here we can see the browser title and to make the browser title dynamic in in this case, accepting

different city names, we need just to select so the city name and replace it by a wild card.

So by this way, the action will search for a window that contains a text.

![](./images/143.png)

Some type of text can be some name or more than one name.

And then after that, containing in last weather in Celsius, Google Search.

So by this way, we'll work without any exceptions.

So.

Let's save our bot.

And now here on recorded capture action, we can, for example, type here, um, Kurdish and space.

And now let's run our bot.

So let's run.

![](./images/144.png)

I will close this tab.

So the boat is already running.

![](./images/145.png)

And let's see if we'll give some examples.

So as you can see, without exception, the bot extracted with success, the Celsius value.

Now we will develop the bot to show to us a message with a recommendation depending on the

city temperature.

So to make the boat show to us a certain message, depending on the city temperature, we need to use

conditions.

So to use conditions, let's search for the if action.

![](./images/146.png)

And let's click here on live and let's drag the infection after the message box.

So this action allows us to set conditions one or more.

![](./images/147.png)

And if the condition is true, the bot will perform the actions inside the action.

So the actions that are here, if not, will not perform this action.

So here on condition, let's we can see a lot of types of conditions.

![](./images/148.png)

So we want the number one.

So we want the number condition because we extract a number the Celsius value.

![](./images/149.png)

And now we need to indicate the source value.

So we need to indicate here, uh, the Celsius value that is stored in this variable that we created

of type string.

![](./images/150.png)

And if we click here to insert the variable.

![](./images/151.png)

We can see that doesn't appear our temperature variable.

Why?

![](./images/152.png)

Because it's of the type string, not of the type number.

So before we set the condition, we need to transform the value of string to number.

To do that, let's cancel here and let's type here on actions to number.

So this action from string, let's click here on string and let's drag these actions.

![](./images/153.png)

So this action allows us to convert a string to numbers.

So here we enter the string.

So let's call here the temperature variable.

![](./images/154.png)

And let's click here.

And now we need to create a new variable that will be of type number.

So let's click here on Create Variable.

![](./images/155.png)

Let's type here number.

A temperature.

And let's click on create.

And now, yes, if we go to our if action, click here.

And let's click on insert value.

We can see our variable that we created right now.

![](./images/156.png)

So let's click in this one.

Yes, insert.

And now we need to set the operator.

So let's set the operator less than and the target value will be ten.

So if the value, the extracted temperature is less than ten, we want the bot show us the message.

So this one that shows too cold, we are something that keeps you warm.

So now we need to basically use a message box.

![](./images/157.png)

Inside the infection.

So, oops, let's drag it inside the infection.

And now let's enter here the message.

So basically, the message is too cold.

Yea, something that keeps you warm.

A jacket, for example.

So let's type here.

So let's run our test squad to see if it's working well.

So let's click on Run.

![](./images/158.png)

So the boat is already running.

![](./images/159.png)

Its typing must read editor in Celsius so we can see that the temperature in Celsius is five.

![](./images/160.png)

So the bot should show to us a message that we defined right now.

So let's close this message box and as you can see, our bot shows to us the message to cold here,

something that keeps you warm and jacket, for example, because the temperature the value is less than

ten like we defined here.

![](./images/161.png)

So now you just need to define the other conditions.

So now let's use the else if action.

![](./images/162.png)

So basically by this way, with this action, we can put side by side the conditions.

So let's here define the condition.

So let's search here for number condition and now we'll do the condition.

So let me show to you the condition.

So now we will define this one.

So if the temperature is measured than ten and less or equals than 25, the bot should show to us this

message.

So here in source value, let's call our variable number temperature insert.

![](./images/163.png)

And now in our operator, let's choose the greater than or equal to.

So if the temperature is equal or major than ten.

And now the target value is ten.

So.

So, now with the final this condition in the action and now we need to find to this one so if the

temperature is.

Equal or greater than ten.

And if the temperature is less or equal to 25, I made a mistake.

It's end isn't.

Or so if it's between these values, the temperature or if it is 10 or 25.

So the task should go through here.

So now here, let's click on the elseif action.

Let's click on Add condition.

Now we have these two options.

Let's click on the end.

And now here let's search for number condition.

Another source.

Value number.

Temperature.

And now here, if it's less than or equal to 25.

And by this way, if the temperature it's between these values, 10 or 25 or if it is 10 or 25, the

bot will show this message to us.

![](./images/164.png)

So let's type here message box in actions.

And and the message will be so reasonable.

Whether the lights, jackets.

If you want.

And now we need to define one more condition, the one that if the temperature is measured on 25.

So let's go here to actions search for the if.

If.

Click here on live.

And now we will use the action.

![](./images/165.png)

So basically, let's drag it after the elseif condition and this action will execute the actions inside

it if these ones are all false.

![](./images/166.png)

So if the temperature is less than ten and if the temperature isn't major or equal to ten or less and

equal to 25, so the bot will execute the conditions inside here.

So we don't need to set here a condition.

We just need to search here for the message box.

![](./images/167.png)

Let's rock it here.

And now let's set here the message.

Pretty hot outside.

You can wear shorts.

![](./images/168.png)

![](./images/169.png)

And by this way, we should have a working clothing consultant bot that shows recommendations based

on the temperature.

Now we will finish our automation and test all the conditions.

So to finish our automation, we will want the bot to close the tab that it will open to to perform

the search and extract the Celsius value of the city.

So here in actions, let's use the action, simulate keystrokes and let's drag it after all actions.

![](./images/170.png)

So in the end of the automation and we will send the keystroke control w to close the tab.

So first we need to say the window that we want to send these keystrokes.

![](./images/171.png)

So basically the window is the one that we extract the value.

So it's this one and we can get the window by this variable.

So here let's type dollar sign, variable window, weather, window three, Let's select this one and

we can see here the window title.

And now here we perform.

We say the keystrokes, the keys that we want to send.

So basically, let's click here on this button.

Let's click on control button and now let's click close.

![](./images/172.png)

And now between the these tags, let's type here the W.

So in this way the bot will will send the control plus W keystrokes to close the tab.

So let's test if it's working.

So I will close this tab.

And now let's run our test bot.

![](./images/173.png)

So the water already extracted the value.

![](./images/174.png)

So let's close the message box.

And so now after we close this message box, the bot should close this tab.

![](./images/175.png)

So let's click on close.

And now as you can see, the bot closes the tab and runs successfully.

![](./images/176.png)

So now let's test our automation in our conditions.

So I already picked three cities that each one meets one of these conditions.

So the first one will be johnsburg.

So here in our first in the first action Capture, let's type here.

![](./images/177.png)

In my case I will type here johnsburg.

And just make a key here, the space.

And now let's run our bot.

![](./images/178.png)

So click on Run.

So the bot already performed the search and extracted the value.

So we can see the value is 23.

![](./images/179.png)

So the bot should show to us the message is exactly the reasonable whether is the.

So basically in a second condition.

So let's close just close here and.

So the vote run successfully.

![](./images/180.png)

So this condition so did well.

So now let's run the second city.

So.

Will the real Janeiro.

So I will type here.

Field generator.

So let's type here.

Now let's run.

![](./images/181.png)

And this one I already checked should meet the third conditions.

So the bot is already typing here.

![](./images/182.png)

Regional weather in Celsius.

So the temperature is 27.

![](./images/183.png)

So our bot should show twas the third.

It's right now.

Right now pretty hot outside.

You can wear the shorts.

So now.

Now we just need to test one more condition.

This one.

So I will pick the Madrid city.

So here I will type Madrid.

So let's type here Madrid and let's run our bot.

So I already check the temperature.

It should match the first the first message.

![](./images/184.png)

So we can see here.

Temperature in Madrid in Celsius is four.

![](./images/185.png)

So she'll show to us to call exactly match the first condition.

So our bot is working well.

![](./images/186.png)

We already have a working bot, so it's working well.