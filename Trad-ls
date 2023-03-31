import requests
from bs4 import BeautifulSoup
from gtts import gTTS
import os
import playsound

#por informações de login da API 
access_token = ""
app_token = ""

#colocar a url do site no ""
response = requests.get("")


soup = BeautifulSoup(response.content, 'html.parser')


text = soup.get_text()


with open("output.txt", "w") as file:
    file.write(text)
    
with open("output.txt", "r") as file:
    text = file.read() 
data = {
    "action": "translate",
    "text": text,
    "to": "LIBRAS"
       }
response = requests.post("https://vlibras.gov.br/app/api", data=data, headers={
    "Authorization": "Bearer " + access_token,
    "App-Token": app_token
    
response = requests.post("https://vlibras.gov.br/app/api", data=data, headers={
    "Authorization": "Bearer " + access_token,
    "App-Token": app_token
# caso consiga só ouvir file_path = "texto.txt"
'''
file_path = "texto.txt"
with open(file_path, "r") as file:
    text = file.read()
language = 'pt-br'
tts = gTTS(text=text, lang=language)
tts.save("temp.mp3")
playsound.playsound("temp.mp3")
os.remove("temp.mp3")

'''
