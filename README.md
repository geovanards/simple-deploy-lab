# 🚀 Projeto com GitHub Actions + Docker

Este repositório demonstra uma configuração simples de **CI/CD** utilizando **GitHub Actions**, junto com um ambiente básico usando **Docker**.

---

## 📦 Estrutura do Projeto

```
📦 projeto
┣ 📂 .github
┃ ┗ 📂 workflows
┃   ┗ 📄 CD.yml
┣ 📄 Dockerfile
┣ 📄 index.html
┗ 📄 README.md
```

---

## ⚙️ Tecnologias Utilizadas

* GitHub Actions (CI/CD)
* Docker
* HTML

---

## 🔄 Workflow (CI/CD)

O workflow localizado em:

```
.github/workflows/CD.yml
```

é responsável por:

* Executar automações sempre que houver:

  * Push na branch `main`
* Rodar processos de build
* Simular um pipeline de deploy (Render ou outro serviço)

---

## 🐳 Docker

O arquivo `Dockerfile` define o ambiente da aplicação.

Exemplo do que ele pode fazer:

* Criar uma imagem do projeto
* Servir o `index.html`
* Preparar para deploy em produção

---

## 🌐 Aplicação

O arquivo principal da aplicação é:

```
index.html
```

Este arquivo pode ser usado como base para testes de deploy contínuo.

---

## 📊 Execuções do Workflow

Você pode acompanhar as execuções em:

* Aba **Actions** do repositório no GitHub

Exemplo:

* ✅ Update README.md
* ✅ new

Cada execução mostra:

* Status da pipeline
* Tempo de execução
* Commit relacionado

---

## ▶️ Como usar

1. Clone o repositório:

```bash
git clone <url-do-repositorio>
```

2. Entre na pasta:

```bash
cd nome-do-projeto
```

3. (Opcional) Rode com Docker:

```bash
docker build -t meu-projeto .
docker run -p 8080:80 meu-projeto
```

---

## 📌 Objetivo

Este projeto serve como:

* Exemplo de pipeline CI/CD
* Teste inicial com GitHub Actions
* Base para deploy automatizado
