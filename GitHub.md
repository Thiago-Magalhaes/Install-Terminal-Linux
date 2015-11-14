## GitHub

```
$ apt-get install git-core
#Configure o nome que aparecerá quando você enviar algo para ao servidor
$ git config –global user.name “Your Name Here”
#Recomendo utilizar o mesmo e-mail do cadastro do GitHub
$ git config –global user.email “your_email@youremail.com”
#Insira o comando abaixo e pressione Enter até que ele te peça uma senha
$ ssh-keygen -t rsa -C “your_email@youremail.com”
#Digite a senha para a sua chave e confirme.
$ sudo apt-get install xclip
$ xclip -sel clip < ~/.ssh/id_rsa.pub

Abra a página do GitHub e vá nas configurações de chave ssh.
Clique em “Add ssh key”
Dê um nome para a chave
E no campo “Key” dê Colar(Ctrl+v)
Clique no botão verde escrito “Add Key”

Volte para o terminal
$ ssh -T git@github.com
$ Yes
#Depois disso deve aparecer uma mensagem contendo o seu usuário do GitHub
```