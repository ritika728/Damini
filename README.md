# DAMINI- Together We Can

Damini uses cutting-edge technology and simulation to tackle the most grave issue facing human civilization to date. The most crucial aspects of the app include Emergency SOS service,  Siren alert, Hidden camera detector (either manually or through a simulation of an electromagnetic field invented by us), tips on manually detecting spy cameras at different locations like changing room, bathroom, bedroom or outdoors,  news about women's struggles and empowerment, contact information to reach out keeping the data private, and a method to empower others through messaging and getting in touch. In summary, this app addresses both preventive and post-event actions for sexual harassment.


       
## Description
It is a complete women's safety app that requires a woman to save the phone numbers of maximum four of her family members/friends/guardian. Whenever she is in trouble, she can tap the power button three times, which will send an emergency message to her family members with a live update of her location. It will also make a phone call to her first relative even if the phone is locked, eliminating the need to unlock the device and launch the app. She can press the power button three more times to activate the siren warning if she gets into more difficulty and needs to find the offender. The fetures are noted down :

## Features

- Allows to Save the phone numbers of your close relatives/friends/guardian as the emergency contacts.
- By just pressing the power button three times, you may send messages with live locations and make phone calls. Both these tasks are performed simultaneoulsy to avoid any delay.  
- You can even start a siren alarm to distract the offender and stop it by pressing the power button three times in quick succession.
- Scan the suspicious areas to find any hidden spy cameras. 
- Learn how to manually detect spy cameras.
- Read articles on the struggles of women to get empowerment. 
- Contacting Us Feature to reach out in case of any issue
- Empowering sharing feature

## Brief Process Flow 

- A splash screen integrated with the lottie animations is shown when we tap the launcher icon.
- The programme will then ask for some permissions before displaying the home screen with its seven CardView Buttons.
- Emergency SOS, Hidden Camera Detector, Women's News, Siren Alarm, App Tour, About Us, Share, and save lives are among the seven card view buttons.
- After entering in the application:

1. When using the emergency SOS service, shared preferences are used to save the phone numbers of family members as a key value pair. When we tap the "Try It" button, implicit intent is used to make a phone call, and the SMS Manager class is used to send a message, which includes the user's current location as provided by the fusedlocationprovider client API.

- As this capability must be activated even while the phone is locked, we must do so now. Therefore, we are unable to execute any background actions when the phone is locked because the programme is in a paused state. In order for some functionality to be done even while the phone is locked, a background service is registered inside the app.
- In order to receive the broadcast message from the OS about the screen's ON/OFF state and track the number of times the power button has been pressed, a broadcast receiver has now been registered inside the background service.
Additionally, when we press the power button for the first time, a timer is also started. If we press the power button three more times, the try-it functionality is activated. If we press the power button six times in the space of 30 seconds, a siren alarm is activated to alert the culprit, and if we press the power button three more times, the alarm is silenced.

2. Hidden camera detector Feture. We must be aware that all electronic cameras emit electromagnetic radiations. The magnetometer sensor on our phone detects these electromagnetic radiations' strengths in all three directions, and if the result is greater than a predetermined range, the phone will begin to beep.

3. Women's News displays a screen with solely women's news, which is filled with data from a news api that was acquired with the aid of the retrofit library.

4. Siren Alert Next, with the aid of the media player API, this screen activates a siren alarm in a loop.

5. Contact Us to enable the user to learn more about us and to get in touch with us using implicit intents.

6. App tour to get a comprehensive look at the app and gain a thorough understanding of it.

7. Spread a message of empowerment so that people will spread it and save lives.

## Technologies, Libraries and Components Used
Technologies and Libraries used:
- Java 
- XML
- Sensor Manager API
- Implicit intents for sms,call and email
- Background Service 
- Broadcast Receiver
- Magnetometer Sensor
- SMS Manager API
- Retrofit Library
- Media player api 
- Shared Preferences for storing local data
- News Api 
- FusedLocationProviderClient API for efficient user location retrieval
- Airbnb’s Lottie animations 


Android Components which are used:
- ProgressBar 
- MenuBar
- RecyclerView
- ConstraintLayout 
- LinearLayout 
- TextView, Button, EditText, ImageView, 
- CardView 
- Material text fields ( TextInputEditText ) 
- Explicit and implicit intents 
- Intent filters 
- Object Animator
- FrameLayout 
- GridLayout 
- FloatingActionButton 
- RelativeLayout , 
- NestedScrollView 
- SpeedometerView
- ScrollView 
- LottieAnimationView



## Authors

- [@ritika728](https://github.com/ritika728)

