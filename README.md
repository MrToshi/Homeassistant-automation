# Homeassistant-automation

Batterien Lade-Synchronisation.yaml

Daly Smart BMS 

![image](https://github.com/user-attachments/assets/a977fbd6-a74a-4e07-9fd7-49ca457f1359)

Vorher 
![image](https://github.com/user-attachments/assets/2cf48ad1-1fea-48f8-8cfb-795175769816)

Nachher 

![image](https://github.com/user-attachments/assets/54f8b4e9-2ffd-4b83-8c5a-4a9ed66796fd)


Diese Home Assistant Automation synchronisiert zwei Batterien während des Ladevorgangs, indem sie die schwächere Batterie bevorzugt lädt, wenn ein signifikanter Unterschied im Ladezustand (SOC) besteht. 
Sobald beide Batterien einen ähnlichen Ladezustand erreicht haben, werden sie gleichzeitig geladen.

Funktionsweise
Die Automation überprüft alle 5 Minuten den Ladezustand beider Batterien und entscheidet basierend auf der SOC-Differenz, welche Batterie(n) geladen werden sollen:

Wenn eine Batterie mehr als 2% mehr SOC hat als die andere, wird nur die schwächere Batterie geladen

Wenn der Unterschied 2% oder weniger beträgt, werden beide Batterien gleichzeitig geladen

Dies führt zu einer gleichmäßigen Nutzung beider Batterien und verhindert, dass eine Batterie stärker beansprucht wird als die andere.
