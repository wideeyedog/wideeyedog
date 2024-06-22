- 👋 Hi, I’m @wideeyedog
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
[Uploading server.cfg…](#--------------------------------#
# https://discord.gg/E3wheBM5fZ ---#
#--------------------------------#
sv_enforceGameBuild 3095
# Only change the IP if you're using a server with multiple network interfaces, otherwise change the port only.
endpoint_add_tcp "217.182.71.133"
endpoint_add_udp "217.182.71.133"

sv_hostname "West tuning _RP"
sets Optimisation "Notre serveur dispose d un Développement Unique et OPTIMISER. ( 64 Joueurs ) 🌙"
set steam_webApiKey 18941DFB6CA33C4FC8FDB72D0CD0BD62
sv_licenseKey "cfxk_PcKmaluEG0Jn5yieILMj_bXrh3" 
load_server_icon esxLogo.png
sv_maxclients 64

sets sv_projectName "West tuning_RP FA"
sets sv_projectDesc "➔ BASE US"
sets locale "fr"
sets tags "fr, esx, rp, baseus, baylife, unity, revolution, nopaytowin ,drugs, drug"
sv_scriptHookAllowed 0


sets banner_detail ""
sets banner_connecting ""
sets 👕 "Vêtements moddées"
sets 🚗 "Vehicules Imports"
sets 🌎 "https://discord.gg/6ZVbxyUfUy"
sets activitypubFeed "jeromelambot@mas.to"
sets Fondateur "Jérome"


setr ox:locale "fr"
setr inventory:slots 50
setr inventory:weight 30000
setr inventory:target false
setr inventory:keys ["TAB", "K", "F2"]
set inventory:vehicleloot [["cola", 1, 1],["water", 1, 1],["garbage", 1, 2, 50],["money", 1, 50],["money", 200, 400, 5],["bandage", 1, 1]]
set inventory:dumpsterloot [["mustard", 1, 1],["garbage", 1, 3],["money", 1, 10],["burger", 1, 1]]


## [txAdmin CFG validator]: onesync MUST only be set in the txAdmin settings page.
# set onesync on
## [txAdmin CFG validator]: onesync MUST only be set in the txAdmin settings page.
# set onesync on
set mysql_connection_string "server=185.200.246.238;database=s9032_lossantos;userid=u9032_iWYKQNhjc8;password=Cxq1s@RaNzR2hI1!RSG!HMrD"




stop esx_skin
stop esx_multicharacter


setr ox:locale "fr"
setr inventory:slots 50
setr inventory:weight 30000
setr inventory:target false
setr inventory:keys ["TAB", "K", "F2"]
set inventory:vehicleloot [["cola", 1, 1],["water", 1, 1],["garbage", 1, 2, 50],["money", 1, 50],["money", 200, 400, 5],["bandage", 1, 1]]
set inventory:dumpsterloot [["mustard", 1, 1],["garbage", 1, 3],["money", 1, 10],["burger", 1, 1]]

setr fivem-appearance:customization 1
setr fivem-appearance:locale "fr"
ensure fivem-appearance

######################################################################################################################################################

# System Administrators
# ---------------------
# Add system admins

add_principal group.admin group.user
add_ace group.admin command allow # allow all commands
add_ace group.admin command.quit deny # but don't allow quit
add_ace resource.es_extended command.add_ace allow
add_ace resource.es_extended command.add_principal allow
add_ace resource.es_extended command.remove_principal allow
add_ace resource.es_extended command.stop allow
add_ace group.superadmin Misc allow
add_ace group.superadmin AdminMenu allow


#SUPERADMINS 
add_principal identifier.fivem:9044829 group.superadmin
add_principal identifier.fivem:13989220 group.superadmin
add_principal identifier.fivem:12473704 group.superadmin
add_principal identifier.fivem:8529504 group.superadmin
add_principal identifier.fivem:4924939 group.superadminfivem:11498753

#ADMINS
add_principal identifier.steam:110000109b1b334 group.admin

#MODERATORS
add_principal identifier.fivem:11304765 group.mod

# dont have to change this below unless you want to
#PERMISSIONS GIVEN TO SUPER ADMINS
add_ace group.superadmin AdminMenu allow
add_ace group.superadmin Client allow
add_ace group.superadmin Weapon allow
add_ace group.superadmin Vehicle allow
add_ace group.superadmin Blacklist allow
add_ace group.superadmin Misc allow

#PERMISSIONS GIVEN TO ADMINS
add_ace group.admin BypassSpectate allow
add_ace group.admin BypassVPN allow
add_ace group.admin AdminMenu allow
add_ace group.admin BlipsBypass allow
add_ace group.admin Client allow
add_ace group.admin Misc allow
add_ace group.admin Vehicle allow
#PERMISSIONS GIVEN TO MODERATORS
add_ace group.mod BypassSpectate allow
add_ace group.mod BypassVPN allow
add_ace group.mod BlipsBypass allow
add_ace group.mod Client allow
add_ace group.mod Misc allow
# Les lignes ci-dessous permettent de protéger un peu plus votre serveur notamment contre les attaques en Layer 7 (cela désactive info.json / player.json...)
set sv_requestParanoia 3
sv_endpointprivacy true
sv_authMinTrust 4



#################################################################################################################################################################

# pma-voice Config
# ----------------
setr voice_enableRadioAnim 1
setr voice_useNativeAudio true
setr voice_useSendingRangeOnly true

#################################################################################################################################################################

### PMMS

exec @pmms/permissions.cfg
ensure  pmms
add_ace builtin.everyone pmms.interact allow
add_ace builtin.everyone pmms.anyEntity allow
add_ace builtin.everyone pmms.customUrl allow
add_ace builtin.everyone pmms.anyUrl allow
add_ace builtin.everyone command.pmms allow
add_ace group.superadmin Misc allow
add_ace group.superadmin AdminMenu allow

####################################################################################################################################################################

# ESX Language (edit to change the language of ESX)
# -----------------------------------------------------------
setr esx:locale "fr"

###################################################################################################################################################################

# Default & Standalone Resources
# ------------------------------
ensure chat
ensure spawnmanager
ensure hardcap
ensure oxmysql
ensure bob74_ipl
ensure anticheat
# ESX Legacy Core
# ----------
ensure [core]

# ESX Addons
# ----------
ensure [admin]
ensure [Blips]
ensure [libs]
ensure [core]
ensure [esx_addons]
ensure [voiture]

ensure corevoiture
ensure core-mapping
ensure [illegal]
# Scripts
ensure [scripts]
ensure [phone]
ensure [jobs]
ensure [vetement]
ensure [standalone]
# Additional Resource
# -------------------
ensure pma-voice
ensure [mapping]
add_ace resource.nova_adminmenu command allow)

<!---
wideeyedog/wideeyedog is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
