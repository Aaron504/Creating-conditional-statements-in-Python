# Creating conditional statements in Python




<h2>Description</h2>
In this lab, I will open a notebook environment to practice writing conditional statements in Python. I'll be presented with a security scenario to explore throughout the lab. I'll practice applying conditional statements to automate processes across an organization.

What I'll do
I'll have multiple tasks in this lab:

Write code that determines if a user’s operating system requires an update

Write code that determines if login attempts were made by approved users and if login attempts occurred during organization hours
<br />


<h2>Languages and Utilities Used</h2>

- <b>Python</b> 
  

<h2>Environments Used </h2>

- <b>Jupyter</b> 

<h2>Lab Walkthrough</h2>

<p align="center">
You are asked to help automate the process of checking whether a user's operating system requires an update. Imagine that a user's device can be running one of the following operating systems: OS 1, OS 2, or OS 3. While OS 2 is up-to-date, OS 1 and OS 3 are not. Your task is to check whether the user's system is up-to-date, and if it is, display a message accordingly. To do this, complete the conditional statement using the keyword if.  <br/>

  ![Screenshot 2023-08-06 202216](https://github.com/Aaron504/Creating-conditional-statements-in-Python/assets/141078110/0b053244-752a-4564-b336-79992ceefbf6)

<br />
<br />
Nothing is displayed when the system is not equal to "OS 2". This is because the condition didn't evaluate to True.

It would be beneficial if an alternative message is provided to them when updates are needed.

In the following cell, add the appropriate keyword after the first conditional so that it will display a message that conveys that an update is needed when the system is not running OS 2. 

Then, set the value of the system variable to indicate that OS 2 is running and run the cell. After observing what happens, set the value of system to indicate either that OS 1 is running or that OS 3 is running and run the cell.  <br/>
![Screenshot 2023-08-06 205518](https://github.com/Aaron504/Creating-conditional-statements-in-Python/assets/141078110/c1a0c104-b40a-4cd2-8647-15df926cba64)

<br />
<br />
Now I'll move on to the next part of my work. You've been asked to investigate login attempts to a specific device. Only approved users should log on to this device.

I'll start with two authorized users, stored in the variables approved_user1 and approved_user2. I'll need to write a conditional statement that compares those variables to a third variable, username. This will be the username of a specific user trying to log in. <br/>
![Screenshot 2023-08-06 205915](https://github.com/Aaron504/Creating-conditional-statements-in-Python/assets/141078110/45945111-6fd4-47bf-b5c4-8ef7a57f1276)

<br />
<br />
The number of approved users has now expanded to five. Rather than storing each of the approved users' usernames individually, it would be more concise to store them in an allow list called approved_list.

The in operator in Python can be used to determine whether a given value is an element of a sequence. Using the in operator in a condition can help you check whether a specific username is part of a list of approved usernames. For example, in the code below, username in approved_list evaluates to True if the value of the username variable is included in approved_list.

Complete the code in the following cell to display the same messages that you used in the previous step. When the condition evaluates to True, the following message will be displayed: "This user has access to this device." When it evaluates to False, the following message will be displayed: "This user does not have access to this device." Then, run the cell to observe its behavior. Afterwards, reassign the username variable to a username that is not approved and run the cell to observe what happens. <br/>
![Screenshot 2023-08-06 210246](https://github.com/Aaron504/Creating-conditional-statements-in-Python/assets/141078110/6d0bac4c-a59e-4514-bf6c-6ea58221899e)

<br />
<br />
 Now I'll write another conditional statement. This one will use a organization_hours variable to check if the user logged in during specific organization hours. When that condition is met, the code should display the string "Login attempt made during organization hours.". When that condition isn't met, the code should display the string "Login attempt made outside of organization hours.".

The organization_hours variable will have a Boolean data type. If organization_hours has a Boolean value of True, that means the user is logged in during the specified organization hours. If organization_hours has a Boolean value of False, that means the user is not logged in during those hours. <br/>
![Screenshot 2023-08-06 210640](https://github.com/Aaron504/Creating-conditional-statements-in-Python/assets/141078110/4542cb3a-150b-4cb7-9597-9ecffe30f342)

