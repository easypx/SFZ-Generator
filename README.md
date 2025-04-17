# SFZ-Generator
Dieses Tool generiert Multisample-SFZ-Dateien mit gleichmäßig verteilten Notennummern über mehrere Oktaven. Optional kann ein MIDI-File generiert werden, mit dem man in der DAW die einzelnen Noten rendern kann. Reaper bietet zusaetzlich das Rendern von Regions als einzelne Audio-Files, die als CSV gleich miterzeugt werden koennen. Damit spart man sich das nachtraegliche Schneiden. Alle Dateien sind als Zip downloadbar. Damit laesst sich ein komplexes Instrument in wenigen Augenblicken in ein SFZ-Format umwandeln. SFZ kann in weitere Formate konvertiert werden.
Online: https://easypx.github.io/SFZ-Generator/

SFZ is a plain text file format that stores instrument data for sampled instruments. The SFZ format was developed by René Ceballos (founder of rgcaudio)[1] and continues to be used by companies such as Cakewalk, Plogue and Garritan. SFZ is a royalty-free format and can be used by software developers for both free and commercial purposes. The SFZ Format is widely accepted as an open standard to define the behavior of a musical instrument from a bare set of sound recordings. https://en.wikipedia.org/wiki/SFZ_(file_format)

# Ein Multisample erzeugen: (ohne Region Rendering)
1. Instrument (VST) in einer DAW absamplen (alle Noten aus dem SFZ File als ein Audio File rendern)
2. Normalisieren
3. Slicen der Samples https://github.com/flutydeer/audio-slicer (Treshold nutzen fuer konstanten Decay Level z.B. -96dB)
4. Nachbearbeiten in Audacity (Startpunkt korrigieren) und umbenennen nach Muster in SFZ-Generator
5. SFZ generieren
6. Laden und spielen https://www.zampler.de/

# Nutzung von MIDI und Region Files: (getestet in Reaper 7.19)
1. MIDI-File laden
2. Region-Marker-Liste importieren im Region-Manager:Options/Import Regions/Markers
3. evtl. muessen die Noten gestretcht werden (ALT + Grab rechte Seite des MIDI Items)
4. (Samples optimieren/kuerzen mit https://github.com/flutydeer/audio-slicer)
5. Rendern mit Bounds/All Project Regions und Filename: Piano_$region
6. Laden und spielen https://www.zampler.de/
