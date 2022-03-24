# **Resumo Git/GitHub**
Aqui vou resumir o que aprendi sobre Git e GitHub.

## **Git**
Git é um sistema de versionamento de código ou controle de versão, ou seja, por ele você pode ter um controle sobre as modificações do seu projeto. Desta maneira, é possível que várias pessoas colaborem em um projeto, porém sem precisarem ficar baixando milhares de versões do mesmo e sem se perderem de qual é a versão mais recente.

### **Como o Git controla as versões**
Resumindo superficialmente a maneira como ele faz isso: para cada **blob**, **tree** e **commit** ele gera um SHA (Secure Hash Algorithms) que é um código criptografado, gerado com base no conteúdo.

Explicando o que são **blob**, **tree** e **commit**:

**blob**: pode ser qualquer arquivo em um diretório.

**tree**: pode ser qualquer diretório.

**commit**: é o que engloba todas as **trees** e **blobs**.

O dono do projeto consegue ver se houve alteração no projeto pois o GIT aponta quais arquivos foram alterados quando o status do repositório é consultado. Isso acontece porque quando um arquivo (**blob**) é alterado, seu SHA muda e assim o SHA do diretório (**tree**) muda também, e quando o projeto for "commitado" novamente, o SHA do **commit** será diferente do SHA do seu parente (**commit** anterior).

### **Estado dos arquivos**
Quando um arquivo é adicionado em um repositório, inicialmente ele fica no estado "Untracked" (não rastreado), ou seja, o git não está rastreando qualquer mudança que ocorra nele, para que ele passe a ser rastreado, devemos usar o comando **git add**, assim ele passará para o estado "staged" (pronto) neste estado já podemos fazer o **commit** e ele passará para o estado "Unmodified" (não modificado) até que seja modificado e passe para o estado (Modified) e seja precise ser movido para "staged" novamente para fazer o commit, repetindo sempre este ciclo. **OBS: um repositório só pode ser empurrado se estiver totalmente em commit.**

### **Alguns comandos básicos para usar o Git**
- **git init:** Começa um repositório no diretório onde se está no momento da execução
- **git config:** Configurar o repositório
- **git status:** Confere o status do repositório
- **git add:** Move o arquivo de "untracked" para "staged"
- **git commit:** "Commita" o repositório
- **git push origin master:** Empurra para o repositório para o GitHub
- **git pull origin master:** Extrai as alterações contidas na cópia online e junta com o repositório local


## **GitHub**
Como o próprio nome já diz, é um "Hub" para Git, ou seja , uma central de hospedagem de arquivos de controle de versão. No GitHub várias empresas procuram novos talentos, e vários devs se ajudam em prol de algum projeto com a ajuda do sistema de versionamento Git.

