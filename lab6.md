## Lab: Email - Specialized Automation

In this section we will learn about email automation.

So we will develop a task that does email automation.

But before we start to learn and develop our task, what, let's do a quick overview to see what our

task bot will do.

As you can see, I created an image that shows what our task bot will do.

![](./images/187.png)

So first we'll connect to our email and in this case we will use Gmail account.

So if you don't have a Gmail account, I suggest you create one.

It's very simple.

You can create a Gmail account in two minutes.

And after our bot connects to our email, it will apply a filter in the in our emails, in the emails

that we have in our inbox.

And then for each email that we have that matches the filter, the bot will reply to the email and save

the attachment.

If the email has some attachments, it will.

The bot will save it in our computer.

And then after process all emails, the bot then will send the email to the admin.

It can be in our to our account or the email that we have.

So the board will send the email and disconnect from our email and and terminate that task.

We'll start to develop our bonds.

So let's start by craving any one.

![](./images/188.png)

With the name of bots and their score emailed mission.

And let's create it.

So now that our board is created, let's develop the first step.

And the first step is to connect to our email account so then we can get emails from it, send reply

to emails and so on.

So to connect to our email account lets here search on actions for connect.

![](./images/189.png)

And here let's open where sales email.

Let's rock the action connect.

So now here we need to feel some properties of this action.

![](./images/190.png)

So on this section, we will set up the connection to a Gmail account.

So here let's select the option email server.

And now here those so far gmail accounts will be imap dot gmail dot com.

And the part will be 993.

And now we must provide the email address and the password to connect to our email account.

![](./images/191.png)

So let's start the credentials in a secure way by creating a credential in control room.

So to create a credential here lets over this button.

And now let's open the credentials page.

And now let's create a convention.

So to create the credential, let's click here on this button.

And here first, we need to define a credential name so it can be, for example, G.M. credential.

Now here on That's Your Roots.

So the first attribute will be the email address.

So attribute name can be email, so the input can be standard or user provided.

So in our case will be standard will be always the same email.

So let's select here standard.

Here we can uncheck the option.

Mask will not be the password here.

So now here.

Let's indicate our email address.

So now we must create another attribute for the password.

So let's click here on the plus.

![](./images/192.png)

So here as you would name will be password and we'll be standard will be always the same password.

And now here we must indicate the password.

But here to connect to our email accounts will not provide the password that we use to connect to our

Gmail account.

So we will generate a special password to be only used here on automation anywhere.

![](./images/193.png)

So generate this password lets first access to our gmail account.

So let's click here on manage your Google account.

![](./images/194.png)

And now here.

Let's open the security tab.

![](./images/195.png)

And now we'll appear here these option app passwords where we can generate a special password to be

used on a certain app where we want to connect to our email account.

But in order to this option be available to use, first we need to enable the two step verification.

![](./images/196.png)

So if it doesn't appear, make sure you enable first the two step verification.

So you just need to click here and follow the indications and then it should appear here.

This option.

So let's generate a password by clicking here.

Now let's indicate here our credential to connect our email accounts.

![](./images/197.png)

And so now let's hear create a new app password by clicking here on Select Tap.

Now let's like the adoption order and let's right here, for example, automation anywhere.

![](./images/198.png)

And now let's click here on generate to generate our app password.

![](./images/199.png)

And here we have the password.

![](./images/200.png)

So let's copy this password.

And let's face it here on the value of that she would password.

So let's paste it here.

And so now let's create our credential by clicking here on Create Credential.

![](./images/201.png)

So now that we have greater credential, we must create a locker where we will store the credential.

So to create a locker first, let's select here our credential.

And now let's click here on this button.

![](./images/202.png)

And now here we have to define the locker name so it can be, for example, emails locker, for example.

And now here we just have to go to consumers.

Select here our user.

![](./images/203.png)

And now we can create the locker.

So now that we have the credential and the locker created, let's go back again to why we're both.

And now here on credential, let's click on Big.

![](./images/204.png)

Now first we must select the locker that we have created and now will appear the credential that we

have created.

And now we must indicate that throughput.

So in this case will be the email for the username.

And not what's the same for the password?

So here, let's pick the credential.

![](./images/205.png)

Now let's get that throughput password.

So let's see if it's working well.

So let's just run and see if we get some exceptions or not.

So let's click here on run.

![](./images/206.png)

And as you can see, our boat has run successfully.

![](./images/207.png)

So the connection to our email, it's working well.

In the last lab, we connected the board to our email and in this one we will get the emails from

our inbox and apply a filter first to get the emails from our inbox.

We need to use the action loop.

