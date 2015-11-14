## phpMyAdmin

```
sudo apt-get install phpmyadmin

Durante a instalação o uma tela surgirá pedindo para que você informe qual servidor será utilizado para rodar o phpmyadmin, deixe marcada a opção apache2.

Ao final da instalação feche o terminal e acesse o navegador, para testar digite na barra de endereços http://localhost/phpmyadmin, basta digitar a senha informada durante a instalação e você terá acesso normalmente.

Caso você tenha problemas para abrir o phpMyAdmin, e apresente a seguinte mensagem:

The requested URL /phpmyadmin/ was not found on this server.

Basta copiar o diretório /phpmyadmin que se encontra dentro do caminho /usr/share/ para dentro do caminho /var/www .
```