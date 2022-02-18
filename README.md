# Estudo: Git & GitHub

## O que é controle de versão?
O controle de versão, também conhecido como controle de origem, é a prática de rastrear e gerenciar alterações no código do software.
Os sistemas de controle de versão são ferramentas de software que ajudam as equipes de software a gerenciar as alterações no código-fonte ao longo do tempo. À medida que os ambientes de desenvolvimento se aceleram, os sistemas de controle de versão ajudam as equipes de software a trabalhar de forma mais rápida e inteligente.
O software de controle de versão acompanha cada modificação do código em um tipo especial de banco de dados. 
O código de um projeto, aplicativo ou componente de software normalmente é organizado em uma estrutura de pastas ou "árvore de arquivos". Um desenvolvedor da equipe pode estar trabalhando em um novo recurso enquanto outro desenvolvedor corrige um bug não relacionado alterando o código, cada desenvolvedor pode fazer suas alterações em várias partes da árvore de arquivos.
Se for cometido um erro, os desenvolvedores podem voltar no tempo e comparar versões anteriores do código para ajudar a corrigir o erro e minimizar a interrupção para todos os membros da equipe.
O controle de versão ajuda as equipes a resolver esses tipos de problemas, rastreando cada alteração individual, de cada colaborador, e ajudando a evitar que o trabalho simultâneo entre em conflito. As alterações feitas em uma parte do software podem ser incompatíveis com as feitas por outro desenvolvedor trabalhando ao mesmo tempo. Este problema deve ser descoberto e resolvido de forma ordenada, sem bloquear o trabalho do restante da equipe. Além disso, em todo o desenvolvimento de software, qualquer alteração pode introduzir novos bugs por conta própria e o novo software não pode ser confiável até que seja testado. Assim, o teste e o desenvolvimento prosseguem juntos até que uma nova versão esteja pronta.
O software de controle de versão é uma parte essencial do dia a dia das práticas profissionais da equipe de software moderna. Desenvolvedores de software individuais que estão acostumados a trabalhar com um sistema de controle de versão capaz em suas equipes normalmente reconhecem o incrível valor que o controle de versão também lhes oferece, mesmo em pequenos projetos individuais.
Os sistemas de controle de versão (VCS) tiveram grandes melhorias nas últimas décadas. VCS às vezes são conhecidos como ferramentas SCM (Source Code Management) ou RCS (Revision Control System). Uma das ferramentas VCS mais populares em uso hoje é chamada Git. Git é um Distributed VCS, uma categoria conhecida como DVCS, mais tarde abordaremos este assunto. Como muitos dos sistemas VCS mais populares disponíveis hoje, o Git é gratuito e de código aberto.

## Benefícios dos sistemas de controle de versão
1. Um histórico completo de alterações de cada arquivo. As alterações incluem a criação e exclusão de arquivos, bem como edições em seu conteúdo.
Ferramentas VCS diferem em quão bem elas lidam com renomeação e movimentação de arquivos. Esse histórico também deve incluir o autor, data e notas escritas sobre o objetivo de cada alteração. Ter o histórico completo permite voltar a versões anteriores para ajudar na análise de causa raiz de bugs e é crucial quando é necessário corrigir problemas em versões mais antigas do software.

2. Ramificação e fusão. A criação de uma "ramificação" (branch) nas ferramentas VCS mantém vários fluxos de trabalho independentes uns dos outros, ao mesmo tempo em que fornece a facilidade de mesclar esse trabalho novamente, permitindo que os desenvolvedores verifiquem se as alterações em cada filial não são conflitantes. Muitas equipes de software adotam uma prática de ramificação para cada recurso ou talvez ramificação para cada versão, ou ambas. Há muitos fluxos de trabalho diferentes que as equipes podem escolher quando decidem como usar os recursos de ramificação e mesclagem no VCS.

