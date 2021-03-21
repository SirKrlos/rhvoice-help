# rhvoice-help
Uma ajuda de como instalar o RHVoice em algumas distribuições linux.
`Obs: Um trabalho em andamento`

# Como instalar

## Fedora Linux
```bash
$ sudo dnf install git scons

$ cd ~/Downloads
$ git clone https://github.com/RHVoice/RHVoice && cd RHVoice
$ git submodule init
$ git submodule update

$ scons
$ sudo scons install
$ sudo ldconfig
```

# Como testar
```bash
$ spd-say -o rhvoice "Instalação aparentimente ok, parabéns"
```
Certamente irá escutar uma voz natural.

# Como usar no orca
```bash
$ orca -s
```
![image](https://user-images.githubusercontent.com/64156428/111920714-45ae8400-8a6f-11eb-97ef-e63232b17a1d.png)

`Selecione a aba "Voz"`

![image](https://user-images.githubusercontent.com/64156428/111920740-6ecf1480-8a6f-11eb-9c17-a5c9160a3d9e.png)

Altere `Sistema de fala` para `Speech Dispatcher`

Altere `Sintetizador de fala` para `rhvoice`

![image](https://user-images.githubusercontent.com/64156428/111920804-c4a3bc80-8a6f-11eb-914c-98dfbd683c46.png)
