# Maurício Mello - Android Developer Portfolio 📱

Olá! Sou o Maurício, desenvolvedor Android focado em criar aplicativos nativos de alta performance, modernos, escaláveis e com design centrado na experiência do usuário (UX). Trabalho com as principais tecnologias recomendadas pelo Google para desenvolvimento nativo moderno.

---

## 🛠️ Habilidades Técnicas (Tech Stack)

*   **Linguagens:** Kotlin (Sólido), Java
*   **Interface Gráfica (UI):** Jetpack Compose, Material Design 3, XML Clássico
*   **Arquitetura & Padrões:** Clean Architecture, MVVM (Model-View-ViewModel), StateFlow/SharedFlow, Injeção de Dependências (Dagger Hilt)
*   **Banco de Dados & Persistência:** Room Database, SQLite, SharedPreferences
*   **Assincronismo:** Kotlin Coroutines & Flow
*   **Backend & Sincronização:** Firebase Firestore, Firebase Cloud Messaging, APIs RESTful (Retrofit, Ktor), Servidor Flask (Python)
*   **Mapas & Geolocalização:** osmdroid, OSRM (Open Source Routing Machine), Nominatim API, FusedLocationProviderClient (Google Play Services)
*   **Outras Ferramentas:** Git/GitHub, NotificationListenerService (Background execution), PDF Document Generation, TextToSpeech API

---

## 🚀 Projetos em Destaque

Abaixo estão os projetos nativos desenvolvidos por mim, detalhando as soluções arquiteturais e recursos implementados:

### 1. 🗺️ GPS Pro (Sistema de Navegação & Alertas em Tempo Real)
Aplicativo de navegação ativo completo com visualização dark futurista (cyberpunk), inteligência de câmera ativa, alertas locais e sincronização via Firebase.
*   **Recursos Principais:**
    *   **Navegação Ativa Estilo Waze:** Câmera 3D travada no veículo, rotacionando o mapa dinamicamente baseado na direção (*bearing*) do motorista e deslocando o ponto central (offset) para mostrar mais pista à frente.
    *   **Alertas em Tempo Real via Firestore:** Registro de perigos (Radar, Polícia, Acidente, Buraco) com sincronização em tempo real e expiração automática dos pins após 2 horas.
    *   **Filtro Geográfico Dinâmico:** Algoritmo que calcula distâncias e exibe alertas no mapa apenas dentro do raio de 10 km da posição atual.
    *   **Busca Integrada Nominatim:** Pesquisa preditiva que exibe um painel de detalhes do endereço no rodapé contendo o local, bairro e cidade antes de traçar a rota.
    *   **TTS (TextToSpeech) e Recálculo:** Sintetizador de voz nativo que avisa manobras em português e dispara novo request de rota (OSRM) em caso de desvio de rota de 60 metros.
*   **Stack:** Kotlin, osmdroid, OSRM API, Nominatim, Play Services Location, Firebase Firestore.

### 2. 💰 Leitor Financeiro Pro (Automação de Transações Bancárias)
Gerenciador de finanças reativo que automatiza o controle de gastos lendo notificações de transações financeiras em segundo plano.
*   **Recursos Principais:**
    *   **Leitura de Notificações em Background:** Captura automática de mensagens bancárias através de `NotificationListenerService` com extração precisa de dados e controle anti-duplicidade de transações.
    *   **Módulo de Controle de Reservas:** Sistema para poupar dinheiro que deduz as reservas do saldo líquido utilizável exibindo os valores de forma isolada.
    *   **Relatórios e Comprovantes em PDF:** Geração e exportação de relatórios em formato A4 diretamente na memória do aparelho.
    *   **Verificação de Updates com Flask:** Sistema conectado a um backend em Python (Flask) que avisa o usuário sobre novas versões e instala o APK diretamente.
*   **Stack:** Kotlin, Jetpack Compose, Room Database, NotificationListener API, PDF Document API.

### 3. 📅 Agenda Show Jackson e Maurício (Gestão de Shows e Logística)
Aplicativo de painel de controle e gerenciamento de agenda, projetado para conciliação offline de datas de apresentações e controle de cachês.
*   **Recursos Principais:**
    *   **Sincronização Offline First:** Armazenamento local das datas de shows em banco SQLite e Room para acesso sem internet, com upload assíncrono ao conectar.
    *   **Painel Financeiro Integrado:** Cálculo de despesas de viagem, faturamento bruto e líquido da banda.
*   **Stack:** Kotlin, Jetpack Compose, Room DB, Coroutines.

### 4. 🩺 ClinicFlow (Gestão de Fluxo de Atendimento Clínico)
Painel inteligente integrado para controle de filas e triagem de pacientes em clínicas de saúde.
*   **Recursos Principais:**
    *   **Painel Interativo:** Organização de prioridades no fluxo de atendimento médico de forma reativa.
    *   **Integração e Sincronização:** Listagem dinâmica atualizada instantaneamente ao despachar pacientes.
*   **Stack:** Kotlin, Jetpack Compose, Coroutines, Flow.

### 5. 🎧 VsShowPlayer (Reprodutor Multitrack para Bandas)
Player de áudio nativo de alta performance para reprodução de trilhas de backing track (VS) e cliques de bateria sincronizados.
*   **Recursos Principais:**
    *   **Separação de Canais L/R:** Envia a guia/clique para o fone do baterista (Canal Esquerdo) e as pistas de instrumento (VS) para a mesa de som (Canal Direito).
    *   **Latência Zero:** Utilização de buffers otimizados para garantir o tempo perfeito de execução musical.
*   **Stack:** Kotlin, Jetpack Compose, Android Media Player / ExoPlayer API.

---

## 📈 Contato & Redes

*   **LinkedIn:** [linkedin.com/in/mauriciomello](https://linkedin.com)
*   **GitHub:** [github.com/MauriciovzM](https://github.com/MauriciovzM)
*   **E-mail:** [kakau466@gmail.com](mailto:kakau466@gmail.com)
