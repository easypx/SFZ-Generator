# SFZ-Generator
Dieses Tool generiert Multisample-SFZ-Dateien mit gleichmäßig verteilten Notennummern über eine Oktave, sowie Velocity-Layern. Die SFZ-Datei ist als Zip downloadbar.
https://easypx.github.io/SFZ-Generator/

SFZ is a plain text file format that stores instrument data for sampled instruments. The SFZ format was developed by René Ceballos (founder of rgcaudio)[1] and continues to be used by companies such as Cakewalk, Plogue and Garritan. SFZ is a royalty-free format and can be used by software developers for both free and commercial purposes. The SFZ Format is widely accepted as an open standard to define the behavior of a musical instrument from a bare set of sound recordings. https://en.wikipedia.org/wiki/SFZ_(file_format)

Ein Multisample erzeugen:
1. Instrument einer DAW samplen (alle gewuenschten Noten als ein Audio File rendern)
2. Normalisieren
3. Slicen der Samples https://github.com/flutydeer/audio-slicer (Treshold nutzen fuer Decay Level)
4. Nachbearbeiten in Audacity (Startpunkt korrigieren)
5. Umbenennen nach Muster in SFZ-Generator
6. SFZ generieren
