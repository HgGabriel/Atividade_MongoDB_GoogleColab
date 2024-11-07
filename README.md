# Atividade Extra MongoDB Atlas - Google Colab 🗂️💻

## Tabela de Conteúdos 📑

- [Objetivo da Atividade 🎯](#objetivo-da-atividade)
- [Tema Escolhido 🎮](#tema-escolhido)
- [Estrutura do Projeto 🏗️](#estrutura-do-projeto)
  - [Coleta e Estruturação dos Dados 📊](#coleta-e-estruturação-dos-dados)
  - [Configuração do MongoDB Atlas 🗄️](#configuração-do-mongodb-atlas)
  - [Desenvolvimento no Google Colab 🧑‍💻](#desenvolvimento-no-google-colab)
  - [Documentação 📚](#documentação)
- [Como Reproduzir o Projeto 🔄](#como-reproduzir-o-projeto)
- [Tecnologias Utilizadas 🛠️](#tecnologias-utilizadas)
- [Estrutura de Dados 📂](#estrutura-de-dados)
- [Conclusão ✅](#conclusão)

---

## Objetivo da Atividade 🎯

Este projeto faz parte da disciplina *IBD-016 – Banco de Dados Não Relacional*, ministrada pelo Prof. Anderson Silva Vanin no curso de Desenvolvimento de Software Multiplataforma. O objetivo principal é construir e analisar uma base de dados no MongoDB utilizando a integração com o Google Colab e Python. A atividade requer que o aluno crie um banco de dados com informações coletadas da internet, realize operações de inserção, consulta, atualização e exclusão, e documente todo o processo.

---

## Tema Escolhido 🎮

Para esta atividade, escolhi o tema **Jogos de PS5**. Os dados foram coletados de fontes públicas na internet e incluem informações relevantes como título, desenvolvedor, publicador, data de lançamento, gêneros e plataforma.

---

## Estrutura do Projeto 🏗️

### Coleta e Estruturação dos Dados 📊

- Realizei uma pesquisa na internet para coletar dados de jogos de PS5. 
- Foram reunidos pelo menos 20 registros, cada um com os seguintes campos:
  - `title`: Título do jogo
  - `developer`: Desenvolvedor do jogo
  - `publisher`: Publicador do jogo
  - `release_date`: Data de lançamento
  - `genre`: Gêneros do jogo
  - `platform`: Plataforma (PS5)

### Configuração do MongoDB Atlas 🗄️

- Configurei um cluster gratuito no [MongoDB Atlas](https://www.mongodb.com/cloud/atlas).
- Criei uma base de dados e uma coleção para armazenar os registros de jogos de PS5.

### Desenvolvimento no Google Colab 🧑‍💻

- Utilizei a biblioteca `pymongo` para realizar a conexão com o MongoDB Atlas.
- Criei um script em Python que realiza as seguintes operações:
  - **Inserção de Dados**: Inserí os documentos coletados na coleção.
  - **Consultas**: Filtrei dados específicos, como jogos de um gênero específico ou desenvolvidos por uma empresa específica.
  - **Atualizações**: Implementei operações de atualização, como a modificação de campos existentes e a adição de novos campos.
  - **Exclusões**: Implementei operações de exclusão, removendo documentos com base em critérios específicos.

### Documentação 📚

- Todas as etapas foram explicadas em células Markdown no notebook do Google Colab, facilitando o entendimento do processo.
- Comentários foram adicionados ao código para maior clareza.

---

## Como Reproduzir o Projeto 🔄

1. **Clonar o Repositório** 🖥️

   Clone o repositório para sua máquina local:

   ```bash
   git clone https://github.com/seu-usuario/Atividade_MongoDB_GoogleColab.git
   ```

2. **Abrir o Notebook no Google Colab** 🌐

   - Faça upload do arquivo `.ipynb` no Google Colab ou acesse diretamente via GitHub.
   - Abra o [Google Colab](https://colab.research.google.com/) e faça o upload do notebook ou insira a URL do seu repositório GitHub.

3. **Configurar a Conexão com o MongoDB Atlas** 🔑

   - No script, substitua a string de conexão pela sua URI de conexão fornecida pelo MongoDB Atlas.
   - Execute as células do notebook para inserir, consultar, atualizar e excluir dados.

---

## Tecnologias Utilizadas 🛠️

- **Python**: Linguagem de programação usada para manipular e analisar dados.
- **Google Colab**: Ambiente de desenvolvimento para execução de scripts em Python.
- **MongoDB Atlas**: Serviço de banco de dados na nuvem, usado para armazenar e gerenciar os dados.
- **pymongo**: Biblioteca Python para interagir com o MongoDB.

---

## Estrutura de Dados 📂

Cada documento na coleção contém os seguintes campos:

```json
{
  "title": "Nome do Jogo",
  "developer": "Desenvolvedor",
  "publisher": "Publicador",
  "release_date": "Data de Lançamento",
  "genre": ["Gênero1", "Gênero2"],
  "platform": "PS5"
}
```

---
