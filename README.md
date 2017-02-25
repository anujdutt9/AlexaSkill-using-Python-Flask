# AlexaSkill-using-Python-Flask
*This repository contains Python Jupyter Notebook for Alexa Skill using Python 3 and Flask.*

#Requirements
1.**flask**

Use:
```
pip install flask
```

2.**flask-ask**

Use:
```
pip install flask-ask
```

3.**json**

Use:
```
pip install json
```

4.**unidecode**

Use:
```
pip install unidecode
```
5.**ngrok**
Download it from: [https://ngrok.com/] (https://ngrok.com/)


#Using the Skill
1. Extract ngrok to the same folder where you have your python code.
2. Using command prompt (Windows), go to the folder containing the code and run the following command:
```
ngrok http 5000
```
3.Step 2 provides you with an Https address in your command prompt. We will use this address in AWS Console.

4.Go to developer.amazon.com and log in to same account as on Alexa. 

5.Click on Alexa tab and Alexa Skills Kit.

6.Enter a valid name for the app and invocation name.

7.Under Intent Schema enter the following:
```
{ 
	"intents": [{ 
		"intent": "YesIntent" 
	}, 
	{ 
		"intent": "NoIntent" 
	}]
} 
```

8.Under Sample Utterence, enter sample text that you may say to trigger intents. Ex:
```
YesIntent yes
YesIntent sure

NoIntent no
NoIntent go away
```

9.In Endpoint, we are using Https, select North America.

10.Type in the Https URL obtained from the Command Prompt.

11.In Certificates, select the second one.

12.Click Next and start talking to your Alexa device.
