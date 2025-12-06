![Integrando seu projeto React com APIs](thumbnail.png)

# Alfood

O Alfood é um site que lista restaurantes e pratos do menu. 
É um MVP que tá só começando e ainda tem muitas funcionalidades novas para serem desenvolvidas.

<img src="screencapture.png" alt="Imagem do Alfood" width="50%">


## 🔨 Funcionalidades do projeto

O Alfood é uma aplicação completa de gerenciamento de restaurantes e pratos, com integração total com a API.

### Funcionalidades Implementadas

#### 🏠 Páginas Públicas
- **Home**: Página inicial do site
- **Vitrine de Restaurantes**: Listagem pública de restaurantes e seus pratos

#### 🔐 Área Administrativa

**Gerenciamento de Restaurantes:**
- ✅ Listagem de restaurantes cadastrados
- ✅ Criação de novos restaurantes
- ✅ Edição de restaurantes existentes
- ✅ Exclusão de restaurantes

**Gerenciamento de Pratos:**
- ✅ Listagem de pratos cadastrados
- ✅ Criação de novos pratos com upload de imagem
- ✅ Edição de pratos existentes (com atualização opcional de imagem)
- ✅ Exclusão de pratos
- ✅ Visualização de imagens dos pratos

### Rotas da Aplicação

- `/` - Página inicial
- `/restaurantes` - Vitrine de restaurantes
- `/admin/restaurantes` - Administração de restaurantes
- `/admin/restaurantes/novo` - Cadastro de novo restaurante
- `/admin/restaurantes/:id` - Edição de restaurante
- `/admin/pratos` - Administração de pratos
- `/admin/pratos/novo` - Cadastro de novo prato
- `/admin/pratos/:id` - Edição de prato

## ✔️ Técnicas e tecnologias utilizadas

Se liga nessa lista de tudo que usaremos nesse treinamento:

- **React** - Biblioteca JavaScript para construção de interfaces
- **React Hooks** - useState, useEffect para gerenciamento de estado e efeitos colaterais
- **TypeScript** - Superset do JavaScript com tipagem estática
- **axios** - Cliente HTTP para comunicação com APIs
- **React Router DOM** - Roteamento e navegação entre páginas
- **Material-UI (MUI)** - Biblioteca de componentes React
- **FormData** - API para envio de dados multipart/form-data (upload de imagens)
- **SCSS Modules** - Estilização com módulos CSS

## 🛠️ Abrir e rodar o projeto

### Pré-requisitos
- Node.js instalado
- API backend rodando (normalmente em `http://localhost:8000`)

### Instalação e Execução

1. Clone o repositório
2. Instale as dependências:
```bash
npm i
```

3. Inicie o projeto:
```bash
npm start
```

4. Acesse <a href="http://localhost:3000/">http://localhost:3000/</a> no seu navegador

### Estrutura do Projeto

```
src/
├── componentes/          # Componentes reutilizáveis
│   ├── Banner/
│   ├── ListaRestaurantes/
│   ├── NavBar/
│   └── Rodape/
├── interfaces/           # Interfaces TypeScript
│   ├── IPaginacao.ts
│   ├── IPrato.ts
│   └── IRestaurante.ts
├── paginas/             # Páginas da aplicação
│   ├── Administracao/   # Área administrativa
│   │   ├── Pratos/
│   │   └── Restaurantes/
│   ├── Home/
│   └── VitrineRestaurantes/
└── http/                # Configuração do axios
```

### Funcionalidades de API

O projeto utiliza endpoints REST para comunicação com o backend:

- `GET /api/v2/restaurantes/` - Lista restaurantes
- `POST /api/v2/restaurantes/` - Cria restaurante
- `PUT /api/v2/restaurantes/:id/` - Atualiza restaurante
- `DELETE /api/v2/restaurantes/:id/` - Exclui restaurante
- `GET /api/v2/pratos/` - Lista pratos
- `POST /api/v2/pratos/` - Cria prato (com upload de imagem)
- `PUT /api/v2/pratos/:id/` - Atualiza prato
- `DELETE /api/v2/pratos/:id/` - Exclui prato
- `GET /api/v2/tags/` - Lista tags disponíveis

## 📚 Mais informações do curso

Busque na plataforma da Alura o curso **Integrando seu projeto React com APIs** publicado na Escola Frontend.