3. Rastreabilidade. Ser capaz de rastrear cada alteração feita no software e conectá-lo ao software de gerenciamento de projetos e rastreamento de bugs, como o Jira , e ser capaz de anotar cada alteração com uma mensagem descrevendo o propósito e a intenção da alteração pode ajudar não apenas na análise da causa raiz e outros forenses. Ter o histórico anotado do código na ponta dos dedos quando você está lendo o código, tentando entender o que ele está fazendo e por que ele foi projetado pode permitir que os desenvolvedores façam alterações corretas e harmoniosas que estejam de acordo com o design de longo prazo pretendido do sistema. Isso pode ser especialmente importante para trabalhar efetivamente com código legado e é crucial para permitir que os desenvolvedores estimem o trabalho futuro com precisão.

## Gerenciamento de código-fonte
O gerenciamento de código-fonte (SCM) é usado para rastrear modificações em um repositório de código-fonte. O SCM rastreia um histórico de alterações em uma base de código e ajuda a resolver conflitos ao mesclar atualizações de vários colaboradores.
 
## Práticas recomendadas de gerenciamento de código-fonte

1. Comprometa-se com frequência
Commits são baratos e fáceis de fazer. Eles devem ser feitos com frequência para capturar atualizações em uma base de código. Cada commit é um instantâneo para o qual a base de código pode ser revertida, se necessário. Commits frequentes dão muitas oportunidades para reverter ou desfazer o trabalho. Um grupo de commits pode ser combinado em um único commit usando um rebase para esclarecer o log de desenvolvimento.

2. Verifique se você está trabalhando na versão mais recente
O SCM permite atualizações rápidas de vários desenvolvedores. É fácil ter uma cópia local da base de código atrás da cópia global. Certifique-se de puxar ou buscar (pull) o código mais recente antes de fazer atualizações. Isso ajudará a evitar conflitos no momento da mesclagem.

3. Faça anotações detalhadas
Cada commit tem uma entrada de log correspondente. No momento da criação do commit, essa entrada de log é preenchida com uma mensagem. É importante deixar mensagens de log de confirmação descritivas e explicativas. Essas mensagens de log de commit devem explicar o “porquê” e “o que” que englobam o conteúdo dos commits e deixam um rastro para futuros colaboradores revisarem.

4. Revise as alterações antes de confirmar
SCM's oferecem uma 'área de preparação' (staging area). A área de teste pode ser usada para coletar um grupo de edições antes de gravá-las em um commit.

5. Usar Branches
Branching é um mecanismo SCM poderoso que permite aos desenvolvedores criar uma linha de desenvolvimento separada. As branches devem ser usadas com frequência, pois são rápidas e baratas. As branches permitem que vários desenvolvedores trabalhem em paralelo em linhas de desenvolvimento separadas. Essas linhas de desenvolvimento geralmente são características de produtos diferentes. Quando o desenvolvimento é concluído em uma branch, ela é incorporada à linha principal de desenvolvimento.

6. Concordar em um fluxo de trabalho
Por padrão, os SCMs oferecem métodos de contribuição de forma muito livre. É importante que as equipes estabeleçam padrões compartilhados de colaboração.

## Instalando o Git no Windows
1. Baixe o instalador: Link: https://gitforwindows.org/

2. Ao iniciar o instalador, você deverá ver a tela do assistente de configuração do Git . Siga os prompts "Avançar" e "Concluir" para concluir a instalação.

3. Abra um prompt de comando e faça:
- ``` $ git config --global user.name "Emma Paris" ```
- ``` $ git config --global user.email "eparis@atlassian.com" ```

