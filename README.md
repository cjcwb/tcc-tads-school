# TADS School

Bem-vindo ao TADS School! Este projeto foi desenvolvido para auxiliar na gestão de ocorrências, alunos, turmas e demais funcionalidades associadas ao ambiente escolar.

## Sobre o Projeto

O TADS School é uma aplicação web que utiliza Node.js, Next.js e Prisma para gerenciar dados de alunos, turmas e ocorrências de forma simples e interativa. Além disso, oferece recursos de autenticação, análise de dados e histórico de mudanças.

## Pré-Requisitos

- **Windows 10 ou superior** (para usar o script `.bat` e `winget`)
- Acesso à internet para instalar dependências
- **Git (opcional)** caso queira clonar o repositório diretamente

O script contido em `tads-school.bat` irá garantir a instalação do Node.js (caso não esteja instalado) e realizar as configurações iniciais do projeto.

## Iniciando o Projeto

1. **Baixar o Projeto**  
   Faça o download do código-fonte ou clone o repositório.

2. **Iniciar o Script de Instalação**  
   Localize o arquivo `tads-school.bat` na raiz do projeto.

3. **Executar o `tads-school.bat` e `populate.bat` ou `populateAdminOnly.bat`**  
   Dê um duplo clique no `tads-school.bat` ou execute-o via prompt de comando (CMD).  
   
   Este script irá:
   - Verificar se o Node.js está instalado. Caso contrário, instalará automaticamente via winget.
   - Instalar as dependências do projeto executando `npm install`.
   - Executar o `prisma generate` para gerar os artefatos do Prisma.
   - Iniciar o servidor de desenvolvimento com `npm run dev`.
   - Abrir automaticamente o navegador na página de login da aplicação (`http://localhost:3000/auth/login`).

## Fluxo do Script

- **Verificação do Node.js:**  
  O script checa se o Node.js está instalado. Se não estiver, utiliza o winget para fazer a instalação silenciosa.

- **Instalação das Dependências:**  
  Com o Node.js instalado, o script executa `npm install` para instalar todas as dependências listadas no `package.json`.

- **Prisma Generate:**  
  Após a instalação das dependências, o script roda `npx prisma generate` para garantir que todos os artefatos do Prisma (tipos, cliente, etc.) estejam atualizados.

- **Início do Servidor e Navegador:**  
  Ao final, o servidor de desenvolvimento é iniciado. Após aguardar alguns segundos, o script abre o navegador na página de login da aplicação, permitindo que você acesse diretamente o sistema.

## Acesso ao Sistema

- URL padrão: [http://localhost:3000/auth/login](http://localhost:3000/auth/login)
- User padrao: `admin : admin`
- Certifique-se de ter o servidor rodando para acessar a interface.

## Dicas

- Caso queira parar o servidor, basta fechar a janela do terminal onde o `npm run dev` está rodando.
- Para rodar novamente, basta executar novamente o `tads-school.bat`.
- Caso ocorram erros, verifique o console do terminal para detalhes sobre o que pode ter dado errado.

## Contribuições e Suporte

- Sinta-se à vontade para customizar o projeto conforme suas necessidades.
- Em caso de problemas, verifique os logs no terminal e o navegador.

Obrigado por utilizar o TADS School!
