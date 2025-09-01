# 🌊 Flume Water - Monitor de Consumo de Água

Um aplicativo web que simula o funcionamento do **Flume Water**, permitindo monitorar o consumo de água residencial em tempo real com interface moderna e intuitiva.

![Flume Water App](https://img.shields.io/badge/Version-1.0.0-blue) ![HTML](https://img.shields.io/badge/HTML-5-orange) ![CSS](https://img.shields.io/badge/CSS-3-blue) ![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)

## 📋 Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Funcionalidades](#funcionalidades)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Como Usar](#como-usar)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Screenshots](#screenshots)
- [Personalização](#personalização)
- [Contribuições](#contribuições)
- [Licença](#licença)

## 🎯 Sobre o Projeto

O **Flume Water App** é uma simulação completa do aplicativo original Flume Water, desenvolvido para demonstrar como seria uma interface de monitoramento de consumo de água residencial. O projeto inclui todas as funcionalidades principais do app original, com dados simulados atualizados em tempo real.

### 🌟 Características Principais

- **Interface Moderna**: Design limpo e intuitivo inspirado no app original
- **Responsivo**: Funciona perfeitamente em desktop, tablet e celular
- **Tempo Real**: Dados atualizados automaticamente a cada 2 segundos
- **Navegação Intuitiva**: Sistema de abas na parte inferior
- **Dados Realistas**: Simulação de consumo de água com valores realistas

## ⚡ Funcionalidades

### 🏠 Dashboard Principal
- **Monitoramento em tempo real** do consumo atual (L/min)
- **Consumo diário** com valor atualizado
- **Estatísticas semanais e mensais**
- **Consumo por ambiente** (Cozinha, Banheiros, Lavanderia)
- **Sistema de alertas** para uso elevado e vazamentos

### 📊 Análises Detalhadas
- **Gráfico de consumo semanal** com barras interativas
- **Comparativo mensal** com percentual de economia
- **Metas de economia** com indicador visual de progresso
- **Histórico de consumo** por períodos

### ⚙️ Configurações Avançadas
- **Alertas personalizáveis** (uso elevado, vazamentos, relatórios)
- **Preferências de unidades** (Litros/Galões)
- **Configuração de metas** mensais de consumo
- **Status dos dispositivos** conectados
- **Relatórios automáticos** por email

## 🛠️ Tecnologias Utilizadas

- **HTML5** - Estrutura semântica
- **CSS3** - Estilos responsivos e animações
- **JavaScript (ES6)** - Funcionalidade interativa
- **Lucide Icons** - Biblioteca de ícones moderna
- **CSS Grid & Flexbox** - Layout responsivo
- **LocalStorage** (opcional) - Persistência de dados

## 🚀 Como Usar

### Método 1: Arquivo HTML Único
1. **Download** do arquivo `flume-water.html`
2. **Abra** o arquivo em qualquer navegador moderno
3. **Navegue** pelas abas para explorar as funcionalidades

### Método 2: Servidor Local
```bash
# Clone ou baixe o projeto
git clone [url-do-repositorio]

# Entre na pasta
cd flume-water-app

# Inicie um servidor local (Python)
python -m http.server 8000

# Ou use o Live Server do VS Code
# Abra o projeto no VS Code e use a extensão Live Server
```

### Método 3: Hospedagem Online
- **GitHub Pages**: Faça upload para um repositório GitHub
- **Netlify**: Arraste o arquivo para netlify.app
- **Vercel**: Deploy direto da pasta do projeto

## 📁 Estrutura do Projeto

```
flume-water-app/
│
├── flume-water.html          # Aplicação completa (HTML+CSS+JS)
├── README.md                 # Este arquivo
│
└── assets/ (opcional)
    ├── screenshots/          # Capturas de tela
    └── docs/                 # Documentação adicional
```

### 🏗️ Estrutura do HTML

- **Header**: Logo e status de conexão
- **Dashboard**: Tela principal com consumo atual
- **Analytics**: Gráficos e análises de consumo
- **Settings**: Configurações e preferências
- **Bottom Navigation**: Navegação entre páginas

## 📱 Screenshots

### Dashboard Principal
- Consumo atual em tempo real
- Estatísticas diárias e mensais
- Uso por ambiente com gráficos

### Página de Análises
- Gráfico de consumo semanal
- Comparativos mensais
- Metas de economia

### Configurações
- Alertas personalizáveis
- Preferências de unidades
- Status dos dispositivos

## 🎨 Personalização

### Cores e Temas
```css
:root {
  --primary-color: #3b82f6;    /* Azul principal */
  --success-color: #10b981;    /* Verde para economia */
  --warning-color: #f59e0b;    /* Amarelo para alertas */
  --danger-color: #ef4444;     /* Vermelho para problemas */
}
```

### Dados Simulados
Modifique os valores iniciais no JavaScript:
```javascript
let currentUsage = 2.3;        // Uso atual (L/min)
let dailyUsage = 127;          // Consumo diário (L)
let monthlyUsage = 3420;       // Consumo mensal (L)
```

### Ambientes Monitorados
Edite a lista de ambientes no HTML:
```javascript
const locations = [
    { name: 'Seu Ambiente', usage: 34.2, percentage: 27 }
    // Adicione mais ambientes aqui
];
```

## 📊 Dados e Métricas

### Valores Simulados
- **Uso atual**: 0.5 - 4.0 L/min (varia automaticamente)
- **Consumo diário**: ~127 L (incrementa gradualmente)
- **Consumo mensal**: ~3420 L (meta: 4000 L)
- **Ambientes**: Cozinha, Banheiros, Lavanderia

### Frequência de Atualização
- **Dados principais**: A cada 2 segundos
- **Gráficos**: Estáticos (podem ser dinamizados)
- **Alertas**: Configuráveis pelo usuário

## 🔧 Funcionalidades Avançadas

### Sistema de Alertas
- **Uso elevado**: Detecta quando o consumo excede limites
- **Vazamentos**: Simula detecção de vazamentos
- **Relatórios**: Notificações sobre relatórios disponíveis

### Responsividade
- **Mobile First**: Otimizado para dispositivos móveis
- **Breakpoints**: 480px, 768px, 1024px
- **Touch Friendly**: Botões e elementos otimizados para touch

### Acessibilidade
- **Cores contrastantes**: Atende WCAG 2.1
- **Textos alternativos**: Para ícones e imagens
- **Navegação por teclado**: Suporte completo

## 🤝 Contribuições

Contribuições são bem-vindas! Para contribuir:

1. **Fork** o projeto
2. **Crie** uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. **Commit** suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. **Push** para a branch (`git push origin feature/AmazingFeature`)
5. **Abra** um Pull Request

### 📋 To-Do List

- [ ] Integração com APIs reais de sensores
- [ ] Sistema de login/cadastro
- [ ] Histórico de dados mais extenso
- [ ] Exportação de relatórios (PDF/Excel)
- [ ] Notificações push
- [ ] Modo escuro
- [ ] Múltiplas residências
- [ ] Comparação com vizinhos

## 📄 Licença

Este projeto é uma simulação educacional e não possui afiliação oficial com a Flume Water. 

**MIT License** - Veja o arquivo `LICENSE` para mais detalhes.

## 👨‍💻 Autor
Caíque Gomes
Desenvolvido como simulação educacional do aplicativo Flume Water.


## 🔗 Links Úteis

- [Flume Water Original](https://flumewater.com/)
- [Lucide Icons](https://lucide.dev/)
- [MDN Web Docs](https://developer.mozilla.org/)
- [Can I Use](https://caniuse.com/)

---

⭐ **Se este projeto foi útil, não esqueça de dar uma estrela!**

📱 **Testado em**: Chrome, Firefox, Safari, Edge
🌐 **Compatibilidade**: iOS Safari, Chrome Mobile, Samsung Internet
