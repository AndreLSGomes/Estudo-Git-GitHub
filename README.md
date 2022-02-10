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

2. Ao iniciar o instalador, você deverá ver a tela do assistente de configuração do Git . Siga os prompts Avançar e Concluir para concluir a instalação.

3. Abra um prompt de comando e faça:
- ``` $ git config --global user.name "Emma Paris" ```
- ``` $ git config --global user.email "eparis@atlassian.com" ```

## Instalando o Git no Linux
1. Debian / Ubuntu (apt-get): Os pacotes Git estão disponíveis via apt (https://wiki.debian.org/Apt)

2. Do seu shell, instale o Git usando apt-get:
- $ sudo apt-get update  ``` 
- $ sudo apt-get install git  ``` 

3. Verifique se a instalação foi bem-sucedida digitando git --version:
- ``` $ git --version ``` 
- ``` git version 2.9.2  ``` 

3. Configure seu nome de usuário e e-mail do Git usando os comandos a seguir, substituindo o nome de Emma pelo seu. Esses detalhes serão associados a qualquer commit que você criar:

- ``` $ git config --global user.name "Emma Paris"  ``` 
- ``` $ git config --global user.email "eparis@atlassian.com"  ``` 
