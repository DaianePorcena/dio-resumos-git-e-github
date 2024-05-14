## Primeiros Passos com Git e GitHub

### Criando e Clonado Repositórios

Há duas forma de adquirir um repositório Git em um  dispositivo:

1 - Convertendo um diretório loca não versionado em um repositório Git;
2 - Clonando um repositório Git existente

#### Criando um Repositório Local

- Acesse a pasta do repositório local
- Inicialize um repositório Git:

  ``` 
  $ git init
  ```
- Adicine o repositório local a um repositório remoto:

  ```
    $ git remote add origin https://github.com/username/nome-do-repositorio.git
  ```

#### Clonando um repositório remoto 

- Acesse a pasta em que deseja salvar o repositório remoto;
- Clone o repositório:

   ```
    $ git clone origin https://github.com/username/nome-do-repositorio.git
  ``` 



### Desfazendo Alterações 

| Comando | Descrição                         |
|---------|-----------------------------------|
| ```rm -rf .git``` | Exclui recursivamente um repositório .git |
| ```git restore <arquivo>``` | Descarta mudanças feitas na área de trabalho |
| ```git commit --amend -m "nova mensage"``` | Altera a mensagem de commit sem abrir o editor |
| ```git reset``` | Reseta commits |
| ```git reset soft``` | Pega commits posteriores ao indicado com a hash e adiciona a "stage area" |
| ```git reset mixed``` | Pega commits posteriores ao ao indicado com a hash e adiciona a stage area indicando como "untracked" |
| ```git reset hard``` | Apaga todos os arquivos do commit anterior |


### Trabalhando com Branches

As braches são ramificações do projeto:

- É como um ponteirio móvel para o commit no hitórico do repositório;

Uma branch (ou ramificação) em sistemas de controle de versão permite que desenvolvedores criem uma cópia separada do código-fonte para trabalhar de forma isolada, facilitando o desenvolvimento paralelo, a experimentação e a implementação de novas funcionalidades.

#### Características de uma Branch:

- **Isolamento:** Mudanças em uma branch não afetam outras branches.
- **Fusão (Merge):** O trabalho concluído pode ser mesclado de volta à branch principal.
- **Histórico Independente:** Cada branch possui seu próprio histórico de commits.
- **Nomeação:** Branches são nomeadas conforme seu propósito, como feature/nova-funcionalidade, bugfix/corrigir-bug, ou release/v1.0.

#### Exemplos de Uso:

- **Desenvolvimento de Funcionalidades:** Criar uma branch para novas funcionalidades sem interferir na branch principal.
- **Correção de Bugs:** Criar uma branch específica para corrigir bugs, testando a correção separadamente.
- **Lançamentos:** Manter branches separadas para diferentes versões do software, facilitando manutenção e suporte.
