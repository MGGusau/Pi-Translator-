# Pi-Translator-
import sys

try:
  import pyttsx3
 except ImportError:
 sys.exit()
tts = pyttsx3.init() # initialize the TTS engine
print('Text To Talk, by isyakumurtala99@gmail.com')
while True:
    text = input('> ')
    if text.upper() == 'QUIT':
        print('Thanks for playing!')
        sys.exit()
tts.say(text)
tts.runAndWait()
