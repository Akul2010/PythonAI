# PythonAI
An opensource AI Assistant for the Raspberry Pi
**By Kevin McAleer**

---

## 1 August Update
I'm returning to this project and will be doing a couple of new videos to improve the capabilities and to tidy up our code as its grown a bit unwieldly!

Here are a couple of things I'll be looking next:
- [x] a conversation history 
- [ ] a conversation API
- [ ] a web interface (finally!)
- [ ] a 'proper' skills framework, using plugin technology

---

Create an API key (its free) at <home.openweathermap.org>


## On Raspberry Pi

Make sure you have pyaudio and espeak installed:

```bash
sudo apt-get install espeak
sudo apt-get install python-audio 
```

## Respeaker (Microphone array Hardware for Raspberry Pi)
Using the respeaker hat from Seeed studios:

```bash
git clone https://github.com/respeaker/seeed-voicecard
cd seeed-voicecard
sudo ./install.sh
sudo reboot
```

If this doesn't work and you get ASLA error messages, try:

*It may probably happen that the driver won't compile with the latest kernel when raspbian rolls out new patches to the kernel. If so, please try sudo ./install.sh --compat-kernel which uses an older kernel but ensures that the driver can work.*
