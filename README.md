# senai - versoes - colaboracoes

readme de exemplo


Role para baixo
 
Desafio 2 - Parte 1
No desafio 1, você viu que o Git é um sistema de controle de versão, fez a sua instalação e a configuração inicial necessária para o seu funcionamento. Daremos início agora à jornada para utilizá-lo na prática.

Nesta etapa, você desenvolverá o desafio 2:

Realizará todas as configurações e demais ações necessárias, para a prática de monitoramento e gerenciamento de alterações no código.
Para facilitar o seu entendimento, dividiremos os conhecimentos a seguir em duas partes:

Na primeira parte, você estudará:

A estrutura e organização de arquivos;
Termos e comandos básicos para criar arquivos, rastrear alterações, adicionar versões, verificar e salvar alterações;
Criação de repositórios locais e remotos (online).
Na segunda parte, você conhecerá:

Publicação de repositório online;
Criação de ramificações (branchs);
Como ignorar alterações.


Estrutura Digital
Antes de mais nada, é necessário organizar a estrutura digital para o projeto.

Assista ao vídeo e descubra porque é importante organizar seus arquivos.

Termos e comandos
Agora vamos abordar outros termos típicos da área para que você comece a se familiarizar.

Prompt

Repositório local

Repositório remoto

Staging

Commit

Ramo principal

Branch

Readme

.gitignore


Vamos abordar também alguns comandos, como:

git init

git status

git add

git commit

git log

git show número-do-commit

git remote add origin "destino"

git remote –v

git push -u origin main

git pull

Criando a estrutura inicial
Para resolver o desafio proposto (realizar as configurações para o monitoramento e gerenciamento de alterações no código) usando o Git, o primeiro passo é criar o repositório local.

Vamos criar uma pasta chamada senai-versoes-colaboracoes.

Clique nas abas para acompanhar o passo a passo.

Acesse uma pasta de sua preferência em seu computador (no exemplo, é a "_git");
Clique na área em branco dentro da pasta "_git" com o botão direito do mouse;
Com o botão esquerdo do mouse, clique em → "Novo" → "Pasta".
Tela 1
Nomeie como "senai-versoes-colaboracoes".
Tela 1
Nesta pasta "senai-versoes-colaboracoes", serão feitos o rastreamento de suas atividades, a criação dos arquivos e também a solução desse desafio.
Tela 1

Criando um repositório git local
Um repositório Git é um armazenamento virtual para os projetos, no qual serão gravadas as versões do código e que você poderá sempre acessar quando necessário. O repositório local é a pasta/diretório da sua máquina com o seu projeto.

Clique nas abas para aprender como começar a usar o Git.

● Para criar o repositório Git local, dê um duplo clique na pasta "senai-versoes-colaboracoes" criada anteriormente para acessá-la.

Tela 1
● Clique na área em branco dentro da pasta "senai-versoes-colaboracoes" com o botão direito do mouse e inicialize o Git Bash, clicando em "Git Bash Here".

Tela 1
● O prompt abrirá e nele você vai digitar todos os comandos.

Tela 1
Você pode usar o prompt de comando do seu sistema operacional para digitar os comandos Git. Por estarmos usando o Windows como exemplo de sistema operacional, usaremos o Git Bash, que emula o terminal do Git, e digitaremos todos os comandos no terminal do Git Bash.


Comandos iniciais
Aqui abordaremos alguns comandos básicos para começar a trabalhar com o Git.

Os próximos passos serão:

iniciar o repositório - comando git init;
criar um arquivo de texto dentro do repositório;
rastrear alterações no repositório - comando git status;
adicionar versão no repositório - comando git add;
verificar alterações antes de salvar - comando git status;
salvar alterações - comando git commit; e
visualizar log da alteração - comando git log.
Iniciar o repositório: comando git init
O primeiro comando que executaremos é o git init, que vai inicializar o repositório local em nossa pasta senai-versoes-colaboracoes.

Ao ser executado, esse comando cria uma pasta chamada .git, com subdiretórios (objects, refs/heads, refs/tags), e transforma o diretório atual em um repositório do Git. Na imagem a seguir, o terminal informa que o repositório está vazio, pois nenhum arquivo foi incluído.
Clique sobre a imagem para ampliá-la.

DVCS
Agora, a pasta senai-versoes-colaboracoes é o repositório local e, dentro dela, há outra pasta chamada .git, criada com o comando git init.