So let's go here to actions and type loop and drag this action to our bot.

![](./images/208.png)

And this action will allow us to perform a loop and repeat the actions inside here until the loop breaks

and how he breaks when we don't have more emails in our case.

So this activity, this action will allow us to get our emails.

So let's see here our image.

![](./images/209.png)

So inside this loop we will have the action that will reply to the email and save the attachment and

until we have emails to process, we'll perform a loop for each email.

And when when done we don't have more, we'll go.

We'll break the loop.

So here in the properties we need to choose the iterator so we can perform a loop for each row in the

table, for each query data set for each value in the dictionary.

![](./images/210.png)

So here we have many types of iterators, but the one that we want is from email is for each mail in

mailbox.

So let's select this option.

And now we can apply a filter to the email.

So here in session name needs to be the same as we have here in the connection.

Here we can filter.

For example, if we just want to get rid of the emails, we click here.

If we just want to get rid of, click here.

I want to get all.

So click here.

Here we can say specific folder of the email that we just want to get emails from this folder.

I will let like this the inbox here, we can filter by the subject.

So for example here, for example, let's say that we just want emails that have the subject automation

and your course.

So if we type here automation anywhere, course we will just get emails with this subject.

And here we can apply a filter from to get just emails from specific senders.

So in this case we will use these ones.

So for example, if here are some emails, let's imagine that we just want to get emails from this one.

You should use one on your side.

For example, I will just copy this email and let's here just paste like this.

Here we can apply a filter by the date here.

Message format.

Let's click on play text to get clean text without HTML tags.

And now we need to assign a variable.

Create a variable that will contain basically the information of the email.

So to create the variable, let's click here.

![](./images/211.png)

And now let's for example, use the name Vic email.

And will be of the type dictionary.

So basically variable of type dictionary is a variable that contains the many values.

For example, in this case our variable will contain uh, the sender or the sender of the email will

contain the subject.

The body so contains multiple values, this type of variable.

So now let's just create the variable.

![](./images/212.png)

And now we have already to read to get the email.

So we will now test if it's working.

So to see our the emails that we are getting in the visual way, we will use the action message box

that will display to us in the message box, the text of our email.

So let's drag this message box inside the loop so it needs to be inside to for each email performs this

action that will shows the text of each email.

![](./images/213.png)

And now we need to specify, uh, the message that the our action will display.

So here in the message property, we will define to get the subject of each email and the the message.

So let's type here subject for example.

And now we need to call our variable that we created the dictionary and just get the value of the subject.

So let's see or click on this button to call our variable.

![](./images/214.png)

And let's click here on email.

Our dictionary.

And now we need to say the key of the subject.

![](./images/215.png)

So here we we type the key and the key will give us certain value.

So I have here a page that of the documentation of automation anywhere that says the keys.

For example, if we want to get just the email subject, we need to type the key email subject.

![](./images/216.png)

If we want to get just the email message, we need to type the key email message.

So just works like this.

It's very simple.

So for example, in this case we need to type the key email subject and insert.

And in this way we will get just the email subject here.

And now let's here type enter.

And let's type here message.

![](./images/217.png)

And we will call here just the value of the message.

So it's the same.

We can click here or directly let's do dollar, sign the email.

And now let's open here and just delete this and let's type the key email message and dollar sign again.

And now we should just get emails from the sender.

The sender in my case, and in plain text and with a message box for each email saying the subject and

the message.

So let's go test if it's working, let's click here on Run.

It's deploying in our computer.

![](./images/218.png)

So we've already got our first email, so let's check.

So here on my account we can see, uh, automation anywhere.

Course.

![](./images/219.png)

Let's see.

It's from the email that I defined just to get emails so you can see here, Let's close.

![](./images/220.png)

We got another email, let's verify.

So was formed from this one.

We can see here it's the center that we specified to get just emails from.

And now should close the automation.

So as you can see, we applied with success.

![](./images/221.png)

We are getting the emails and we are applying a filter and we can so display get the values from the

email like the subject and the message.

And in the next lab we will learn how to reply to emails.

So we will develop our test bot to reply to the sender of each email that we get.

In the last lab we develop the bot to get emails and apply a filter.

And in this one we'll develop the bot to reply to each email.

![](./images/222.png)

So to reply to each email we need to use the action reply from email and drag it inside the loop to

so to reply to each email to each loop.

So.

Here in this section, we have some properties we can specify here, some people, some emails in CC,

for example, send attachment.

![](./images/223.png)

It's optional.

Here we define if we want, send the email as plain text or HTML.

Let's use the plain text here.

We can type the message that we want send.

So for example, in this case, let's say email read.

VI.

