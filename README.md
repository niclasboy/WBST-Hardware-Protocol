<h1>Aufbau des Protokolls</h1>

Alle Daten werden mittels COBS En-/Decodiert. Es wird eine Datenübertragung von 250k 8N2 verwendet.

|   16bit   |   16bit   |   ......... <br/>
  Datentyp      Länge       Nutzdaten
  
  Datentyp: 
  
  0x0101      Return Serial Number (128bits) <br/>
  0x0102      Return Typ (64bits) <br/>
  0xFF01      Sent Data <br/>
  0xFF02      Get Data -> Nutzdaten (32 bit (Angefragtes Feld) | 32 bit (ID)) <br/>
 
