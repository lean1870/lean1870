- 👋 Hi, I’m @lean1870
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
lean1870/lean1870 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
# Funktion zum Erstellen eines Drum-Beats
def create_drum_beat():
    # Schlagzeugklänge (hier kannst du eigene Sounds verwenden)
    kick = AudioSegment.from_file("path/to/kick.wav", format="wav")
    snare = AudioSegment.from_file("path/to/snare.wav", format="wav")
    hi_hat = AudioSegment.from_file("path/to/hi_hat.wav", format="wav")

    # Takte definieren (1 Takt = 4 Schläge)
    beat = kick + snare + hi_hat + hi_hat

    # Wiederholung für eine bestimmte Anzahl von Takten
    full_beat = beat * 4  # Hier 4 Takte als Beispiel

    return full_beat

# Funktion zum Abspielen des Beats
def play_beat(beat):
    beat.export("path/to/beat.wav", format="wav")  # Exportiere den Beat als Audio-Datei
    beat = AudioSegment.from_file("path/to/beat.wav", format="wav")
    beat.export("path/to/beat.mp3", format="mp3")  # Optional: Exportiere den Beat als MP3

    beat.export("path/to/beat.mp3", format="mp3")  # Optional: Exportiere den Beat als MP3

    beat.export("path/to/beat.mp3", format="mp3")  # Optional: Exportiere den Beat als MP3

    # Hier könntest du Code hinzufügen, um den Beat mit einem Musikplayer oder einer DAW abzuspielen

# Beispielaufruf
beat = create_drum_beat()
play_beat(beat)
