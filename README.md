# P2P-Botnet-Architecture 
Developing a encrypted P2P Botnent-Architecture 
# HELP WANTED. IF YOU ARE INTERESTED IN DEVELOPING: EMAIL ME: hacker5preme@protonmail.com
# This is in the making, NOT WORKING !!!
# Starting on 15.06.2021

# Botnet-IDEA:

## Initialisation:
  - Download this repository on your main machine (No bot)
  - Run setup script: (This will be python)
    - Define first BOT(A) (IP-ADRESS), Email adress and Master Password to use for you to give instructions to all bots
    - Upload a config_file containing BOT IP-adress to a webserver (I don't know which on e or like pastebin) over the TOR network
## First BOT (BOT A):
  - Like any other BOT in the botnet, this machine can work as a SERVER and as RECIEVER
  - BOT A listens for new connections (The listening and acting as a server will be coded in python)
## Second / Third / nth BOT:
  - (1) Go to Webserver and download config.txt with password and IP-adresses (This will be done via C)
  - (2) Try to connect to the first BOT on the list via TOR network (This will be done via C)
  - (3.1) If connection succeds: BOT A or what BOT is first in the list and works will update the config file with the new BOT, specify a new password and email the update and the New List of BOTS to an Email adress via another Bot email adress. After all of this was successfull it will delete the connect_script and config file so no traces will be available and the server will only listen for new Connections.
## Use the BOTNET:
As the host you can connect to one of the IP-ADRESSES in the config file (you know the location of ) and you specify a specific password. This password wille be stored as a hash on the clients so it is not reversible. If the Connection was succesfull the BOT transforms to a Command and Control server. It will be a flask server, showing all online bots, their specs, their location and will give a graphical interace to execute commands simultainously on the bots. The instructions to the bots will also be send through the TOR network.


For educational puproses only.;)