DVCS
Criar um arquivo de texto dentro do repositório
Antes do próximo comando (rastrear alterações), devemos criar um arquivo para ser alterado e rastreado.

Clique nas abas a seguir para conhecer o processo.

Dentro da pasta "senai-versoes-colaboracoes", crie um arquivo de texto, chamado "versoes", com a extensão ".txt". Para criar esse arquivo, clique na área em branco da pasta "senai-versoes-colaboracoes" com o botão direito do mouse e, então, clique em "Novo" → "Documento de texto".
Tela 1
● Nomeie o arquivo como "versoes.txt".

Tela 1
● Você possui uma pasta chamada "senai-versoes-colaboracoes" com uma subpasta do .git e um arquivo de texto criado.

Tela 1
Rastrear alterações no repositório: comando git status
Você criou um arquivo, mas ele ainda não está sendo rastreado pelo Git e, consequentemente, as informações não foram salvas em seu repositório. Isso significa que o Git ainda não está fazendo o monitoramento de alterações de seu arquivo.

Para verificarmos o status das alterações que foram realizadas dentro de um repositório, utiliza-se o comando git status. Esse comando nos ajuda a verificar ao longo do tempo de desenvolvimento de seu projeto, quais arquivos estão sendo alterados por você em sua máquina dentro do repositório.
Clique sobre a imagem para ampliá-la.

DVCS
Então, de um repositório Git vazio do início, agora temos o diretório senai-versoes-colaboracoes com uma pasta .git, que não conta como uma alteração e que contém informações relacionadas a nosso versionamento e informações do nosso repositório, e um arquivo de texto chamado "versoes.txt". Ao adicionar um arquivo, fizemos uma alteração.

Tela 1
Adicionar versão no repositório: comando git add
O arquivo "versoes.txt" ainda não foi adicionado ao histórico do projeto. Para isso, primeiro devemos registar a alteração com o comando git add, depois salvá-la no nosso repositório com o comando git commit e, aí sim, podemos considerar a alteração adicionada ao histórico. Depois do comando git add, as alterações vão para um ponto seguro, onde é possível verificar as alterações antes de salvá-las, chamado Staging.

Tela 1
O comando git add [nome-do-arquivo] adiciona os arquivos modificados na área de staging, que é um ponto intermediário entre a máquina do desenvolvedor e o repositório de trabalho. A staging é uma área que você pode fazer uma revisão do que foi alterado antes de ser salvo no histórico de alterações.

DVCS
Caso você tenha mais de um arquivo, você pode executar o comando git add. para adicionar todos os arquivos que foram modificados.

Verificar alterações antes de salvar: comando git status
Para verificar essas alterações antes de confirmar, você pode utilizar o comando git status.

DVCS
As alterações no Git, diferentemente de outros tipos de versionamento de código, podem ser feitas localmente e depois publicadas em um repositório remoto (disponível online e para outras pessoas).

Salvar alterações: comando git commit
Um dos passos mais importantes é confirmar as alterações do fluxo de trabalho em versões no histórico do repositório. O Git irá confirmar a captura do diretório de staging (isto é, a captura de todas as alterações adicionadas no git add) e salvar no histórico de confirmação de repositórios, completando o commit.

Tela 1
Veja como digitar o comando completo git commit –m "meu primeiro commit" na imagem a seguir.

GIT COMMIT
Importante

Por padrão, todas as alterações serão feitas no ramo principal do repositório, chamada main. Você pode criar ramificações da main para testar parte do código, chamadas de branch. Por enquanto, mantenha em mente que todas as alterações estão sendo feitas na linha de trabalho principal, na main1.

GIT COMMIT
Visualizar log da alteração: comando git log
Para visualizar as alterações feitas no seu repositório de trabalho, você pode executar o git log no terminal.

Log
Uma das vantagens do Git é visualizar as informações que foram alteradas em um determinado ponto do desenvolvimento. As alterações que foram confirmadas podem ser visualizadas pelo terminal ao executar o comando git log.

Log
Para visualizar as alterações ao longo do projeto, usamos o comando git show número-do-commit.

Log
Assista ao vídeo que resume todos os comandos básicos abordados até agora.

Devido ao movimento Black Lives Matter, alguns termos que remetiam a escravidão foram substituídos. O termo “master” foi substuído por “main”.


PDF

Clique aqui para baixar o PDF ccom o mesmo conteúdo do vídeo.


