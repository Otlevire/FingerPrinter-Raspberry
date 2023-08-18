# FingerPrinter-Raspberry

<h1>Steps to Install</h1>
1º Passo: sudo apt update
2º Passo: sudo apt-get full-upgrade
3º Passo: sudo reboot
4º Passo: sudo apt-get install python3-pip
5º Passo: sudo pip3 install --upgrade setuptools

6º Passo(Activar a comunicação i2c): sudo raspi-config
7º Passo(Ver o endereço do display): sudo i2cdetect -y 1
8º Passo(Instalar a library do oled): 
pip3 install adafruit-circuitpython-ssd1306
sudo apt-get install python3-pil

9º Passo(Baixar o script OLED):   git clone https://github.com/mklements/OLED_Stats.git
10º Passo(Abrir a pasta e rodar): python3 stats.py

11º Passo(Colocando o código correndo automaticamente no startup):
No terminal: crontab -e
Adicionar a seguinte linha no final do arquivo: 
@reboot python3 /home/'user_name'/program_name.py &



<!-- pip install adafruit-circuitpython-ili9341 -->