Automation anywhere to squat.

And that's your thought here.

We can say if you want to include a message, a default message from automation anywhere that is encouraging

to protect the environment.

Let's let let's check this option.

And now we need to say the email server.

So, so we need to say here the host of our email server is smtp.gmail.com, the email port, the email

server port, it's four, six five.

And here we need to check this option to do the authentication.

![](./images/224.png)

So now let's pick our credential here.

![](./images/225.png)

Let's click on our log credential email and here the email attributes.

And now to the password.

It's the same.

Let's pick our lock our credential and attribute password.

I'll.

Let's confirm.

![](./images/226.png)

So in this way the bot should reply to each email that we get.

So let's here click on Run and now I will open the the email that the bot will reply the the email that

we defined in the filter.

![](./images/227.png)

So I will open near the email box.

![](./images/228.png)

The bot is starting to run.

So we got now our emails.

![](./images/229.png)

Our first email.

Let's close.

And now the bot should reply to the email.

So for example, let's here just refresh and we can see the bot did a reply to to the email.


![](./images/230.png)

Let's see here.

Like you can see the, the message that we defined and the default message that is encouraging to protect the environment.

![](./images/231.png)

And now the bot should reply to one more email.

So we have this one.

Let's close and now.

We will refresh our email box so you can see that the bot did a reply.

![](./images/232.png)

So let's open just the email and we can see here the message.

![](./images/233.png)



Now we will learn how to save the attachments included in the email.

So it's very simple.

To save the attachments, we need to go to actions and type save attachment.

So let's use this action.

![](./images/234.png)

And drag it inside the loop to to do for each email.

And now we just need to say a folder where we want store the attachments.

So.

So for example, I will create a folder here, let's say.

Automation.

![](./images/235.png)

Anywhere attachments.

![](./images/236.png)

And now let's copy the path and let's paste here.

And now we need to say here, if we want to overwrite files.

![](./images/237.png)

So, for example, if we got two attachments with the same name, the last one, if we have this option

checked, will overwrite the the one stored.

So let's check this option like this.

And so in my case, you can see here that we got we have here two emails that we are getting from this

sender and the the two emails have the same attachment with the same name.

![](./images/238.png)

So in my case should just be stored one.

So, um, let's see here what will happen.

So I will open here my task bot and just click here on run.

![](./images/239.png)

So we already got our first email.

![](./images/240.png)

Let's close the message box.

And now let's see if you already have the attachment on our computer.

So you can see here in the final folder that we defined in the action we have here.

![](./images/241.png)

So the attachment that exists on the email.

So now let's close this message box and now we can see here that we just have one PDF because of the

overwrite.

![](./images/242.png)

So they have the same name.

Now we will develop our task bot to in the end of the loop.

So after get all emails, send a message to a specific email.

So to send a message to a specific email we need to use the action send.

![](./images/243.png)

So let's type here, send and drag this action after the loop.

So not inside the loop after the loop.

So by this way the bot will just use this action after get all emails.

![](./images/244.png)

And as you can see here, we use the reply here we will use the sensor.

So the difference here is that the in reply action, we don't need to say the the email that we want,

send the email because automation anywhere already knows when we are getting each email in the send

one we need to say so like you can see here the address, the email address that we want, send the

email.

So first, let's say here the address.

So you type the one address that you have or you know, I will type here one specific address.

So let's type here.

Now here we can see the subject.

So let's say automation, execution, for example, the subject of the email.

So here the email.

So we will send in plain text here.

The message, let's say, for example, automation executed with success.

So now we need to say the address that the bot will use, the email that the bot will use to send the

email.

So I will type here.

One email.

Now we need to say here the email server also is the smtp.gmail.com.

And now the part is.

Four, six, five.

So let's live like this.

Let's hear shake through use connection.

Now let's click on through to use the authentication.

![](./images/245.png)

And now we just need to pick the credentials.

So let's click here in our locker credentials, email and now email attributes confirm.

![](./images/246.png)

And now let's pick our password.

And password attributes confirm.

![](./images/247.png)

And now the what's after process.

Ishmael should send a message to the email address that you specified here on the property.

So let's test if the automation is working.

So if the test bot is sending in, then the email.

So let's just remove this action because isn't needed.

So let's remove, let's click here and delete action.

![](./images/248.png)

And now let's just run our bot.

So let's click here and let's see what will happen.

So you can see here that the bot has run successfully the automation.

![](./images/249.png)

And now let's close this pop up and I will open the email that should get the the email that the bot

sends.

![](./images/250.png)

And now as you can see, I got the email with the subject automation execution.

So saying that the automation executed with success.