Criando um Repositório Online
Para disponibilizar o repositório local, temos que utilizar um repositório online e, para isso, vamos utilizar a plataforma GitHub.

Importante

O usuário do GitHub aparece em alguns comandos no repositório local. Lembre-se, portanto, de trocar o do exemplo (hstrada) pelo seu usuário quando for praticar.

Clique no player a seguir para acessar o vídeo que mostra como fazer o cadastro no GitHub.


Parte 2
Agora que você já sabe como organizar arquivos no Git, os comandos básicos para criar arquivos, rastrear alterações, adicionar versões, verificar e salvar alterações e criar repositórios locais e remotos, siga em frente para a segunda parte para aprender como:

Publicar repositório online;
Criar ramificações (branchs);
Ignorar alterações.

Publicando no repositório online
Você criou um repositório online, mas não especificou que é neste repositório que gostaria de publicar seu trabalho.


Depois de criar o repositório remoto, precisamos fazer a ligação com o repositório local. Para isso, no terminal local, vamos:

informar a pasta remota: git remote add origin git@github.com:hstrada/senai-versoes-colaboracoes.git (lembre-se de trocar o usuário no comando);
visualizar o repositório remoto: git remote –v; e
publicar as alterações no repositório remoto: git push -u origin main.
No repositório remoto, vamos:

autorizar o usuário.
Depois, vamos verificar se todas as etapas foram completadas corretamente, então, devemos:

no repositório local: visualizar a autenticação de usuário feita no repositório remoto;
no repositório remoto: visualizar a publicação feita.
Informar no repositório local a pasta remota: git remote add origin git@github.com:hstrada/senai-versoes-colaboracoes.git
Para realizar a ligação dos repositórios, primeiro é necessário informar no repositório local que o repositório remoto que você deseja trabalhar é aquele criado no GitHub, através do comando git remote add origin git@github.com:hstrada/senai-versoes-colaboracoes.git.

DVCS

Visualizar o repositório remoto: git remote –v
Para visualizar o repositório remoto informado e visualizar as informações, digite no terminal git remote –v.

DVCS
Publicar as alterações no repositório remoto: git push -u origin main
Para publicar as alterações no repositório remoto, execute o comando git push -u origin main.

DVCS
Autorizar usuário no repositório remoto
O repositório criado no GitHub está atrelado à sua conta e, portanto, seu user deve ser autorizado a se comunicar com seu repositório local.

Clique nas abas de navegação para saber como fazer esse procedimento.

● Para criar um Personal Access Token, precisamos acessar a opção Settings. Para isso, clique na sua foto de perfil no lado direito do cabeçalho da página.

Tela 1
● Após acessar as configurações do perfil, clique na opção Developer Settings, localizada na aba de opções na lateral esquerda.

Tela 1
● Nessa tela, selecione a opção de Personal access tokens, e depois clique no botão Generate new token, para iniciar a geração desse novo token de acesso pessoal.

Tela 1
● Nessa tela, você terá as opções de configuração do token, incluindo uma breve descrição (Note), seu prazo de validade (Expiration) e também as operações que são permitidas ao utilizá-lo (Scopes).

● No nosso exemplo, vamos criar um token sem prazo de validade, que fará com que ele não expire, e o escopo selecionaremos a opção repo, que já será suficiente para as operações básicas nos repositórios.

Tela 1
● Após selecionar as configurações, clique no botão “Generate token” no final da página.

● Depois de gerar o token, ele será exibido na tela. Copie-o e guarde-o como se fosse uma senha. Depois de sair dessa tela, o token não será mais mostrado, por isso é importante copiá-lo.

Tela 1
● Agora que temos o token criado, para fazermos as operações de push no Github, quando for solicitado usuário e senha, você deverá inserir o token no campo de senha (Password)

Tela 1
Verificações
Depois de autorizar seu usuário no GitHub, vamos fazer as verificações local e remota.

Seu terminal local deve mostrar as informações como a imagem a seguir.

DVCS
● Acesse o navegador e atualize a página para visualizar as informações publicadas.

Tela 1
● Para visualizar as alterações, clique nos "commits".

● É o equivalente a executar o git show no terminal local.

Tela 1
● Podemos visualizar as alterações de cada "commit" ou estado atual do projeto.

● Clique no "commit" mais antigo.

Tela 1
● Todas as informações sobre as alterações realizadas no arquivo serão exibidas.

Tela 1
Assista ao vídeo para conhecer as principais ações executadas para criar, publicar e gerenciar ações no GitHub.

