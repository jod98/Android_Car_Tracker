# Android_Car_Tracker
With the increased threat of car theft in the modern era, I decided to repurpose an old Android phone to become a car tracker. Using the 'Tasker' application, I had the ability to program this device to transmit it's current location via an API request. This solution offers a significant price advantage compared to similar methods whereby a constant mobile data (4G) connection is not required. 

#### Demonstration:
![Demonstration](https://user-images.githubusercontent.com/36043248/114793644-b8670280-9d82-11eb-93c7-6d6941683c7c.jpg)

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

#### Setup Process - Send Low Battery SMS:

1. 


Extras:
- Ensure all battery optimisations are switched of the device, this will prevent any issues with Tasker sending/receiving commands
- Personally, to avoid paying €20-€30 per month retrieving the device's location 24/7 using mobile data, I decided to use Tasker combined with a small credit balancec €5. If in the event I notice my vehicle has been stolen, I can simply send an SMS text to the device which is hardwired into the fusebox (constantly charging) and I receive the details of its current location. This solution is cheaper and provides the same means as the more expensive mobile data enabled option.

Reference: https://thomaschaplin.medium.com/track-your-android-location-remotely-via-sms-using-automation-with-tasker-6cb5e9bfd93d
