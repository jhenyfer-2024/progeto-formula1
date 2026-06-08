<div align="center">



# 🏎️ FORMULA 1 API

<p>
API REST desenvolvida com <strong>Fastify</strong> e <strong>TypeScript</strong> para gerenciamento e consulta de equipes e pilotos da Fórmula 1.
</p>

</div>

<br>

<div align="center">

![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue.svg)
![Node.js](https://img.shields.io/badge/Node.js-20+-green.svg)
![Fastify](https://img.shields.io/badge/Fastify-5.x-black.svg)

</div>

---

# 🚀 Tecnologias

Este projeto foi desenvolvido utilizando:

- TypeScript
- Fastify
- @fastify/cors
- Node.js
- TSX

---

# 📋 Funcionalidades

### Equipes

- Listar todas as equipes
- Buscar equipe por ID

### Pilotos

- Listar todos os pilotos
- Buscar piloto por ID

### Recursos Extras

- Respostas em JSON
- Tratamento de erros
- Estrutura REST
- Suporte a CORS

---

# 📂 Estrutura das Rotas

## Equipes

### Listar Equipes

```http
GET /api/teams
```

### Buscar Equipe por ID

```http
GET /api/teams/:id
```

Exemplo:

```http
GET /api/teams/1
```

Resposta:

```json
{
  "id": 1,
  "name": "McLaren",
  "country": "United Kingdom"
}
```

---

## Pilotos

### Listar Pilotos

```http
GET /api/drivers
```

### Buscar Piloto por ID

```http
GET /api/drivers/:id
```

Exemplo:

```http
GET /api/drivers/3
```

Resposta:

```json
{
  "id": 3,
  "name": "Lando Norris",
  "number": 4,
  "teamId": 1
}
```

---

# 📦 Estrutura das Respostas

### Listagem

```json
{
  "total": 3,
  "data": []
}
```

### Registro Único

```json
{
  "id": 1,
  "name": "Max Verstappen",
  "number": 1,
  "teamId": 3
}
```

### Erro 404

```json
{
  "error": "Piloto não encontrado"
}
```

---

# ⚙️ Como Executar

Clone o repositório:

```bash
git clone https://github.com/seu-usuario/formula1-api.git
```

Entre na pasta:

```bash
cd formula1-api
```

Instale as dependências:

```bash
npm install
```

Execute o projeto:

```bash
npm run dev
```

Servidor disponível em:

```bash
http://localhost:3333
```

---

# 🔥 Melhorias Implementadas

- Prefixo `/api` nas rotas
- Busca individual de equipes
- Busca individual de pilotos
- Correção de IDs duplicados
- Relacionamento através de `teamId`
- Respostas padronizadas
- Tratamento de erros HTTP 404
- Estrutura mais próxima de APIs reais

---

# 📁 Estrutura do Projeto

```bash
src/
│
├── server.ts
│
├── routes/
│
├── controllers/
│
└── data/
```

---

# 👨‍💻 Autor

Projeto desenvolvido para fins de estudo utilizando Fastify e TypeScript.

---

# 📜 Licença

Este projeto está disponível para uso educacional e estudos.
