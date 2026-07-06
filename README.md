# ⛽ Gestor de Despesas de Viaturas (Nativo e Estável)

Uma aplicação web estática (Single Page Application) leve, segura e responsiva, concebida para funcionar em qualquer navegador de forma 100% local, autónoma e sem a necessidade de servidores externos ou bases de dados complexas.

## 🚀 Funcionalidades Principais

- **Persistência Local (localStorage)**: Guarda todas as contas de utilizadores, veículos e despesas diretamente no navegador, permitindo a utilização em Modo Offline.
- **Isolamento de Dados**: Sistema multi-utilizador simulado localmente. O Utilizador A nunca conseguirá visualizar as viaturas ou despesas do Utilizador B.
- **Ficha Técnica Expandida**: Permite carregar fotos personalizadas dos veículos com **compressão automática via Canvas** para poupar espaço, além de registar o Tipo de Combustível (Gasolina, Diesel, GPL, Elétrico).
- **Alertas Dinâmicos e Prazos Legais**: Avisos visuais coloridos (Verde/Amarelo/Vermelho) para datas de vencimento do Seguro, Inspeção (IPO) e quilometragem para a próxima revisão (ex: mudar o óleo).
- **Filtros Avançados Combinados**: Filtragem em tempo real na tabela de registos por Mês e por Categoria em simultâneo.
- **Validação de Quilometragem**: Impede inserções acidentais de KMs inferiores ao maior valor já registado para evitar corrupção nos cálculos de consumo.
- **Exportação Mestre (Excel/CSV)**: Botão nativo que gera relatórios em formato CSV compatível com as regras de acentuação e separadores regionais, respeitando os filtros ativos no ecrã.
- **Painel Geral de Administração**: Acesso de super-utilizador (`admin@sistema.com`) para auditoria global de todas as contas, tabelas de gastos e exportação de toda a base de dados do sistema.
- **Modo Escuro Permanente**: Interface adaptável com memorização de tema ativa.

## 📂 Estrutura do Projeto

```text
📂 gestor-despesas-viaturas
 ┣ 📂 imagens
 ┃ ┣ 🖼️ oficina.jpg
 ┃ ┣ 🖼️ seguros.jpg
 ┃ ┗ 🖼️ pneus.jpg
 ┣ 📄 index.html (Código-fonte unificado: HTML5, CSS3 e JS Nativo)
 ┗ 📄 README.md (Documentação do sistema)
```

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estruturação semântica e File API.
- **CSS3**: Layouts flexíveis (Flexbox), animações e transições do carrossel publicitário e Modo Escuro.
- **JavaScript (Vanilla JS)**: Lógica de encriptação Base64, manipulação do Canvas para compressão de imagens, motores de filtragem, exportadores de ficheiros e Web Storage.
