# 🚀 Roadmap do DCs.AI

## 🎯 Ciclo de desenvolvimento

📌 Próxima fase de upgrade (Gold Master)

🔧 Recursos prioritários

📦 Exportação de métricas → salvar histórico em core/logs/ e permitir download em CSV.

🌐 Internacionalização → README em inglês e painel com suporte multilíngue.

🧠 Inteligência no painel → histórico de uso, médias, picos e alertas automáticos.

📊 Gráficos múltiplos → CPU, RAM, Disco, Rede e Temperatura separados, com visual mais rico.

🔔 Alertas visuais avançados → cores diferentes e ícones dinâmicos para cada tipo de risco.

🛡️ Estabilidade e robustez

👉 Melhorar tratamento de erros no WebSocket (ex: reconectar se cair).

👉 Garantir que métricas falsas ou zeradas não travem o painel.

👉⚠️ Testes simulando carga alta para validar alertas térmicos e de memória.

# 🌍 Roadmap futuro

Painéis extras com estatísticas acumuladas

# 🚀 Roadmap do DCs.AI

## 🎯 Ciclo de desenvolvimento
- **Protótipo**
  - CPU e RAM em tempo real
  - Conexão WebSocket funcionando
  - Estrutura inicial do repositório (`core/`, `ui/`)

- **Alfa**
  - Adição de Disco 💧 e Rede 🌬️
  - Alertas visuais básicos (CPU, RAM, Disco)
  - Primeiros testes internos com métricas reais

- **Beta**
  - README documentado com prints e exemplos
  - Painel público no GitHub
  - Testes externos
  - Captura de alertas reais (ex: risco térmico ⚠️)

- **Gold Master**
  - Painel consolidado e estável
  - Roadmap definido e documentado
  - Versão internacional (README em inglês)
  - Exportação de métricas e histórico em `core/logs/`
  - Reconhecimento de erros em servidores, jogos ou sistemas antes que causem impacto
  - Sugestão/aplicação de correções automáticas
  - Prevenção de problemas futuros com aprendizado de incidentes
  - Geração de logs e painéis de telemetria
  - Funcionamento como sentinela ativo em background

---

## 🚀 Roadmap de evolução

- 🔔 **Alertas visuais**  
  Cores diferentes quando CPU/RAM > 80%. Ícones ou mensagens de risco no painel.

- 📦 **Exportar dados**  
  Botão para baixar CSV com métricas coletadas. Útil para análise posterior ou compartilhar logs.

- 📊 **Múltiplos gráficos**  
  Separar CPU e RAM em gráficos distintos. Adicionar métricas extras: disco, rede, temperatura.

- 🌐 **Dados reais**  
  Substituir valores simulados por leitura via `psutil` no Python. Enviar em tempo real pelo WebSocket.

- 🧠 **Inteligência no painel**  
  Histórico de uso (últimos minutos). Médias, picos e alertas automáticos. Possível dashboard com estatísticas acumuladas.


## 💡 Funções que podem ser adaptadas
- 🌬️ Uso de rede ou atividade de processos  
  Exemplo: `Rede: 13 Mbps — leve tráfego de saída`

- 💧 Uso de disco ou cache ocupada  
  Exemplo: `Disco: 89% — alto uso`

- 🌞 Tempo de boot ou tempo desde último reinício  
  Exemplo: `Sistema ligado desde: 5:17 AM`

- 📈 Carga do sistema ou estabilidade  
  Exemplo: `Carga: 1.013 — estável`

- 🔆 Risco térmico ou alerta de pico  
  Exemplo: `CPU em pico: 90% — risco alto`

- 🕒 Métricas por minuto  
  Exemplo: `CPU/RAM nas últimas 6 horas`


## 🧪 Como isso pode aparecer no DCs.AI Painel
- Painéis como ícones e dados (estilo cards)  
- Gráfico principal + cards laterais com dados extras  
- Seções tipo:  
  - “Condições atuais do sistema”  
  - “Histórico por hora”  
  - “Alertas e picos recentes”
