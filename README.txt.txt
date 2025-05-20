layane valerio da luz 

Criação de um repositório remoto no GitHub: Este será o seu ponto central para armazenar e colaborar no projeto.
Clonagem para o ambiente local: Você trará o repositório remoto para a sua máquina, onde poderá realizar modificações.
Organização do projeto: Criará uma estrutura de diretórios e arquivos simulando um projeto simples.
Ignorar arquivos: Aprenderá a configurar o Git para não rastrear arquivos específicos, como arquivos de log.
Adicionar e commitar alterações: Você preparará e registrará as suas modificações no histórico do Git.
Enviar alterações para o repositório remoto: Publicará suas alterações locais no GitHub.
Gerenciamento de branches: Criará e alternará entre branches para isolar o desenvolvimento de novas funcionalidades.
Mesclagem de branches: Integrará as alterações feitas em uma branch de desenvolvimento de volta à branch principal (main).
Documentação do processo: Você registrará cada comando Git utilizado e capturará printscreens de cada etapa, reforçando a compreensão do que está acontecendo em cada momento.


git add <arquivo(s)>:

Funcionalidade: Adiciona as alterações feitas no(s) arquivo(s) especificado(s) à área de staging. A área de staging é como uma "preparação" para o seu próximo commit. Você informa ao Git quais modificações você quer incluir no próximo instantâneo do seu projeto.
Exemplo:
git add index.html: Adiciona o arquivo index.html ao staging.
git add .: Adiciona todas as alterações (arquivos novos, modificados e excluídos) no diretório atual e subdiretórios ao staging.
git add *.txt: Adiciona todos os arquivos com a extensão .txt ao staging.
git commit -m "<mensagem>":

Funcionalidade: Registra as alterações que estão na área de staging em um commit. Um commit é como um "ponto de salvamento" no histórico do seu projeto. A mensagem que você fornece com -m descreve as alterações que foram incluídas neste commit. Boas mensagens de commit são cruciais para entender o histórico do projeto.
Exemplo:
git commit -m "Adiciona a estrutura básica da página inicial": Cria um novo commit com a mensagem especificada.
git push <remoto> <branch>:

Funcionalidade: Envia os commits do seu repositório local para um repositório remoto. Um repositório remoto é uma versão do seu projeto que está hospedada em um servidor (como o GitHub, GitLab, Bitbucket, etc.). <remoto> geralmente é origin (o nome padrão dado ao repositório remoto quando você clona um repositório), e <branch> é o nome da branch que você quer enviar (geralmente main ou master).
Exemplo:
git push origin main: Envia os commits da sua branch local main para a branch main do repositório remoto chamado origin.
git branch <nome_da_branch>:

Funcionalidade: Cria uma nova branch no seu repositório local. Uma branch é uma linha de desenvolvimento separada. Isso permite que você trabalhe em novas funcionalidades ou correções de bugs isoladamente, sem afetar a branch principal (geralmente main).
Exemplo:
git branch desenvolvimento: Cria uma nova branch chamada desenvolvimento.
git checkout <nome_da_branch>:

Funcionalidade: Muda a sua branch ativa para a branch especificada. Isso significa que os arquivos no seu diretório de trabalho serão alterados para corresponder ao estado da branch para a qual você está mudando.
Exemplo:
git checkout desenvolvimento: Muda para a branch desenvolvimento.
git checkout main: Volta para a branch main.
git checkout -b <nova_branch>: Cria uma nova branch com o nome especificado e já muda para ela (combinação de git branch e git checkout).
git merge <branch_a_ser_mergeada>:

Funcionalidade: Integra as alterações de uma branch especificada para a branch atualmente ativa. Isso é usado para combinar o trabalho feito em branches separadas.
Exemplo:
Estando na branch main, git merge desenvolvimento incorporaria as alterações da branch desenvolvimento na branch main. Se houver conflitos (alterações na mesma linha de código em ambas as branches), você precisará resolvê-los manualmente.