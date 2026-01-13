# ex03 — Criando e entregando a chave SSH

Este exercício tem como objetivo configurar uma chave SSH para permitir o envio do repositório para o servidor Git da 42.

---

## 1. Verificar se já existe alguma chave SSH no computador

Antes de criar uma nova chave, verifique se já existe alguma salva.

Abra o terminal e execute:

```bash
ls ~/.ssh

## 2. Se não houver, crie uma nova.

```bash
ssh-keygen -t rsa -b 4096


#### obs: 
#####id_rsa → chave privada
####id_rsa.pub → chave pública

## 3. Criar o arquivo exigido pela 42 no exercício
### Mostre o conteúdo da chave pública:

```bash
cat ~/.ssh/id_rsa.pub

## 4. Criar o arquivo id_rsa_pub

## 5. Colar somente a chave pública dentro do arquivo

## 6. Atualizar a chave na intranet da 42

### Passos gerais:
#### Entrar na intranet da 42
#### Perfil → SSH Keys
#### Colar a mesma chave pública
#### Salvar

## 7. Testar se funciona

```bash
ssh -T git@vogsphere.42sp.org.br

#### Se aparecer algo como:

```bash
Welcome to Git, <seu_login>!
