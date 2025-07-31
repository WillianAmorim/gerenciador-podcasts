# 🎧 Podcast Manager

Um gerenciador de podcasts em vídeo ao estilo Netflix, com episódios organizados por categorias como saúde, fitness, mentalidade e humor.

## 📌 Descrição

Este projeto tem como objetivo centralizar e organizar episódios de podcasts em vídeo. A aplicação fornece uma API REST que retorna informações como o nome do podcast, nome do episódio, imagem de capa, link do episódio e categorias.

---

## 🛠 Tecnologias Utilizadas

- **Node.js** – Ambiente de execução para JavaScript no backend.
- **TypeScript** – Superset do JavaScript com tipagem estática.
- **Express** – Framework minimalista para criação de APIs REST.
- **Dotenv** – Gerenciamento de variáveis de ambiente.

---

## 🚀 Funcionalidades

- ✅ Listar episódios de podcasts organizados por categorias.
- ✅ Filtrar episódios pelo nome do podcast.
- ✅ Cada episódio contém:
  - `podcastName`: nome do podcast
  - `episodeName`: nome do episódio
  - `videoId`: ID do vídeo do YouTube
  - `cover`: imagem de capa do episódio
  - `link`: link para o episódio
  - `category`: array de categorias (ex: saúde, humor)

---

## 📂 Estrutura de Resposta da API

```json
[
  {
    "podcastName": "Nome do Podcast",
    "episodeName": "Nome do Episódio",
    "videoId": "aGsBPwMYJUM",
    "cover": "https://i.ytimg.com/vi/aGsBPwMYJUM/maxresdefault.jpg",
    "link": "https://www.youtube.com/watch?v=aGsBPwMYJUM",
    "category": ["Saúde", "Humor"]
  }
]
```
### Clone o projeto
```bash
    git clone https://github.com/WillianAmorim/gerenciador-podcasts.git
    cd gerenciador-podcasts
```

### Instale as dependências
```bash
    npm install
```

### Execute o servidor
```bash
    npm run dev
```

### Rotas da API
```plaintext
| Método | Rota                    | Descrição                            |
| ------ | ----------------------- | ------------------------------------ |
| GET    | `/podcasts`             | Retorna todos os episódios           |
| GET    | `/podcasts?filter=nome` | Filtra episódios por nome do podcast |
```

### Organização do projeto
```
src/
├── controllers/
├── routes/
├── services/
├── data/
├── types/
└── index.ts
```