## FileZilla

```
Baixe a versão atualizada
http://sourceforge.net/projects/filezilla/

Use o comando a seguir para descompactar o arquivo baixado
sudo tar -xjvf filezilla.tar.bz2 -C /opt/

Renomeie a pasta criada. Se ao executar o comando abaixo ocorrer um erro com a mensagem iniciando com “mv: é impossível sobrescrever o não-diretório”, pule este passo
sudo mv /opt/FileZilla*/ /opt/filezilla

Finalmente, crie um atalho para facilitar a execução do programa;
sudo ln -sf /opt/filezilla/bin/filezilla /usr/bin/filezilla

Se seu ambiente gráfico atual suportar, crie um lançador para o programa, executando um editor de texto com o comando (se for preciso, use outro editor de textos e substitua “gedit” por ele)
sudo gedit /usr/share/applications/filezilla.desktop

Copie o conteúdo abaixo e cole ele no arquivo aberto. Em seguida, salve e feche o arquivo;

[Desktop Entry]
Version=1.0
Type=Application
Terminal=false
Name=filezilla
Exec=/opt/filezilla/bin/filezilla
Icon=/opt/filezilla/share/icons/hicolor/48x48/apps/filezilla.png
Categories=Application;

```