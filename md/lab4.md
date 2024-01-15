## Lab:	Understanding Types of Bots

## Introduction

This lab focuses on exploring the Bots page in Automation Anywhere, understanding how to organize and manage bots, and examining various functionalities and features.

## Exploring the Bots Page

### Accessing the Bots Page

1. Navigate to the Bots page in Automation Anywhere where developer bots are listed.

   ![Bots Page](./images/50.png)

### Organizing Bots

1. Observe the default folder structure and existing bots, such as the 'bot notepad'.
2. Learn how to create and organize bots into folders for better management.

   ![Creating Subfolders](./images/51.png)

3. View the newly created folder in the Bots page.

   ![Created Folder](./images/52.png)

### Managing Task Bots

1. Understand how to copy task bots to different folders for organization.

   ![Copying Task Bot](./images/53.png)

   ![Bot in New Folder](./images/54.png)

2. Confirm the action and view the bot in the new folder.

   ![Task Bot Management](./images/55.png)

3. Explore additional management options like deleting, copying, and editing task bots.



### Analyzing and Running Bots

1. Analyze the design and configuration of task bots.

   ![Viewing Bot Design](./images/56.png)

2. Understand the limitations of bot analytics if not developed specifically for it.

3. Learn how to run bots directly from the Bots page.

   ![Bot Analytics](./images/57.png)


## Working with Credential Space and Global Values

### Credential Space

1. Use Credential space to store sensitive data like passwords for use in automations.

   ![Running Bots](./images/59.png)

### Global Values

1. Understand how to access and use global values that are accessible to all automations.


## Understanding Packages

1. Learn about different packages available for use in task bots.

   ![Bot Packages](./images/61.png)

2. Explore specific packages like Data.table and Database packages.


A package is a basket of actions.
For example, we have a package called Data.table that allows us to work with data tables.
Database package is basically a package that contains a bunch of actions to work with the database.


In this section, we will learn about using variables, triggers, and the recorder feature in Automation Anywhere. This will include creating a variable, setting up triggers, and utilizing the recorder to automate tasks.

## Part 1: Understanding and Creating Variables

### What is a Variable?

- A variable in Automation Anywhere allows you to store a single value or multiple values for use in tasks.

### Creating a Variable

1. Navigate to your bot page and select your bot. For this example, we'll use a bot named "Notepad."
   
   ![](./images/62.png)

2. Open the bot to view the actions, triggers, and variables.

3. To create a new variable, click on the 'Variables' section and then click the plus icon.

   ![](./images/64.png)

4. Enter a name for your variable, such as 'message'.

   ![](./images/65.png)

5. Optionally, add a description.

6. Choose the variable type (String, Number, Date Time, Boolean, etc.). For this lab, select 'String'.

7. Set a default value for the variable, e.g., 'Hello World'.

   ![](./images/66.png)

8. Incorporate the variable into your task. In the recorder action, replace the hardcoded text with your variable.

   ![](./images/67.png)

### Using the Variable in a Task

1. Clear any existing text in the action where the variable is to be used.

   ![](./images/68.png)

2. Insert the variable into the action. This can be done by typing the variable name with a dollar sign (e.g., `$message`) or by using the 'Insert a Value' feature.

   ![](./images/69.png)

3. Test the bot by running it to ensure it types 'Hello World' in Notepad.

   ![](./images/71.png)


We'll use variables to receive outputs from actions to give, to give values to actions.


This section will guide you through using triggers and the recorder feature in Automation Anywhere. You'll learn how to automate tasks based on specific triggers and record actions for repetitive tasks.

## Part 1: Understanding and Setting Up Triggers

### Exploring Triggers

1. Open your notepad task bot in Automation Anywhere and navigate to the 'Triggers' section.

   ![](./images/73.png)

2. Understand that a trigger enables a task to run automatically in response to an event on your device.

3. Examine the types of triggers available.

   ![](./images/74.png)

### Setting Up a Hotkey Trigger

1. Decide to use a hotkey trigger for simplicity.

2. Drag the hotkey trigger into your bot workflow.

   ![](./images/75.png)

3. Define a hotkey combination in the hotkey trigger properties. For example, use Ctrl + A.

   ![](./images/76.png)

4. Save your bot configuration.

### Running the Bot with the Trigger

1. Run the bot and observe it waiting for the trigger.

   ![](./images/77.png)

2. Press the defined hotkey combination and watch the bot execute its task.

   ![](./images/78.png)

   ![](./images/79.png)

## Part 2: Using the Recorder Feature

### Creating a New Task Bot for Recording

1. Navigate to the 'My Bots' section and create a new task bot in the appropriate folder.

   ![](./images/80.png)

2. Name the bot (e.g., 'Bot Recorder') and begin editing.

   ![](./images/81.png)

### Utilizing the Recorder

1. Access the recorder feature within the bot.

   ![](./images/82.png)

2. Choose the window to record your actions. For this exercise, select the Calculator app.

   ![](./images/83.png)

### Recording Actions

1. Open the Calculator application.

   ![](./images/84.png)

2. Refresh the window list in the recorder to detect the Calculator.

   ![](./images/85.png)

3. Start recording actions in the Calculator using the Universal Recorder.

   ![](./images/86.png)

4. Perform a series of actions (e.g., simple calculations) and observe the recorder capturing these actions.

   ![](./images/87.png)

5. Pause or stop the recorder once you have completed the actions.

   ![](./images/88.png)

6. Review the captured actions.

   ![](./images/89.png)

### Testing the Recorded Bot

1. Clear the Calculator to its initial state.

   ![](./images/90.png)

2. Run the automation and watch the bot perform the recorded actions.

   ![](./images/91.png)

   ![](./images/92.png)

## Conclusion

You have now learned how to set up triggers and use the recorder feature in Automation Anywhere. These skills are vital for automating tasks based on specific events and for quickly developing bots for repetitive actions. Next, we will explore developing use cases for web automation.
