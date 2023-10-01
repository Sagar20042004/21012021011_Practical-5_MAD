# 21012021011_Practical-5_MAD
PR5

Intent introduction : 

An Intent is a messaging object you can use to request an action from another app component. Although intents facilitate communication between components in several ways, there are three fundamental use cases:

**Starting an activity : **

An Activity represents a single screen in an app. You can start a new instance of an Activity by passing an Intent to startActivity(). The Intent describes the activity to start and carries any necessary data.

If you want to receive a result from the activity when it finishes, call startActivityForResult(). Your activity receives the result as a separate Intent object in your activity's onActivityResult() callback. For more information, see the Activities guide.

**Starting a service :** 

A Service is a component that performs operations in the background without a user interface. With Android 5.0 (API level 21) and later, you can start a service with JobScheduler. For more information about JobScheduler, see its API-reference documentation.

For versions earlier than Android 5.0 (API level 21), you can start a service by using methods of the Service class. You can start a service to perform a one-time operation (such as downloading a file) by passing an Intent to startService(). The Intent describes the service to start and carries any necessary data.

If the service is designed with a client-server interface, you can bind to the service from another component by passing an Intent to bindService(). For more information, see the Services guide.

**Delivering a broadcast** : 

A broadcast is a message that any app can receive. The system delivers various broadcasts for system events, such as when the system boots up or the device starts charging. You can deliver a broadcast to other apps by passing an Intent to sendBroadcast() or sendOrderedBroadcast().

The rest of this page explains how intents work and how to use them. For related information, see Interacting with Other Apps and Sharing Content.

Intent types
**There are two types of intents:**

Explicit intents specify which application will satisfy the intent, by supplying either the target app's package name or a fully-qualified component class name. You'll typically use an explicit intent to start a component in your own app, because you know the class name of the activity or service you want to start. For example, you might start a new activity within your app in response to a user action, or start a service to download a file in the background.

Implicit intents do not name a specific component, but instead declare a general action to perform, which allows a component from another app to handle it. For example, if you want to show the user a location on a map, you can use an implicit intent to request that another capable app show a specified location on a map.


**Intent Action** : An intent lets you start an activity in another app by describing an action you'd like to perform, such as "view a map" or "take a picture," in an Intent object.

Some examples of intent actions :

ACTION_ALL_APPS

List all the applications available on the device.

2	
ACTION_ANSWER

Handle an incoming phone call.

3	
ACTION_ATTACH_DATA

Used to indicate that some piece of data should be attached to some other place

4	
ACTION_BATTERY_CHANGED

This is a sticky broadcast containing the charging state, level, and other information about the battery.

5	
ACTION_BATTERY_LOW

This broadcast corresponds to the "Low battery warning" system dialog.

6	
ACTION_BATTERY_OKAY

This will be sent after ACTION_BATTERY_LOW once the battery has gone back up to an okay state.

7	
ACTION_BOOT_COMPLETED

This is broadcast once, after the system has finished booting.

8	
ACTION_BUG_REPORT

Show activity for reporting a bug.

9	
ACTION_CALL

Perform a call to someone specified by the data.

10	
ACTION_CALL_BUTTON

The user pressed the "call" button to go to the dialer or other appropriate UI for placing a call.

ETC....

**AIM**: What is Intent? Write down types of Intent and types of Intent Action. Create an
application which demonstrates implicit Intent for following features.
1.	Make call to specific number			4. Open Gallery
2. Open specific URL				5. Set Alarm
3. Open Call Log					6. Open Camera

![image](https://github.com/Sagar20042004/21012021011_Practical-5_MAD/assets/98373145/d61ed4b5-6ddc-4d34-9272-b2a95c81985a)

![image](https://github.com/Sagar20042004/21012021011_Practical-5_MAD/assets/98373145/e8c1d162-a6be-4b79-865b-6a51413b06ed)

![image](https://github.com/Sagar20042004/21012021011_Practical-5_MAD/assets/98373145/bf6a42ce-6236-4bf7-98df-8eb408cb370e)

![image](https://github.com/Sagar20042004/21012021011_Practical-5_MAD/assets/98373145/9ce11a21-006c-4a2a-9e24-15c6a163a1bc)

![image](https://github.com/Sagar20042004/21012021011_Practical-5_MAD/assets/98373145/3f4108fa-ef82-4754-8fd6-afa132f223c2)

![image](https://github.com/Sagar20042004/21012021011_Practical-5_MAD/assets/98373145/aa246338-674a-40eb-9158-bda9a42467c5)

![image](https://github.com/Sagar20042004/21012021011_Practical-5_MAD/assets/98373145/86bb86e2-0629-4544-8529-53ff37244e28)

![image](https://github.com/Sagar20042004/21012021011_Practical-5_MAD/assets/98373145/151d8bb5-d798-4a8d-9630-22c068fe4181)