Devido ao movimento Black Lives Matter, alguns termos que remetiam a escravidão foram substituídos. O termo “master” foi substuído por “main”.


PDF

Clique aqui para baixar o PDF com o mesmo conteúdo do vídeo.

A imagem a seguir mostra o fluxo atual de trabalho com as alterações feitas.

DVCS

Fluxo de Trabalho
Neste primeiro cenário de fluxo de trabalho, todas as alterações estão sendo feitas no nosso ramo principal, que chamamos de main.

Muitas vezes, durante o desenvolvimento do projeto, há a necessidade de testar ou corrigir algum trecho do código-fonte ou adicionar um novo recurso, para isso, criamos ramificações do main, chamados branchs.


Esse tipo de abordagem facilita o processo de desenvolvimento entre diferentes pessoas, possibilitando manter o código oficial como base, descentralizando o desenvolvimento.

Pense Nisso

Assim como você, outros programadores da equipe também enviam suas respectivas alterações para o repositório online. Portanto, cada programador tem em sua máquina apenas as suas alterações e somente o repositório remoto está atualizado e completo. Acompanhe, a seguir, como baixar as alterações do repositório online para a sua máquina.

Baixando as alterações de um repositório remoto
O nosso repositório local deve ser uma cópia do repositório remoto. Isso significa que devemos enviar nossas alterações para o repositório remoto e também baixar as alterações de lá para nossa máquina.

Então, para aprender como sincronizar e baixar as alterações quando o repositório remoto for atualizado, vamos:

fazer uma alteração diretamente no repositório remoto; e
baixar a alteração no repositório remoto: git pull.
Vamos também abordar uma técnica muito útil para:

impedir que uma alteração seja monitorada: arquivo .gitignore.
Fazer uma alteração diretamente no repositório remoto
Vamos criar um arquivo README no repositório remoto para simular uma alteração feita por outro programador.

DICA

O README.md é um arquivo de texto utilizado para descrever, documentar ou exemplificar seu projeto. Apesar de não ser obrigatório (seu código vai funcionar perfeitamente sem ele), o README é essencial, pois mescla o cartão de visitas e a ementa do projeto, sendo o responsável por cativar interesse em seu trabalho ou relembrá-lo dos aspectos gerais e pontos relevantes daquele desenvolvimento.

A extensão .md representa um arquivo Markdown, uma linguagem de marcação com a qual você pode exibir diversas formatações de texto (bold, itálico, cabeçalhos, entre outros).

Por padrão, o README.md sempre vai estar disponível, acessível e visível nos repositórios remotos.

Clique nas abas de navegação para aprender como criar um arquivo README no repositório remoto.

● Acesse o repositório remoto através do link "github/seu-usuário/nome-repositório". No nosso exemplo: "https://github.com/
hstrada/senai-versoes-colaborações".

Tela 1
● Clique em "Add a README".

Tela 1
● Adicione um comentário.

Tela 1
● Clique em "Commit new file".

Tela 1
● Você criou o "README" no repositório remoto, agora é necessário baixar as alterações para o repositório local.

Tela 1
Baixar a alteração no repositório remoto: git pull
Para baixar a atualização de seu repositório remoto para seu repositório local, execute no terminal local o comando git pull.

Agora é possível visualizar a atualização baixada no diretório local.

DVCS
Tela 1
Impedir que uma alteração seja monitorada: arquivo .gitignore
Imagine que você estava testando um trecho de código que não deu certo e, portanto, você não quer publicá-lo. Com o Git, é possível gerenciar arquivos que não desejamos publicar. Para isso, você deve criar um arquivo .gitignore dentro da pasta do projeto e informar quais arquivos você deseja ignorar. Podemos adicionar pastas, arquivos ou qualquer outro item que não desejamos publicar e/ou adicionar em nosso repositório.

Clique nas abas de navegação para aprender como ignorar alterações.

● Crie um arquivo de texto chamado "arquivo-nao-publicado.txt" em nossa pasta de trabalho "senai-versoes-colaboracoes".

Tela 1
● Crie um arquivo de texto e o nomeie como ".gitignore".

Tela 1
● Clique em "Sim" para aceitar.

Tela 1
● Agora vamos inserir o arquivo que deve ser ignorado, o "arquivo-não-publicado.txt".

Tela 1
● Adicione o nome do arquivo "arquivo-nao-publicado.txt" que você não deseja que o Git faça o rastreio.

