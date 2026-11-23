### Bibliotech - Gestão de Acervo Literário

## Desafios Técnicos e Aprendizados

O maior desafio durante o desenvolvimento desta atividade foi a configuração correta das variáveis de ambiente e do servidor Nginx, principalmente na integração entre o frontend, o backend e o banco de dados PostgreSQL hospedados no Render. Alguns erros ocorreram por falta de atenção a detalhes importantes, como os valores das variáveis, os caminhos dos arquivos e as configurações necessárias para a execução dos contêineres. Essas dificuldades exigiram análise de logs, revisão dos arquivos de configuração e reconstrução das imagens Docker até que todos os serviços funcionassem corretamente. Apesar dos obstáculos, a experiência foi bastante enriquecedora, pois permitiu colocar em prática conhecimentos sobre Docker, Docker Hub, Nginx e deploy em nuvem, além de reforçar a importância da atenção aos detalhes, da validação de configurações e da resolução de problemas no ambiente de produção. Foi um excelente aprendizado, especialmente por demonstrar como pequenos erros de configuração podem impactar o funcionamento de toda uma aplicação.

## 🔗 Links da Aplicação

A aplicação **BiblioTech** está disponível publicamente por meio do Render, com suas imagens Docker publicadas no Docker Hub e o código-fonte versionado no GitHub.

| Entregável | Descrição | Link |
|---|---|---|
| Frontend — Render | Interface React + Vite hospedada em nuvem | [Acessar aplicação](https://bibliotech-frontend-1-0.onrender.com) |
| Backend — Render | API REST Node.js + Express | [Acessar API](https://bibliotech-backend-1-0.onrender.com/api/books) |
| Frontend — Docker Hub | Imagem Docker do frontend com Nginx | [Visualizar imagem](https://hub.docker.com/r/tomatty/bibliotech-frontend) |
| Backend — Docker Hub | Imagem Docker da API Node.js | [Visualizar imagem](https://hub.docker.com/r/tomatty/bibliotech-backend) |

### 🚀 Executar as imagens Docker

Para executar a aplicação, consulte as instruções de configuração e as variáveis de ambiente documentadas neste repositório.

**Backend:**
```bash
docker pull tomatty/bibliotech-backend:1.1
```

**Frontend:**
```bash
docker pull tomatty/bibliotech-frontend:1.0
```