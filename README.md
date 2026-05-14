# Consultador de CPF via API 🔍

Este projeto é uma ferramenta desenvolvida para automatizar a validação e consulta de informações cadastrais de CPFs, integrando-se de forma segura a uma API externa de dados.

## 🚀 Funcionalidades

* **Consulta em Tempo Real:** Conexão direta com API para buscar dados cadastrais atualizados.
* **Validação de Formato:** Tratamento prévio de strings para garantir o envio do CPF no formato correto.
* **Tratamento de Erros:** Sistema preparado para identificar CPFs inválidos, inexistentes ou falhas de conexão.
* **Segurança:** Estrutura configurada para ocultar chaves de API sensíveis utilizando variáveis de ambiente.

## 🛠️ Tecnologias Utilizadas

* **Python 3** (ou a linguagem utilizada no seu projeto)
* **Requests** (Biblioteca para consumo e requisições HTTP da API)
* **Python-dotenv** (Gerenciamento seguro de credenciais e tokens)

## 📦 Como Instalar e Rodar o Projeto

### Pré-requisitos
* Python instalado na máquina.
* Uma chave de acesso (Token/API Key) da API de consulta utilizada.

### 1. Clonar o repositório
```bash
git clone https://github.com
cd nome-do-seu-repositorio
```

### 2. Instalar as dependências
```bash
pip install requests python-dotenv
```

### 3. Configurar as credenciais
Crie um arquivo chamado `.env` na raiz do projeto e adicione a sua chave da API:
```env
API_KEY=sua_chave_secreta_aqui
API_URL=https://exemplo.com
```

### 4. Executar a aplicação
```bash
python main.py
```

## 📝 Exemplo de Retorno (JSON)

Ao realizar uma consulta válida, o programa retorna os dados estruturados da seguinte forma:

```json
{
  "status": "regular",
  "nome": "Fulano de Tal",
  "data_nascimento": "01/01/1990"
}
```

## ✒️ Autor

* **[Marcelo Rodrigues]**
