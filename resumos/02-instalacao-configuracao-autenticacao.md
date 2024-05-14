## Instalação, Configuração e Autenticação

### Instalando no Windows

- Acesse a [página de download do git]( https://git-scm.com/download/win);
- Baixe e execute o instalador;
- Aceite a licença de uso;
- Configure como desejar e clique em "next" para os próximos passos;
- Finalize clicando em "install"

OBS: Deixe as opções "GitBash Here" e "Git GUI" selecionadas em "select components".

### Instalando no Linux

- Siga aas intuções da documentação [https://git-scm.com/book/en/v2/Getting-Started-Installing-Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git);
- `add-apt-repository ppa:git-core/pp`
- `apt update`
- `apt install git`

### Configurando o Git

| Comando               | Descrição |
|-----------------------|-----------|
| ```$ git config --list```    | Lista todas as configurações que estão definidas no Git|
| ```$ git config --global user.name "Nome Sobrenome"``` | Configura globalmente um nome de usuário |
| ```$ git config --global user.email usuario@email.com``` | configura globalmente um e-mail de usuário |
| ```$ git config --global init.defaultBranch main``` | Configura o nome da branch padrão |

### Autenticação via Token

- Acesse a conta do GitHub;
- Abra a aba "Settings";
- Clique em "Developr settings";
- Abra a aba "Personal acess tokens" e selecione a opção "tokens (classic)";
- Clique em "Generate new token";
- Selecione a ultima opção;
- Insira as configurações do token: nome, duração, escopo, etc.

Para salvar as credenciais  do token siga as seguintes isntruções: 

```$ git config credential.helper store ```

- Informe a senha e nome de usuário;
- Digite o token.

Para visualizar as credenciais:

 ```$ git config --show-origin credential.helper```

### Autenticação Via SSH

- Acesse "Settings";
- Em "Acess", escolha a opção "SSH and GPG Keys";
- Verifique se há chaves existentes: 
  - ```ls -al ~/.ssh```
- Clique em "Gerar uma nova chave SSH":
  - ```ssh-keigen -t ed25519 -C "email@example.com"```
  - Insira o caminho da chave no terminal
  - Digite uma senha
- Adicionar o ssh agent:
  - ```eval "$(ssh-agent -s)"```
  - ```ssh-add ~/.ssh/id_ed25519```
- No No GitHub, em "SSH and GPG Keys", clique em "New SSH Key"
- Adicione um título;
- Selecione o tipo: autenticação ou assinatura;
- Copie e cole a chave pública:
  - ```cd ~/.ssh```
  - ```cat id_ed25519.pub

