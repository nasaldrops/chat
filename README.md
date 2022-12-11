# chat
This app works using Whatsapp and Twilio.

I followed this tutorial to set up the bulk of the code: 

https://www.twilio.com/blog/python-whatsapp-chef-bot-openai-gpt3

# This is important - Ngrok
You will need to register for ngrok's **free tier account** otherwise it will not work for you. It will also reset every 8 hours or so making this a temporary solution.

Create a file, call it .env and add this to it:
    
    OPENAI_API_KEY = lkldjflgkjdfLKJLKHLKHIH7889879h

    Don't put quotes or anything around it.
    
    Be sure not to expose your API.  

# Running on a RaspberryPi

These instrucitons on how to iunstall Ngrok on RPi were very useful:
https://medium.com/@gaelollivier/connect-to-your-raspberry-pi-from-anywhere-using-ngrok-801e9fd1dd46

Once installed, be sure to authenticate with Ngrok and include ./ngrok in the terminal and not ngrok, at least that was what worked for me.

Use ./ngrok http 5000 inside the RPi terminal to start your ngrok port forwarder. Take the https url and add it to the Twilio/Whatsapp HTTP Post section, along with folder name.


