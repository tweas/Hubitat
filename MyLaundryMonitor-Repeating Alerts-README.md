# HubitatPublic
MyLaundryMonitor-Repeating Alerts
      Uses a switch to set up repeating alerts using the runEveryXMinutes or Hours schedule.

Section ("Turn Off These Switches At Start.") 
   The main intent of these switches is to turn off the switches controlling the repeating alerts from a prior instance of this app, or another instance of this app
   For instance, using a virtual switch called Washer Done and having it turned off here by a separate instance that monitors the dryer.
   I also have it set to turn off the light in the washroom (cause my kids never do)
   
"When this device stops drawing power (Washer or Dryer Meter Settings)" 
    This is the power meter you are monitoring for your washer or dryer)
    
   "Start cycle when power consumption goes above (W)"
        This the value that starts the monitoring of the cycle.  I use 30 for my dryer and 10 for my washer
    "Stop cycle when power consumption drops below (W) ..."
        This is the value that triggers the "I'm Done" alert.  Take care to make it low enough that you do not get false positives, but realize your washer will not be zero
        unless unplugged.
    "... for at least this long (min)"
        Most washers have an idle state that lasts a few minutes.  This setting minimizes false alerts due to those pauses.
    
  "Send This Message"
    "Notification message"
        The text of the message you want to send.
  
  
  "Using These Notification Methods"
    "Send a device notification?"
      Click this if you want to send a phone device notification
    "Notification device" (Can be left blank)
      Select the devices you want to send the phone notification to
    "Speak Via: (Speech Synthesis)"
      Speech Synth devices (can be left blank)
    "Speak Via: (Music Player -> TTS)"
      Music Player Devices (can be left blank)
   
   "For Repeating Messages, turn on this switch (MUST BE TURNED OFF MANUALLY IF NOT TURNED OFF AT BEGINNING OF THIS PROGRAM)"
        "Turn on this switch when done(Primary - WILL REPEAT ALERTS IF THIS SWITCH IS SELECTED)"
            HEED THE WARNING - IF YOU DO NOT TURN THIS SWITCH OFF, THE MESSAGES WILL BE REPEATED INDEFINITELY AT THE SELECTED INTERVAL
            You can have this switch automatically turn off at the beginning, or use the app.  But if you select a switch, it WILL repeat.
  "How Often To Be Reminded (CHOICES ARE 1, 5, 10, 15, 30, 60, or 180 - ANYTHING ELSE WILL ERROR)"
            THIS IS REQUIRED IF YOU SELECT A SWITCH ABOVE.  ALSO YOU CAN ONLY USE THE LISTED VALUES.  NOT DOING SO WILL ERROR OUT AND YOU WILL GET NO MESSAGES
  
  "Turn On These Additional Switches (Can be lights)"
        If you have other switches or lights you would like to switch on, you can add them here.  (Turning on the laundry light is a nice visible reminder if you do not want
          phone or audio messages)
