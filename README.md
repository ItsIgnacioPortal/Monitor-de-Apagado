# Monitor-de-Apagado
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FItsIgnacioPortal%2FMonitor-de-Apagado&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Contador+de+visitas&edge_flat=false)](https://hits.seeyoufarm.com)

App para Android que mantiene un registro de cuando se apaga el dispositivo

It's a very simple app that, seconds before the device is about to be turned off, logs the following information into a file:

- Battery level
- Battery temperature
- Time the phone has been charging
- Available RAM

With this information we'll be able to diagnose this issue faster. If the shutting off of the device is handled by the OS when this bug happens, then the app will be notified and it'll be able to generate a report. If the shutdown happens suddenly because of a hardware errorthe app won't be able to generate a report. That information should help us diagnose the issue.


- In the English version ("Shutdown Monitor"), the log is saved in the internal storage in "Shutdown-Monitor/log.txt"
- In the Spanish version ("Monitor de Apagado"), the log is saved in the internal storage in "Monitor-de-Apagado/registro.txt"

When the app is opened it will ask you if you want to enable an alert for when the phone is about to turn off. What that means, is that when  the phone is about to turn off, the app will make a *BEEP* sound. Do note that if notification volume is muted, then you won't hear the sound (obviously). If you want to disable the app you can disable it from its notification. The notification also a button you can press to open the log file.

Some things to keep in mind: This app has a couple of unnecessary notifications. You can hold the notification to open notification settings and disable the unnecessary categories. Just disable the "System notifications" category for this app.


Also, Google Play Protect may complain about this app, since I made it in a whim and it's not actually on any app store. You can safely dismiss this warning. If you're skeptical, here is the VirusTotal scan of the dssnglish apps, and the tasker project source code is available on this GitHub repo.

# Compilar
Esta app fue echa desde tasker.

- `Monitor_de_Apagado.prj.xml` Archivo del proyecto en Español
- `Shutdown_Monitor.prj.xml` Archivo del proyecto en Ingles
