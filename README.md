Fico feliz que tenha dado certo! Vamos criar um `README.md` para documentar o que foi feito até agora, incluindo os requisitos adicionados.

Aqui está um modelo que você pode usar para o seu projeto:

---

# Doorstop - Requisitos do Sistema

Este repositório contém os requisitos do sistema para o projeto, que utiliza o **Doorstop** como ferramenta para gerenciar os requisitos.

## O que foi feito

* **Criação de um novo projeto de requisitos** usando o **Doorstop**.
* **Adição de dois requisitos** para o sistema de simulação, com **requisitos pai e filho**.
* **Configuração do GitHub para controle de versão**, incluindo autenticação via **Token de Acesso Pessoal (PAT)**.

## Estrutura do Repositório

A estrutura do projeto foi configurada da seguinte maneira:

```
/
├── reqs/
│   └── sim/
│       ├── REQ001.yml
│       └── REQ002.yml
├── .gitignore
└── README.md
```

* O diretório `reqs/sim/` contém os arquivos YAML que definem os requisitos do sistema.
* `SIM001.yml` e `SIM-1.yml` são os arquivos de requisitos.

---

## Requisitos Adicionados

### Requisito 1: **REQ001**

**Descrição:**

O sistema deve disponibilizar informações filtradas conforme o grupo de usuário, garantindo que cada perfil (Operacional, Tecnologia, Governança/Compliance) visualize apenas os dados previamente definidos como relevantes para suas funções.

**Detalhes:**

* **Header:** Adequação das Informações por Grupo de Usuários
* **Level:** 1.0
* **Normativo:** `true`
* **Referência:** (não especificada)
* **Revisado:** `true`
* **Texto:**

```
O sistema deve disponibilizar informações filtradas conforme o grupo de usuário, garantindo que cada perfil (Operacional, Tecnologia, Governança/Compliance) visualize apenas os dados previamente definidos como relevantes para suas funções. A definição de quais informações pertencem a cada grupo deve seguir a matriz de perfis aprovada pela organização.
```

### Requisito 2: **REQ002**

**Descrição:**

O sistema deve disponibilizar uma visualização geoespacial em mapa interativo, atualizada em tempo real, que exiba obrigatoriamente: posições de aeronaves, posição de drones, as restrições de uso de espaço, as áreas solicitadas e os demais objetos definidos no cenário da simulação.

**Detalhes:**

* **Header:** Visualização Geoespacial
* **Level:** 2.0
* **Normativo:** `true`
* **Referência:** (não especificada)
* **Revisado:** `true`
* **Texto:**

```
O sistema deve disponibilizar uma visualização geoespacial em mapa interativo, atualizada em tempo real, que exiba obrigatoriamente: posições de aeronaves, posição de drones, as restrições de uso de espaço, as áreas solicitadas e os demais objetos definidos no cenário da simulação. A visualização deve refletir o estado atual da simulação conforme os dados produzidos pelo motor de simulação e deve permitir que gestores, operadores e analistas acompanhem a execução para fins de conscientização situacional.
```

---

## Configuração do GitHub

### Autenticação no GitHub

Para interagir com o repositório, foi configurado o **Token de Acesso Pessoal (PAT)**, que substitui a autenticação por senha. Esse token foi configurado para que o Git não peça as credenciais repetidamente.

#### Passos para configurar a autenticação com o Token:

1. Gerar um Token de Acesso Pessoal no GitHub com a permissão `repo`.
2. Configurar o Git para armazenar as credenciais de forma segura, utilizando o helper `store` ou `cache`.
3. Quando o Git pedir a senha, fornecer o **Token de Acesso Pessoal** gerado no GitHub.

---

## Comandos Git Utilizados

Durante o processo, os seguintes comandos Git foram usados:

1. **Criação de uma nova branch**:

   ```bash
   git checkout -b feat/REQ-SIM-1
   ```

2. **Adicionar, commit e push de mudanças**:

   ```bash
   git add .
   git commit -m "Adicionando requisitos SIM001 e SIM002"
   git push -u origin feat/REQ-SIM-1
   ```

3. **Configuração do repositório remoto (caso necessário)**:

   ```bash
   git remote set-url origin https://github.com/clubfullstack/recs_sac.git
   ```

4. **Configuração de usuário e email no Git**:

   ```bash
   git config --global user.name "clubfullstack"
   git config --global user.email "seu-email@dominio.com"
   ```

---

## Próximos Passos

* Continuar adicionando requisitos conforme o progresso do projeto.
* Manter o controle de versão e os requisitos organizados no repositório.

---
