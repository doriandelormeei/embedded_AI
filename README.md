# embedded_AI
Pour utiliser une board speech

--------------------------------------
L'utilisation de Ollama + TinyLlama peut-être utile, il suffit de 1G 
Utilisation de Eleven Lab pour effectuer le choix de la voix du Text-to-speech

--------------------------------------
La library whisper_mic permet d'analyser la voix et de faire une captation des mots plus ou moins fiable en fonction du "--model" utilisé 

from whisper_mic import WhisperMic

print("start")           
mic = WhisperMic()                                            # lancement du programme d'écoute audio
result = mic.listen()
if "doberman" in result or "dobermann" in result:             # phase de test
    print("le mot est là \n")
print(result)                                                 # transcription du vocal en mots
print("fin")

-------------------------------------
