Anteriomente para fazer o acesso entre a sua maquina e repositorio
era necessário email e senha para finalizar essa comunicação.
Com a Chave SSH não há mais a necessidade de fazer esse procedimento.
Primeiro vc tem que ir no settings da sua conta no github e ir em chave SSH e GbG keys.
Loga após isso vc tem ir na sua maquina e fazer o seguinte procedimento: 

ssh-keygen -t ed25519 -C "email"
Resultado:
Generating public/private ed25519 key pair.
Enter file in which to save the key (/home/alexandre/.ssh/id_ed25519):

sao geradas duas chaves um publica e outra privada

Agora é necessario dar um cd no endereço onde foi armazeando as chaves privadas e publicas 
"	cd/home/alexandre/.ssh/id_ed25519"
Dado um ls vai haver dois arquivos 
"id_ed25519  id_ed25519.pub"

Dando um cat na chave publica temos 
 	cat ed_25519.pub

O resultado do cat da chave publica cola-se no github para configura a chave ssh
