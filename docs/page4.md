# **Configurações iniciais do Git**

## Abrir o Terminal

Após a **[instalação do Git](page3.md\#instalando-o-git)** devemos acessar o **Terminal** para fazer as **configurações iniciais**. 

No **Windows** é fortemente recomendado utilizar o **GIT-BASH**, que vem com a **[instalação do Git](page3.md\#instalando-o-git)** entretanto caso prefira ainda é possível utilizar o **PowerShell** ou **CMD**, já para o **macOS** e as **Distribuições Linux** em geral, o mais comum é utilizar o próprio **Terminal**.

## Salvando as Configuração

O **[Git](page2.md\#o-que-é-o-git)** possui três maneiras de salvar as configurações feitas. São elas:

- Global: Salva no Usuário atual da máquina.
- System: Salva no sistema, ou seja, em todos os Usuários da máquina.
- Local: Salva no Repositório que o comando foi usado.

```{hl_lines="4-6" title='Entrada no Terminal: git config'}
Saida:

Config file location
    --global    use global config file
    --system    use system config file
    --local     use repository config file
...   
```

## Primeiras Configurações

As principais configurações do usuário que devemos definir são **nome** e **e-mail** do **autor** dos **commits**.

### Definindo o Nome do Autor

Para definir o **Nome** utilize o seguinte comando:

```
git config --(location) user.name "(name)" # Substituir (location) e (name).
```
> Exemplos:
    ```
    git config --global user.name "Herbert"
    ```
    ```
    git config --system user.name "Barone"
    ```
    ```
    git config --local user.name "Herbert Barone"
    ```

### Definindo o E-mail do Autor

Para definir o **E-mail** utilize o seguinte comando:

```
git config --(location) user.email (e-mail) # Substituir (location) e (e-mail).
```
> Exemplos:
    ```
    git config --global user.email baron.lord@icloud.com
    ```
    ```
    git config --system user.email herbertbar@yahoo.com
    ```
    ```
    git config --local user.email herbertdev@gmail.com
    ```

### Definindo branch padrão

Com o intuito de trazer maior **organização**, **compreensão** e **colaboração eficiente** nos projetos é **extremamente recomendado** pôr o nome da **branch** padrão como **"main"**.


Para alterar o nome da branch padrão utilize o seguinte comando:
```
git config --(location) init.defaultBranch (branch_name) # Define um novo nome para branch padrão
```
> Exemplo:
    ```{title='Entrada no Terminal: '}
    git config --global init.defaultBranch main
    ```


## Verificando Configurações

Para verificar o **Nome** utilize o seguinte comando:
```
git config user.name    # Retorna o Usuário
```
> Exemplo:
    ```{title='Entrada no Terminal: git config user.name '}
    Exemplo Saida:
        Herbert
    ```

Para verificar o **E-mail** utilize o seguinte comando:
```
git config user.email   # Retorna o E-mail
```
> Exemplo:
    ```{title='Entrada no Terminal: git config user.email '}
    Exemplo Saida:
        baron.lord@icloud.com
    ```

Para verificar o nome da **branch** padrão utilize o seguinte comando:
```
git config init.defaultBranch # Retorna a branch padrão
```
> Exemplo:
    ```{title='Entrada no Terminal: git config init.defaultBranch'}
    Exemplo Saida:
        master
    ```

Para verificar todas as **configurações**, utilize o seguinte comando:
```
git config --list # Retorna todas as configurações 
```

Também é possível verificar as **configurações** especificando onde elas foram salvas:
```
git config --(location) --list
```
> Exemplo:
```{title='Entrada no Terminal:'}
git config --global --list
```

## Tabelas com os comandos deste tópico

### Substituição

| Nome | Esperado |
|:-:|:-:|
| --(location)  | --global |
|  | --system |
|  | --local |
| (name) | Nome do Autor |
| (email) | E-mail do Autor |
| (branch_name) | Nome para a Branch |

### Comandos de Definição

| Comando | Descrição |
|:-:|:-:|
| git config --(location) user.name "(name)" | Define o Nome do Autor |
| git config --(location) user.email (email) | Define o E-mail do Autor |
| git config --(location) init.defaultBranch (branch_name) | Define o nome da Branch Padrão |

### Comandos de Verificação

| Comando | Descrição |
|:-:|:-:|
| git config user.name | Retorna o Nome do Autor |
| git config user.email | Retorna o E-mail do Autor |
| git config init.defaultBranch | Retorna o Nome da Branch Padrão |
| git config --list | Retorna todas as configurações |
| git config --(location) --list | Retorna as configurações do local especificado  |