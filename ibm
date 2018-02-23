import requests 
import json 
import sys 
import subprocess 

# IBM bluemix API url 
url = 'https://stream.watsonplatform.net/speech-to-text/api/v1/recognize?speaker_labels=true'
# bluemix authentication username 
username = 'username dado pelo ibm'

# bluemix authentication password 
password = 'pass dada pelo ibm'

headers={'Content-Type': 'audio/wav'}

# Open audio file(.wav) in wave format 
audio = open('C:/Users/franc/Downloads/work1.wav', 'rb')

r = requests.post(url, data=audio, headers=headers, auth=(username, password))
print(r.content)
# create the json file out of 
with open('C:/Users/franc/Downloads/sample.json', 'w') as f:
 sys.stdout = f
 print(r.text)