Tela 1
● Vamos verificar os status das modificações locais. No Git Bash, execute o comando git status.

● Note que o "arquivo-nao-publicado.txt" não foi reconhecido como modificado/inserido/editado.

Tela 1
● Adicione as alterações com o git add, confirme com o git commit e publique no repositório remoto com o git push.

Tela 1
● Retorne ao GitHub e atualize a página. Observe que o arquivo que adicionamos ao .gitignore não sofreu nenhuma ação ao realizarmos um commit (isso funciona para os arquivos que ainda não foram rastreados).

Tela 1
DICA

Você pode ter reparado que, em alguns momentos durante os commits, adicionávamos comentários semânticos, ou seja, direcionados a quem estava lendo aquela alteração. No exemplo a seguir, o comentário está entre aspas ("adicionando o gitignore").

Tela 1
Esse comentário serve como lembrete do que foi feito no commit. Assim, ao puxar o histórico, você saberá o que foi feito nesse commit sem precisar abri-lo.

Tenha cuidado ao escrever o comentário. Se no exemplo o comentário fosse apenas "gitignore", você não teria como saber qual a alteração feita no arquivo gitignore (o gitignore foi apagado ou adicionado?) e você teria que abrir o commit para descobrir o que significa o comentário.

É uma boa prática de documentação, que deve estar presente em todos os seus projetos e que facilita o desenvolvimento e a visualização das alterações entre a equipe.

Assista ao vídeo que resume todos os comandos básicos abordados até agora.

Devido ao movimento Black Lives Matter, alguns termos que remetiam a escravidão foram substituídos. O termo “master” foi substuído por “main”.


PDF

Clique aqui para baixar o PDF com o mesmo conteúdo do vídeo.


Readme.md
README.md é um arquivo com extensão .md (Markdown), cujo objetivo é conter informações essenciais sobre o projeto.

Em outras palavras, o README.md é a documentação técnica geral do projeto.

O README.md é um arquivo utilizado para descrever, documentar ou exemplificar seu projeto. Apesar de não ser obrigatório (seu código vai funcionar perfeitamente sem ele), o README é essencial, pois mescla o cartão de visitas e a ementa do projeto, sendo o responsável por cativar interesse em seu trabalho ou relembrá-lo dos aspectos gerais e pontos relevantes daquele desenvolvimento.

Por boas práticas, o README.md sempre deve estar disponível, acessível e visível nos repositórios remotos.

Markdown
Markdown Syntax é um tipo de linguagem de marcação, assim como o HTML. A sintaxe facilita a formatação de textos na web, funcionando como um conversor de texto para HTML.

O Markdown também utiliza tags, porém diferentes do HTML. Veja a lista de tags básicas para formatar seu README:

títulos
ênfase
listas
links
tabelas
imagens
Clique no player a seguir para acessar o vídeo sobre instalação do VS Code e de extensões para Git.


Clique nas setas de navegação para conhecer as principais tags para criar seu readme.

1/6
Títulos

A tag de título é a # (hashtag). Basta iniciar o título com a hashtag seguido do texto. Quanto maior o número de hashtags, menor o tamanho do título. Observe que o título 1 é automaticamente acompanhado de uma linha.


Saiba mais...

Há várias maneiras de formatar seu readme, pesquise! Para saber como inserir emojis, por exemplo, clique aqui. Para inserir uma formatação de fonte do tipo código de programação, clique aqui. Para formatar tabelas, clique aqui. Para listas e outras dicas, clique aqui.

Construindo Readme
O foco do nosso readme será uma documentação mais técnica. O que seria necessário eu informar para outro colaborador para que ele possa ser capaz de colaborar com o nosso projeto?
Clique nas abas a seguir para saber como construir o seu readme.

Título e descrição

Features

Tecnologias utilizadas

Organização do projeto

Pré-requisitos de instalação

Execução da aplicação

Erros comuns


Contribuidores

Dica

Nem todos os itens dessa lista são obrigatórios. Quanto mais completo for o seu README, melhor será o entendimento para as pessoas que não fazem parte do projeto e que queiram contribuir.

Outra dica: use o idioma inglês se possível. É comum encontrar projetos com a descrição e o código fonte escrito em inglês, pois ele é muito usado e isso ajuda na expansão de seu projeto.

Confira a seguir um exemplo completo do código fonte de um arquivo readme.md.

zoom_in
