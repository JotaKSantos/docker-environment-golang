
# Ambiente para Desenvolvimento em Go (GoLang)

Ambiente para desenvolver em GO (GoLang) utilizando Docker, WSL2 e VSCode com as extensões necessárias e compartilhando as chaves **gpg** e **ssh** para assina e dar push nos commits

## Iniciando

Essas instruções fornecerão a você uma cópia do projeto em execução em sua máquina local para fins de desenvolvimento e teste.

  

## Pré-requisitos

O que você precisa ter instalado.

* Git.
* Docker.
* WSL2.
* VSCode com a Extensão: [Dev Containers](https://aka.ms/vscode-remote/download/extension)
* Software para GPG no Windows. Veja como [instalar aqui](https://www.youtube.com/watch?v=5IPrjAEqfQ0&t=1252s)
  

## Instalando
Clone o repositório git no seu computador

```
$ git clone https://github.com/JotaKSantos/docker-environment-golang.git
```

Acesse o diretório onde fez o clone e inicie o VSCode

```
cd docker-environment-golang
code .
```
### Assim que o VSCode abrir ele irá reconhecer o projeto e vai sugerir abrir o projeto direto no container.

![](https://github.com/JotaKSantos/docker-environment-golang/blob/main/.docker//imgs/reopen-in-container.jpg)

### Instale as dependências da extensão do GO
![](https://github.com/JotaKSantos/docker-environment-golang/blob/main/.docker//imgs/install-extension-dependencies.jpg)

### Espere até que todas as dependências tenham sido instaladas
![](https://github.com/JotaKSantos/docker-environment-golang/blob/main/.docker//imgs/install-extension-dependencies-succeeded.jpg)

### Assim que terminar as pastas **bin** e **pkg** deverão ter sido criadas
![](https://github.com/JotaKSantos/docker-environment-golang/blob/main/.docker//imgs/install-extension-dependencies-finished.jpg)


## Referências

* ### [Windows + WSL = Ambiente perfeito de desenvolvimento](https://www.youtube.com/watch?v=bniD6dehPCQ)
* ### [Assinatura de commits no Remote Container do VSCode](https://www.youtube.com/watch?v=5IPrjAEqfQ0)
* ### [Software para GPG no Windows](https://www.gpg4win.org/)