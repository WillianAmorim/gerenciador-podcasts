# Podcast Manager

### Descrição
Um app ao estilo netflix, aonde possa centralizar diferentes episódios de podcasts separados por categorias.

### Domínio
Podcasts feitos em vídeo

### Features
- **Lista de Podcasts**: Listar os episódios de podcasts em sessões de categorias.
    - [saúde, fitness, mentalidade, humor]
- Filtrar episódios por nome de podcast.

## Como

### Feature: Lista de Podcasts
- **Lista de Podcasts**: Listar os episódios de podcasts em sessões de categorias.

### Como vou implementar:
  Vou retornar em uma api rest o nome do podcast, nome do episódio, imagem de capa, link, category.

  ```js 
    [
        {
            podcastName: "Nome do Podcast",
            episodeName: "Nome do Episódio",
            videoId: 'aGsBPwMYJUM'
            cover: "https://i.ytimg.com/vi/aGsBPwMYJUM/maxresdefault.jpg",
            link: "https://www.youtube.com/watch?v=aGsBPwMYJUM",
            category: ["Categoria 1", "Categoria 2"]
        },
        {
            podcastName: "Nome do Podcast",
            episodeName: "Nome do Episódio",
            videoId: 'aGsBPwMYJUM',
            cover: "URL da Imagem de Capa",
            link: "URL do Episódio",
            category: ["Categoria 1", "Categoria 2"]
        }
    ]
  ```