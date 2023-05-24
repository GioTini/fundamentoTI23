# fundamentosTI23

Tutorial para a utilização do git

1. primeiro devemos criar uma nova chave SSH, para isso podemos fazer direto pelo git, ou pela linha de comando - que é o nosso caso -, pela linha de comando nós devmos inicialmente abrir o Git Gash, senão tiver, deve baixar. Após o app aberto, devemos digitar hot, após isso você terá criado uma nova chave utilizando o seu email como etiqueta.

é possivel que o comando faça o pedido de uma nova chave, ai criamos uma personalizada - para personalizar apenas mudamos o "ssh-keygen" para o nome que quisermos.

2. em seguida, copiamos a chave SSH e abrimos o github, vamos nas configurações e logo depois clicamos nas teclas SSH e GPG, vamos no botão de nova chave SSH, damos um titulo, que geralmente é o nome do dispositivo do qual vamos usar a chave e em seguida a colamos no local de "key", assim ela sera criada

3. precisamos testar para ver se tudo está ocorrendo normalmente, então clonamos o repositório desejado, usando a chave SSH que ele fornece, usando o terminal "git clone" e a chave, nós o clonamos, assim veremos se está funcionando normalmente, podemos até mesmo a modificar e passar novamente

4. precisamos criar uma pasta dentro do SSH e configurar nossos dados para o git, ou seja, como eu uso o windows o git vai procurar pelo arquivo .gitconfig, para adicionar nossa identidade usamos os comando:

$ git config --global user.name "NOME"
$ git config --global user.email EMAIL

fazendo isso, nã precisaremos mais refazer pois a opção --global faz com que o git utilize essas informações para qualquer outra coisa que for feita no sistema

5. para clocar um projeto devemos entrar no git, escolher o repositório desejado, pegar a chave SSH e colar no nosso terminal logo após o comando git clone, assim ele será clonado

6. para criar uma nova branch devemos digitar os comandos git checkout com a flag -b e o nome escolhido, ou seja: git checkout -b NOME

colocar git status

7. editamos o README que agora estaria com o nosso nome após criarmos uma nova branch, utilizamos o comando git add -A que vai fazer a edição local e depois usamos o commit git commit -m "nova frase"

8. por fim criamos uma pull request para o repositório original, devemos navegar até o repositório onde você fizemos o fork e pressionar o botão “New pull request” no lado esquerdo da página
