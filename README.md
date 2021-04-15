# Android_Car_Tracker
With the increased threat of car theft in the modern era, I decided to repurpose an old Android phone to become a car tracker. Using the 'Tasker' application, I had the ability to program this device to transmit it's current location via an API request. This solution offers a significant price advantage compared to similar methods whereby a constant mobile data (4G) connection is not required. 

#### Demonstration:
<img src="https://user-images.githubusercontent.com/36043248/114793644-b8670280-9d82-11eb-93c7-6d6941683c7c.jpg" width="300">

-------------------------------------------------------------------------------------------------------------------------------

#### Setup Process - Send Location SMS:

1. Install/Buy 'Tasker' from the Google Play Store

![Install Tasker Play Store](https://user-images.githubusercontent.com/36043248/114793688-d9c7ee80-9d82-11eb-9549-cbef810d9226.jpg)

2. Open Tasker application

![Open Tasker Application](https://user-images.githubusercontent.com/36043248/114793729-f19f7280-9d82-11eb-8f6f-d4636efe3005.jpg)

3. Create a profile by clicking on the '➕' button in the bottom right corner and selecting 'Event'

![Create Profile](https://user-images.githubusercontent.com/36043248/114793873-3deab280-9d83-11eb-897f-689d7b24b64c.jpg)

4. Select 'Phone' event

![Select Phone Event](https://user-images.githubusercontent.com/36043248/114794521-8f477180-9d84-11eb-8c8e-224bc5f5832a.jpg)

5. Select 'Received Text' option

![Click Received Text](https://user-images.githubusercontent.com/36043248/114794533-953d5280-9d84-11eb-83c5-cd2ea371a554.jpg)

6. Add your keyword trigger into the 'Content' section. In my case it is '!Location' i.e. when I receive an SMS containing this keyword I will send this phone's current location

![!Location Content](https://user-images.githubusercontent.com/36043248/114794730-efd6ae80-9d84-11eb-8784-f2c33db47504.jpg)

7. Press the back button to return to 'Profiles' page where we will click 'New Task'

![New Task](https://user-images.githubusercontent.com/36043248/114794841-26142e00-9d85-11eb-804d-91213e0f7e06.jpg)

8. Name the new task 'Send Location' as evident in the image below. This can be any phrase of your choice, it is simply a name

!['Send Location' task](https://user-images.githubusercontent.com/36043248/114794906-4cd26480-9d85-11eb-8896-f5d4a3cf46ad.jpg)

9. Click the '➕' button to add an action

![Add Action](https://user-images.githubusercontent.com/36043248/114794947-696e9c80-9d85-11eb-841f-a7ffa2ab7819.jpg)

10. Select 'Location'

![Select Location](https://user-images.githubusercontent.com/36043248/114794982-8014f380-9d85-11eb-89bd-3125009dbb45.jpg)

11. Select 'Get Location v2'

![Select Get Location V2](https://user-images.githubusercontent.com/36043248/114795042-a470d000-9d85-11eb-87ee-72defe29e235.jpg)

12. Press the back button to return to the 'Task Edit' section as per the image below. Now click the '➕' button to add an action

![Back Button Redirected](https://user-images.githubusercontent.com/36043248/114795134-d4b86e80-9d85-11eb-897a-e9a5568d1535.jpg)

13. Select 'Phone' event

![Select Phone](https://user-images.githubusercontent.com/36043248/114795253-0af5ee00-9d86-11eb-9c4f-27122f003830.jpg)

14. Select 'Send SMS'

![Select Send SMS](https://user-images.githubusercontent.com/36043248/114795375-4bee0280-9d86-11eb-9efa-a3bcf8889b6b.jpg)

15. Add the following to the 'Message' section. We will be sending details of the phone's current location and battery percentage

![Add Following](https://user-images.githubusercontent.com/36043248/114795404-5d370f00-9d86-11eb-92da-481cb39a632d.jpg)

16. Press the back button to return to the 'Profiles' section where you can see we have successfully created our first profile

![1st Profile Complete](https://user-images.githubusercontent.com/36043248/114795486-8fe10780-9d86-11eb-8796-86ca9e5ce589.jpg)

#### Setup Process - Send Low Battery SMS:

1. Create a profile by clicking on the '➕' button in the bottom right corner and selecting 'State'

![Select State](https://user-images.githubusercontent.com/36043248/114795528-a71ff500-9d86-11eb-9418-1f8f275e6dc4.jpg)

2. Select 'Power' state

![Select Power](https://user-images.githubusercontent.com/36043248/114795567-c159d300-9d86-11eb-96f8-9fdb42f46cd3.jpg)

3. Select 'Battery Level' option

![Select Battery Level](https://user-images.githubusercontent.com/36043248/114795581-cc146800-9d86-11eb-80aa-7e7dcefc0f17.jpg)

4. Move the value to '10' for both the 'From' and 'To' sliders. This will allow us to automatically send an SMS once the battery perecentage of the phone reaches 10%

![Select 10](https://user-images.githubusercontent.com/36043248/114795696-1a296b80-9d87-11eb-9315-d423797afaa2.jpg)

5. Press the back button to return to 'Profiles' page where we will click 'New Task' and name it 'Low Battery Text'

![Task Creation](https://user-images.githubusercontent.com/36043248/114795757-42b16580-9d87-11eb-982a-8e3874bc27f4.jpg)

6. Click the '➕' button to add an action

![Add Action](https://user-images.githubusercontent.com/36043248/114795807-62488e00-9d87-11eb-9597-658827ef107f.jpg)

7. Select 'Phone' event

![Select Phone Event](https://user-images.githubusercontent.com/36043248/114795851-7f7d5c80-9d87-11eb-8c10-8954c75912d2.jpg)

8. Select 'Send SMS'

![Select Send SMS](https://user-images.githubusercontent.com/36043248/114795375-4bee0280-9d86-11eb-9efa-a3bcf8889b6b.jpg)

9. Add the following to the 'Message' section. We will be sending details of the phone's battery percentage i.e. low battery warning

![Edit Task](https://user-images.githubusercontent.com/36043248/114795940-afc4fb00-9d87-11eb-8064-78d73362e148.jpg)

10. Press the back button to return to the 'Profiles' section where you can see we have successfully created our two profiles

![Two Profiles](https://user-images.githubusercontent.com/36043248/114796039-d97e2200-9d87-11eb-82d6-84fc3a4ce707.jpg)

11. Both these profiles are now active. To demonstrate the first profile we made, we will simply text the keyword '!Location' from our personal phone to this device (one to be used as a Car Tracker equipped with Tasker). This car tracker device will transmit the current location of the vehicle along with the phone's battery level to notify the owner if the device is due to be charged.

![Demonstration](https://user-images.githubusercontent.com/36043248/114796172-2f52ca00-9d88-11eb-9db7-fb13a904ce4a.jpg)

Extras:
- Ensure all battery optimisations are switched of the device, this will prevent any issues with Tasker sending/receiving commands
- Personally, to avoid paying €20-€30 per month retrieving the device's location 24/7 using mobile data, I decided to use Tasker combined with a small credit balancec €5. If in the event I notice my vehicle has been stolen, I can simply send an SMS text to the device which is hardwired into the fusebox (constantly charging) and I receive the details of its current location. This solution is cheaper and provides the same means as the more expensive mobile data enabled option.

Reference: https://thomaschaplin.medium.com/track-your-android-location-remotely-via-sms-using-automation-with-tasker-6cb5e9bfd93d
