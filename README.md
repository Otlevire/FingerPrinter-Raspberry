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

#Links úteis
Biblioteca para OLED 128x64 1.3 SSH1106:

https://luma-oled.readthedocs.io/en/latest/software.html

Comandos de instalação:
* sudo apt-get update
* sudo apt-get install python3 python3-pip python3-pil libjpeg-dev zlib1g-dev libfreetype6-dev liblcms2-dev libopenjp2-7 libtiff5 -y
* sudo -H pip3 install luma.oled

Biblioteca para o Biometrico AS106:

https://circuitdigest.com/microcontroller-projects/raspberry-pi-fingerprint-sensor-interfacing

github com  exemplos de uso: https://github.com/bastianraschke/pyfingerprint/tree/Development

Ver também: https://www.youtube.com/watch?v=-IUae_-LqR4

Comandos de instalação:
* sudo apt-get update
* sudo apt-get install python-fingerprint –yes



Biblioteca para Gerar Planilha no Excel:

Comandos de instalação:
* sudo pip3 install openpyxl

Biblioteca Libreoffice[opcional]:
Comandos de instalação:
* sudo apt install libreoffice
