Comandos do GIT
>git init = Inicial repositório atual te colocando na branch master.
>
>git add "." ou git ad "nome_do_arquivo" = O git add . adiciona todos os arquivos modificados ao Stage, já o git add nome_do_arquivo adiciona somente aquele arquivo em especifico.
>
>git status = Mostra o status atual da sua branch, em q branch voce está, se tem arquivos a serem adicionados na preparação antes do commit(Stage). Após ele ser adicionado ao stage, o arquivo estará pronto para ser comitado.

> git rm --cached "nome_do_arquivo" = remove aquele arquivo do stage. 

>git commit -m"sua mensagem" = A mensagem é a identificação do que aquele commit é, por ex: "forma de pagamento adicionada"/"inicio do repositório".

>git log = Mostra o histórico dos commits, quem fez, em que branch estava...
>git log --oneline = Variação do git log de forma mais condensada, ele da menos informações.

> git checkout "id_do_commit"= Usando o id do commit, volta á determinado ponto do sistema, não mostrando mais o que tem á frente daquele ponto.

>git checkout main/nome_da_branch = Sai do git checkout e volta á branch atual. 
>git checkou -b "nomeDaBranch": cria a branch e ja faz o checkout
>git revert "id_do_commit" = O git reverte as alterações feitas até então e criando um novo commit, deve ser confirmado digitando ":q". A reversão fica salva no histórico.

>git reset "id_do_commit": volta pra determinado tempo mas as alterações futuras ainda permanecem.
>git reset "id_do_commit" --hard: Volta áquele determinado momento e limpa todo o histórico futuro(sem possibilidade de recuperação).>

>git branch: puxa a lista de branchs no repositório.
>
>git branch "nome_branch": Cria nova branch.
>git merge "nome_da_branch": Faz a fusao entre as branchs, geralmente feito dentro da branch main para juntar outras branchs a ela.

>git push "enderecoGithub" "nomedabranch": "Empurra" os arquivos da branch pro github

>git remote add origin "enderecoGithub": Define o endereço do repositorio do github pra onde aquele projeto sempre vai ser "empurrado".

>git clone "EnderecoSShProjeto": Clona o repositório do github pra sua máquina localmente
>(também pode passar depois do endereco do repositório um nome q voce queira pro projeto)

>git pull origin main:  Baixa as mudanças do repositório no github, atualizando seu computador(maquina/repositorio local)


> [!Conjugando comandos Git]
> Dá pra conjugar(juntar) comandos git usando "&&", ex: git add . && gi commit -m"Pagamento adicionado".