## Instalando o Git no Linux
1. Debian / Ubuntu (apt-get): Os pacotes Git estão disponíveis via apt (https://wiki.debian.org/Apt)

2. Do seu shell, instale o Git usando apt-get:
- $ sudo apt-get update  ``` 
- $ sudo apt-get install git  ``` 

3. Verifique se a instalação foi bem-sucedida digitando:
- ``` $ git --version ```

4. Configure seu nome de usuário e e-mail do Git usando os comandos a seguir, substituindo o nome de Emma pelo seu. Esses detalhes serão associados a qualquer commit que você criar:

- ``` $ git config --global user.name "Emma Paris"  ``` 
- ``` $ git config --global user.email "eparis@atlassian.com"  ```

## O que é uma CHAVE SSH?
Uma chave SSH é uma credencial de acesso para o protocolo de rede SSH (secure shell). Esse protocolo de rede seguro autenticado e criptografado é usado para comunicação remota entre máquinas em uma rede aberta não segura . O SSH é usado para transferência remota de arquivos, gerenciamento de rede e acesso remoto ao sistema operacional.
O SSH usa um par de chaves para iniciar um handshake seguro entre partes remotas. O par de chaves contém uma chave pública e privada. A nomenclatura privada versus pública pode ser confusa, pois ambas são chamadas de chaves. É mais útil pensar na chave pública como uma "cadeia" e na chave privada como a "chave". Você dá o 'bloqueio' público a partes remotas para criptografar ou 'bloquear' os dados. Esses dados são então abertos com a chave 'privada' que você mantém em um local seguro.

#### Como criar uma chave SSH
As chaves SSH são geradas por meio de um algoritmo criptográfico de chave pública , sendo o mais comum RSA ou DSA . Em um nível muito alto, as chaves SSH são geradas por meio de uma fórmula matemática que leva 2 números primos e uma variável de semente aleatória para gerar a chave pública e privada. Essa é uma fórmula unidirecional que garante que a chave pública possa ser derivada da chave privada, mas a chave privada não pode ser derivada da chave pública.

#### Gerar uma chave SSH no Mac e Linux
Os sistemas operacionais OsX e Linux possuem aplicativos de terminal modernos e abrangentes que acompanham o pacote SSH instalado. O processo para criar uma chave SSH é o mesmo entre eles.

1. execute o seguinte para iniciar a criação da chave
- ``` ssh-keygen -t rsa -b 4096 -C "your_email@example.com" ``` <P>
Este comando criará uma nova chave SSH usando o e-mail como rótulo

2. Em seguida, você será solicitado a "Inserir um arquivo no qual deseja salvar a chave".
Você pode especificar um local de arquivo ou pressionar “Enter” para aceitar o local de arquivo padrão.
- ``` > Enter a file in which to save the key (/Users/you/.ssh/id_rsa): [Press enter] ```
 
3. O próximo prompt solicitará uma senha segura.
Uma frase secreta adicionará uma camada adicional de segurança ao SSH e será necessária sempre que a chave SSH for usada. Se alguém obtiver acesso ao computador em que as chaves privadas estão armazenadas, também poderá obter acesso a qualquer sistema que use essa chave. Adicionar uma senha às chaves evitará esse cenário.
- ```  > Enter passphrase (empty for no passphrase): [Type a passphrase] ``` 
- ```  > Enter same passphrase again: [Type passphrase again] ```  <P>
 
Neste ponto, uma nova chave SSH terá sido gerada no caminho do arquivo especificado anteriormente.

4. Adicione a nova chave SSH ao agente ssh

O ssh-agent é outro programa que faz parte do conjunto de ferramentas SSH. O agente ssh é responsável por manter as chaves privadas. Pense nisso como um chaveiro. Além de manter as chaves privadas, também intermedia solicitações para assinar solicitações SSH com as chaves privadas, para que as chaves privadas nunca sejam passadas sem segurança.

Antes de adicionar a nova chave SSH ao ssh-agent, primeiro verifique se o ssh-agent está em execução executando:
- ``` $ eval "$(ssh-agent -s)" ```
- ``` > Agent pid 59566 ```
 
Quando o ssh-agent estiver em execução, o comando a seguir adicionará a nova chave SSH ao agente SSH local.
- ``` ssh-add -K /Users/you/.ssh/id_rsa ```
 
A nova chave SSH agora está registrada e pronta para uso!
 
#### Gerar uma chave SSH no Windows
Os ambientes Windows não possuem um shell unix padrão. Programas shell externos precisarão ser instalados para ter uma experiência completa de geração de chaves. A opção mais direta é utilizar o Git Bash (https://www.atlassian.com/git/tutorials/git-bash). Depois que o Git Bash estiver instalado, as mesmas etapas para Linux e Mac podem ser seguidas no shell do Git Bash.

## configuração do git
O comando *git config* é uma função que é usada para definir valores de configuração do Git em um nível de projeto global ou local.
O comando *git config* pode aceitar argumentos para especificar em qual nível de configuração operar. Os seguintes níveis de configuração estão disponíveis:
- --local<p>
Por padrão, o comando *git config* gravará em um nível local se nenhuma opção de configuração for passada. A configuração de nível local é aplicada ao repositório de contexto git configem que é invocado. Os valores de configuração local são armazenados em um arquivo que pode ser encontrado no diretório .git do repositório:.git/config

- --global<p>
A configuração de nível global é específica do usuário, o que significa que é aplicada a um usuário do sistema operacional. Os valores de configuração global são armazenados em um arquivo localizado no diretório inicial de um usuário. ~ /.gitconfig em sistemas unix e em windows C:\Users\\.gitconfig

- --system<p>
A configuração no nível do sistema é aplicada em uma máquina inteira. Isso abrange todos os usuários em um sistema operacional e todos os repositórios. O arquivo de configuração no nível do sistema reside em um arquivo *git config* fora do caminho raiz do sistema.<p>

Assim, a ordem de prioridade para os níveis de configuração é: local, global, sistema. Isso significa que ao procurar um valor de configuração, o Git iniciará no nível local e subirá até o nível do sistema.
 
## Configurando um repositório
 
Um repositório Git é um armazenamento virtual do seu projeto. Ele permite que você salve versões do seu código, que você pode acessar quando necessário. 
 
#### Inicializando um novo repositório: git init
Para criar um novo repositório, você usará o comando:
- ``` git init ``` 
 
*git init* é um comando de uso único que você usa durante a configuração inicial de um novo repositório. A execução deste comando criará um novo subdiretório *.git* em seu diretório de trabalho atual. Isso também criará uma nova *branch* principal.
 
#### Versionando um projeto existente com um novo repositório git
Este exemplo pressupõe que você já tenha uma pasta de projeto existente na qual gostaria de criar um repositório. Você irá primeiro acessar a pasta do projeto raiz e, em seguida, executará o comando *git init*.

- ``` cd /path/to/your/existing/code ```
- ``` git init ``` <p>
 
Apontar *git init* para um diretório de projeto existente executará a mesma configuração de inicialização mencionada acima, mas com escopo para esse diretório de projeto.

 - ``` git init <project directory> ``` <p>
 
 #### Clonando um repositório existente: git clone
Se um projeto já foi configurado em um repositório central, o comando clone é a maneira mais comum de os usuários obterem um clone de desenvolvimento local. Assim como o comando *git init*, a clonagem geralmente é uma operação única. Depois que um desenvolvedor obtém uma cópia de trabalho, todas as operações de controle de versão são gerenciadas por meio de seu repositório local.

 - ``` git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY ``` <p>
 
Quando executado, a versão mais recente dos arquivos de repositório remoto na *branch* principal será baixada e adicionada a uma nova pasta. A pasta conterá o histórico completo do repositório remoto e uma ramificação principal recém-criada.

## Salvando alterações no repositório: git add e git commit
Agora que você tem um repositório clonado ou inicializado, você pode confirmar as alterações de versão do arquivo nele. O exemplo a seguir pressupõe que você configurou um projeto em */path/to/project*. As etapas que estão sendo executadas neste exemplo são:

1. Alterar diretórios para/path/to/project
- ``` cd /path/to/project  ```
 
2. Crie um novo arquivo CommitTest.txt com conteúdo: "Inclusão de novo arquivo para tutorial git"
- ``` echo "Inclusão de novo arquivo para tutorial git" >> CommitTest.txt  ```
 
3. *git add* CommitTest.txt para a área de STAGE do repositório
- ``` git add CommitTest.txt  ```

4. Crie um novo commit com uma mensagem descrevendo qual trabalho foi feito no commit
- ``` git commit -m "adicionado CommitTest.txt ao repositório"  ```

Depois de executar este exemplo, seu repositório agora passará a rastrear o arquivo *CommitTest.txt* coletando e armazenando seu histórico de alterações.
Este exemplo introduziu dois comandos git adicionais: *add* e *commit*. Este foi um exemplo muito limitado, mas ambos os comandos são abordados com mais profundidade nas páginas: https://www.atlassian.com/git/tutorials/saving-changes e https://www.atlassian.com/git/tutorials/saving-changes/git-commit.

Outro caso de uso comum *git add* é a opção *--all*. A execução do comando *git add --all* pegará todos os arquivos alterados e não rastreados no repositório e os adicionará ao repositório e atualizará a árvore de trabalho do repositório.


## Os estágios de um arquivo no Git

![1_LvJtV6HPdpSKpPNdjwf6jQ](https://user-images.githubusercontent.com/45216757/153660536-7700ea37-46ea-4799-8830-0c60c85dfd54.png)
O conceito dos três estados de um arquivo Git é muito importante para o entendimento e uso do Git. Não importa o momento, seus arquivos sempre estão em um dos três estados fundamentais:
1. modificado (modified),
2. preparado (staged) ou
3. consolidado (committed).

Toda vez que um arquivo é salvo no controle de versão, ou seja, é registrado uma versão, o Git armazena algo parecido com uma imagem do arquivo que representa seu estado atual.

![2_oX0oxuHK-SI3nW2BmdaPng](https://user-images.githubusercontent.com/45216757/153661631-cfc6a73c-c798-4472-b921-738eef63cca9.png)

**Modificado (modified)**<p>
No repositório, há um espaço no qual são registradas as modificações nos arquivos e estrutura de diretórios sob uma determinada versão (hash) escolhida pelo usuário. Este espaço é conhecido como Working Tree.
A Working Tree é o primeiro estágio quando se trata de gerar um novo estado para aquele repositório.
Uma vez no repositório, qualquer arquivo que é adicionado, modificado ou removido é marcado como modificado. Significa que o arquivo sofreu alterações, mas ainda não foi dito que ele fará parte do próximo commit, ou seja, da próxima versão que será consolidada.
Significa também que esses arquivos estão diferentes quando comparados com a última versão disponível no histórico.

**Preparado (staged)**<p>
O próximo estágio é indicar para o Git quais mudanças pertencerão ao próximo estado, isto é, corresponderão a nova versão. A seleção se dará baseada nas mudanças detectadas pela Working Tree. No terminal o comando *git add* permite selecionar algumas ou todas as mudanças detectadas lá.

Quando tais mudanças são adicionadas (através do comando *git add*), elas são registradas em um arquivo dentro do repositório *.git*. Neste momento, elas encontram-se na Staging Area (alguns chamam por index). O arquivo assume o estado de preparado (staged) e o Git sabe que o arquivo foi modificado e agora está na área de preparação(stage) para ser consolidado.
A área de stage pode ser pensada como a parte de trás das cortinas de uma apresentação. Pode ser que entre *ou* não no palco. É o momento da decisão!

**Consolidado (committed)**<p>
Nesta etapa será registrado no histórico as mudanças adicionadas na Staging Area. Ao utilizar o comando *git commit* um snapshot de todo o repositório é realizado.
Um snapshot também é comumente denominado de commit.

## Status do Git: inspecionando um repositório
#### git status
O comando *git status* exibe o estado da Working Tree e a área de stage. Ele permite que você veja quais alterações foram preparadas, quais não foram e quais arquivos não estão sendo rastreados pelo Git. A saída de status não mostra nenhuma informação sobre o histórico do projeto confirmado. Para isso, você precisa usar git log.
- ``` git status  ```

#### git tag
*Tags* são referências que apontam para pontos específicos no histórico do Git. O comando *git tag* é geralmente usado para capturar um ponto no histórico que é usado para um lançamento de versão.
A *tag* é como um branch que não muda. Ao contrário das ramificações, as tags, depois de criadas, não têm mais histórico de commits.
Para criar uma nova tag execute o seguinte comando:
- ``` git tag <tagname>  ```

O Git suporta dois tipos diferentes de tags:
1. tags e
2. anotadas e tags leves.<p>
O exemplo anterior criou uma tag leve. Tags leves e tags anotadas diferem na quantidade de metadados de acompanhamento que armazenam. Uma prática recomendada é considerar as tags anotadas como públicas e as tags leves como privadas. As tags anotadas armazenam metadados extras, como: o nome do tagger, e-mail e data. Este é um dado importante para um lançamento público. Tags leves são essencialmente 'marcadores' para um commit, são apenas um nome e um ponteiro para um commit, úteis para criar links rápidos para commits relevantes.

-Tags Anotadas<p>
As tags anotadas são armazenadas como objetos completos no banco de dados Git.
Semelhante a commits e mensagens de commit as *tags anotadas* possuem uma mensagem de marcação. Além disso, por questões de segurança, as *tags anotadas* podem ser assinadas e verificadas com o *GNU Privacy Guard* (GPG). As práticas recomendadas sugeridas para a marcação do git são preferir tags anotadas em vez de leves para que você possa ter todos os metadados associados.<p>
A execução do comando abaixo criará uma nova *tag anotada* identificada com v1.4. O comando abrirá o editor de texto padrão configurado para solicitar mais entradas de metadados.<p>
- ``` git tag -a v1.4  ```

A execução do comando abaixo é semelhante à chamada anterior, no entanto, esta versão do comando recebe a opção -m (mensagem). Este é um método semelhante ao comando *git commit -m* que criará imediatamente uma nova tag e abrirá o editor de texto local para que seja possível salvar a mensagem passada com a opção *-m*.
- ``` git tag -a v1.4 -m "my version 1.4"  ```

-Tags Leves<p>
A execução do comando abaixo cria uma *tag leve* identificada como v1.4-lw. *Tags leves* são criadas com a ausência das opções -a, -s ou -m.<p>
- ``` git tag v1.4-lw  ```

-Listando Tags<p>
Para listar as tags armazenadas em um repositório, execute o seguinte:
- ``` git tag  ```

Para refinar a lista de tags, a opção '-l' pode ser passada com uma expressão curinga:
- ``` git tag -l *-rc*  ```

#### git blame<p>
O comando *git blame* é usado para explorar o histórico de código específico e responder a perguntas sobre o quê, como e por que o código foi adicionado a um repositório.<p>
A execução do comando abaixo nos dará nossa primeira amostra de saída:
- ``` git blame README.MD  ```

![3](https://user-images.githubusercontent.com/45216757/153676274-aeb2821c-fd9e-460b-abd7-48099ccb6cc8.png)

#### git log<p>
O comando *git log* permite listar o histórico do projeto, filtrá-lo e pesquisar alterações específicas.
- ``` git log  ```
 
Lista quais arquivos são staged, unstaged e untracked.

## Desfazendo confirmações e alterações
É importante notar que o *Git* não possui um sistema tradicional de 'desfazer' como os encontrados em um aplicativo de processamento de texto (Microsoft Word, por exemplo). Além disso, o *Git* tem sua própria nomenclatura para operações de 'desfazer'. Essa nomenclatura inclui termos como reset, revert, checkout, clean, e muito mais.<p>
Ao 'desfazer' no Git, você geralmente está voltando no tempo ou para outra linha do tempo onde os erros ainda não aconteceram.

Uma metáfora divertida é pensar no Git como um utilitário de gerenciamento de linha do tempo. Commits são snapshots instantâneos de um ponto no tempo ou pontos de interesse ao longo da linha do tempo. Além disso, várias linhas do tempo podem ser gerenciadas por meio do uso de branches. Ao 'desfazer' no Git, você geralmente está voltando no tempo ou para outra linha do tempo onde os erros não aconteceram.

#### Encontrando o que está perdido: revisando commits antigos
A ideia por trás de qualquer sistema de controle de versão é armazenar cópias “seguras” de um projeto. Depois de criar um histórico de commits do projeto, você pode revisar e revisitar qualquer commit no histórico. Um dos melhores utilitários para revisar o histórico de um repositório Git é o comando *git log*.

No exemplo abaixo, usamos git logpara obter uma lista dos commits mais recentes:
![1](https://user-images.githubusercontent.com/45216757/154678780-6a4b34cf-93a4-4c9b-be87-7acda784865b.jpg)

Cada *commit* tem um hash de identificação (SHA-1 - função hash criptográfica) exclusivo. Esses IDs são usados para percorrer a linha do tempo confirmada e revisitar os commits.
Por padrão, o comando *git log* só mostrará commits para o branch selecionado no momento. É perfeitamente possível que o commit que você está procurando esteja em outro branch. Você pode visualizar todos os commits em todas as ramificações executando *git log --branches=* *.
