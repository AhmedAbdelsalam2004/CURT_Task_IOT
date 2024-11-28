# CURT TASK

### ***ESP32***

[Blinking LED](https://wokwi.com/projects/415787678070030337)

[Analog sensor](https://wokwi.com/projects/415789802821657601)

[Temperature sensor](https://wokwi.com/projects/415795486802385921)

### ***IOT Lecture***

[Full material for IOT by Eng.Abdallah El Ghamry](https://drive.google.com/drive/folders/1cBNP12njPfeEj3vqmLPByq5MJX7pzeyJ)

* **Publisher** => **Broker**(وسيط) => **Subscribers**
* **MQTT**(Message Queuing Telemetry Transport) is a message protocol between IOT devices:
  * Easy implementation
  * Lightweight with minimal packet overheard
  * Publish/Subscribe protocol
  * Bidirectional
  * Highly secure (easy to encrypt messages)
  * Highly scalable(Only Broker's IP address and name)
  * Reliability
* The broker sends the **topic** to the subscriber based on the topic they are subscribed to
* The Publisher can be a subscriber and vice versa
* The topic may have several subtopics. (Ex: Kitchen/Fridge) the main topic is Kitchen and subtopic is fridge
* The use of **ACLs**(Access Control lists) allows restrictions of subscriptions and publishing of clients
* The standard unsecure Port is *1883* while the for secured MQTT broker port is 8883
* Quality Of Service(Qos):
  * Level 0(Fire and Forget): The message will be sent at most once or none
  * Level 1: The message will be sent at least once or more
  * level 2: The message will be sent exactly once (it sends the packet again with a duplicate flag)
