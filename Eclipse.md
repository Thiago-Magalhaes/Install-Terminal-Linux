## [Eclipse] (http://www.eclipse.org/downloads/packages/eclipse-ide-java-ee-developers/junosr1)

```
Após baixar o pacote desejado, descompacte ele na pasta que ele está
tar xzf eclipse-jee-juno-SR1-linux-gtk-x86_64.tar.gz

Após descompactar, mova a pasta descompactada para o diretório /opt da seguinte forma:
sudo mv eclipse /opt/eclipse

dê as permissões corretas para os arquivos criados anteriormente:
sudo chmod -R +r /opt/eclipse
sudo chmod +x /opt/eclipse/eclipse

coloque o caminho para o executável disponível no terminal:
sudo touch /usr/bin/eclipse
sudo chmod 755 /usr/bin/eclipse
sudo gedit /usr/bin/eclipse

No Gedit, cole o seguinte conteúdo dentro do arquivo eclipse:

#!/bin/sh
export UBUNTU_MENUPROXY=0
export ECLIPSE_HOME="/opt/eclipse"
$ECLIPSE_HOME/eclipse $*

Feche o Gedit e crie um link para que o Eclipse seja possível de ser aberto de todos os locais:
sudo ln -s /usr/bin/eclipse /bin/eclipse

Agora crie o arquivo de definição do atalho para o Dash:
sudo gedit /usr/share/applications/eclipse.desktop

No Gedit, cole o seguinte conteúdo:
[Desktop Entry]
Encoding=UTF-8
Name=Eclipse
Comment=Eclipse IDE
Exec=eclipse
Icon=/opt/eclipse/icon.xpm
Terminal=false
Type=Application
Categories=GNOME;Application;Development;
StartupNotify=true

Salve e feche o Gedit.

Para executá-lo pela primeira vez, é preciso abrí-lo com a opção -clean:
eclipse -clean
```