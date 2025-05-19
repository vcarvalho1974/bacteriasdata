# Sistema de Informação Bacteriológica - Solabia Brasil

Este é um sistema web para consulta de informações detalhadas sobre bactérias, desenvolvido para a Solabia Brasil. O sistema permite buscar informações sobre bactérias na internet, exibindo detalhes sobre onde são encontradas, formas de transmissão e métodos eficazes de eliminação, especialmente para ambientes laboratoriais.

## Funcionalidades

- **Busca com Autocomplete**: Digite o nome da bactéria e receba sugestões em tempo real
- **Consulta na Internet**: Busca informações detalhadas em diversas fontes online
- **Informações Detalhadas**: Exibe dados sobre localização, transmissão e eliminação de bactérias
- **Interface Responsiva**: Funciona em dispositivos desktop e móveis
- **Design Personalizado**: Cabeçalho com degradê entre roxo e verde suaves

## Tecnologias Utilizadas

- React com TypeScript
- Tailwind CSS para estilização
- React Query para gerenciamento de estado e requisições
- Axios para chamadas HTTP

## Como Hospedar no GitHub Pages

### 1. Preparação do Repositório

1. Crie um novo repositório no GitHub
2. Clone o repositório para sua máquina local:
   ```
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   ```
3. Copie todos os arquivos deste projeto para a pasta do repositório clonado

### 2. Configuração para GitHub Pages

1. Abra o arquivo `package.json` e adicione as seguintes linhas:
   ```json
   "homepage": "https://seu-usuario.github.io/nome-do-repositorio",
   "scripts": {
     // outros scripts existentes
     "predeploy": "npm run build",
     "deploy": "gh-pages -d dist"
   }
   ```

2. Instale o pacote gh-pages:
   ```
   npm install --save-dev gh-pages
   ```

### 3. Deploy no GitHub Pages

1. Faça commit de todos os arquivos:
   ```
   git add .
   git commit -m "Versão inicial do Sistema de Informação Bacteriológica"
   ```

2. Envie para o GitHub:
   ```
   git push origin main
   ```

3. Execute o comando de deploy:
   ```
   npm run deploy
   ```

4. Acesse as configurações do repositório no GitHub, vá até a seção "Pages" e selecione a branch `gh-pages` como fonte.

5. Seu site estará disponível em alguns minutos no endereço: `https://seu-usuario.github.io/nome-do-repositorio`

## Desenvolvimento Local

Para executar o projeto localmente:

1. Instale as dependências:
   ```
   npm install
   ```

2. Inicie o servidor de desenvolvimento:
   ```
   npm run dev
   ```

3. Acesse `http://localhost:5173` no seu navegador

## Estrutura do Projeto

- `src/components/Header.tsx`: Componente do cabeçalho com o título personalizado
- `src/components/SearchBar.tsx`: Componente de busca com autocomplete
- `src/components/BacteriaInfo.tsx`: Componente que exibe informações detalhadas sobre a bactéria
- `src/App.tsx`: Componente principal que integra todos os outros
- `src/index.css`: Estilos globais da aplicação

## Personalização

Para personalizar o sistema:

- Altere as cores do degradê no arquivo `src/components/Header.tsx`
- Modifique o logo ou adicione imagens na pasta `public/`
- Ajuste os estilos no arquivo `src/index.css`

## Observações Importantes

- O sistema utiliza APIs públicas para buscar informações, portanto, a disponibilidade e precisão dos dados dependem dessas fontes
- Para um ambiente de produção real, considere implementar um backend próprio ou utilizar APIs específicas para informações bacteriológicas
- As informações exibidas devem ser validadas por especialistas antes de serem utilizadas em procedimentos laboratoriais reais

## Suporte

Para suporte ou dúvidas sobre o sistema, entre em contato com o desenvolvedor.
