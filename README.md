# Lolzin - Mundial LoL 2025

Site completo para acompanhar o Mundial de League of Legends 2025 com perfis de jogadores, calendário de partidas e simulador de resultados.

## 🚀 Funcionalidades

- **Home**: Visão geral dos times classificados e próximas partidas
- **Jogadores**: Perfis detalhados de todos os jogadores do mundial com:
  - Estatísticas (Win Rate, KDA, Jogos, Campeonatos)
  - Histórico de títulos mundiais e regionais
  - Times anteriores
  - Conquistas e premiações
  - Destaque especial para campeões mundiais (estilo HLTV)
- **Partidas**: Calendário completo com horários e status das partidas
- **Simulador**: Sistema de simulação de partidas e previsões de campeão

## 🛠️ Tecnologias

- React 18
- React Router DOM
- Vite
- Lucide React (ícones)
- CSS moderno com variáveis e gradientes
- Banco de dados local (JSON)

## 📦 Instalação Local

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/lolzin.git
cd lolzin

# Instale as dependências
npm install

# Rode o servidor de desenvolvimento
npm run dev

# Build para produção
npm run build
```

## 🌐 Deploy no Render

### Passo 1: Configure o Repositório no GitHub

1. Crie um novo repositório no GitHub chamado `lolzin`
2. Execute os comandos:

```bash
git init
git add .
git commit -m "Initial commit - Lolzin Mundial 2025"
git branch -M main
git remote add origin https://github.com/seu-usuario/lolzin.git
git push -u origin main
```

### Passo 2: Deploy no Render

1. Acesse [render.com](https://render.com) e faça login
2. Clique em "New +" e selecione "Static Site"
3. Conecte seu repositório GitHub
4. Configure:
   - **Name**: lolzin
   - **Branch**: main
   - **Build Command**: `npm install && npm run build`
   - **Publish Directory**: `dist`
5. Clique em "Create Static Site"

O site estará disponível em: `https://lolzin.onrender.com`

## 📱 Design Responsivo

O site foi desenvolvido seguindo as melhores práticas de UI/UX:
- Design moderno com gradientes e animações suaves
- Tema escuro otimizado para visualização prolongada
- Cards interativos com efeitos hover
- Layout responsivo para mobile, tablet e desktop
- Tipografia clara e hierarquia visual bem definida
- Destaques especiais para campeões mundiais

## 🎨 Paleta de Cores

- Primary: #e94560 (Vermelho vibrante)
- Secondary: #0f3460 (Azul escuro)
- Accent: #16213e (Azul médio)
- Dark: #0a0e27 (Background)
- Gold: #ffd700 (Campeões mundiais)

## 📊 Banco de Dados

O banco de dados local contém informações completas de:
- 25+ jogadores profissionais
- 5 times classificados (T1, Gen.G, BLG, G2, FlyQuest)
- Estatísticas detalhadas de cada jogador
- Histórico de títulos e conquistas
- Calendário de partidas

## 🏆 Destaques

- Perfis especiais para campeões mundiais com borda dourada
- Sistema de filtros por região e posição
- Simulador com cálculo baseado em estatísticas reais
- Previsões de campeão baseadas em análise de força dos times

## 📄 Licença

MIT License - Sinta-se livre para usar e modificar

## 👨‍💻 Autor

Desenvolvido com ⚡ React + Vite
