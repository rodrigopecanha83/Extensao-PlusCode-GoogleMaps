# Listagem da Chrome Web Store — Copiar Plus Code do Google Maps

Documento gerado para preenchimento direto no **Chrome Developer Dashboard** (Aba **"Detalhes do app"** e Aba **"Privacidade"**).

---

## 📋 Bloco 1: Detalhes do Produto (Aba "Detalhes do app")

### 1.1 Português (Brasil) — Idioma Padrão

- **Título do Pacote:**
  ```text
  Copiar Plus Code do Google Maps
  ```

- **Resumo do Pacote (130 / 132 caracteres):**
  ```text
  Converte coordenadas (lat, lng) copiadas para a área de transferência em Plus Codes do Google Maps com um clique e feedback toast.
  ```

- **Categoria Sugerida:**
  ```text
  Produtividade (ou Ferramentas para Desenvolvedores)
  ```

- **Idioma Principal:**
  ```text
  Português (Brasil)
  ```

- **Descrição Detalhada:**
  ```markdown
  Converta coordenadas geográficas (latitude e longitude) diretamente em Plus Codes do Google Maps de forma instantânea e sem complicações!

  Com o **Copiar Plus Code do Google Maps**, você ganha agilidade no seu fluxo de trabalho: basta copiar qualquer coordenada para a área de transferência e clicar no ícone da extensão. A conversão é feita na hora de forma offline e o Plus Code resultante é copiado automaticamente de volta para a sua área de transferência com uma notificação visual na tela.

  ✨ **Principais Recursos:**
  - ⚡ **Conversão em Um Clique:** Transforma coordenadas copiadas (ex: `-22.9068, -43.1729`) no Plus Code correspondente.
  - 📋 **Cópia Automática:** O código gerado já fica disponível imediatamente na sua área de transferência para colar onde precisar.
  - 🔔 **Notificação Visual Discreta:** Feedback por toast elegante na página para confirmar que a conversão foi bem-sucedida.
  - 🌐 **Suporte Multilíngue Completo:** Interface adaptada para Português, Inglês, Espanhol e Francês.
  - 📴 **Processamento 100% Offline:** Utiliza a biblioteca oficial OpenLocationCode diretamente no seu navegador, sem enviar nenhuma coordenada para servidores externos.

  🔒 **Privacidade e Segurança em Primeiro Lugar:**
  - Zero coleta de dados pessoais ou histórico de navegação.
  - Todo o cálculo matemático é executado de forma puramente local.
  - Não utiliza rastreadores, anúncios ou conexões de rede em segundo plano.

  💡 **Como Usar:**
  1. Copie as coordenadas geográficas (`latitude, longitude`).
  2. Clique no ícone da extensão na barra de ferramentas do seu navegador.
  3. Cole o Plus Code onde desejar!
  ```

---

### 1.2 English (Inglês) — Listagem Internacional

- **Package Title:**
  ```text
  Copy Google Maps Plus Code
  ```

- **Summary (124 / 132 characters):**
  ```text
  Convert copied GPS coordinates (lat, lng) into Google Maps Plus Codes with a single click, instant copy, and toast feedback.
  ```

- **Detailed Description:**
  ```markdown
  Quickly convert geographic coordinates (latitude and longitude) into Google Maps Plus Codes with zero friction!

  With **Copy Google Maps Plus Code**, boost your daily workflow: just copy coordinates to your clipboard and click the extension icon. The conversion is processed offline instantly, and the resulting Plus Code is copied right back to your clipboard with an on-screen toast confirmation.

  ✨ **Key Features:**
  - ⚡ **One-Click Conversion:** Turn copied coordinates (e.g., `-22.9068, -43.1729`) into the matching Plus Code.
  - 📋 **Auto-Copy to Clipboard:** The generated Plus Code is instantly copied and ready to paste.
  - 🔔 **Clean Toast Notification:** Fast on-screen feedback confirming the conversion was successful.
  - 🌐 **Full Multilingual Support:** Ready in English, Portuguese, Spanish, and French.
  - 📴 **100% Offline Processing:** Powered by the official OpenLocationCode library directly in your browser without external servers.

  🔒 **Privacy & Security First:**
  - Zero data collection, tracking, or history storage.
  - Calculations run purely locally on your device.
  - No ads, analytics, or background network calls.

  💡 **How to Use:**
  1. Copy GPS coordinates (`latitude, longitude`) to your clipboard.
  2. Click the extension icon in your Chrome toolbar.
  3. Paste your Plus Code anywhere!
  ```

---

## 🔒 Bloco 2: Privacidade (Aba "Privacidade" do Chrome Developer Dashboard)

### 2.1 Descrição do Único Propósito (Single Purpose Policy)
```text
A extensão tem como único propósito permitir que o usuário converta coordenadas geográficas (latitude e longitude) copiadas na área de transferência em um Plus Code (Open Location Code) do Google Maps com um único clique, copiando o resultado de volta e exibindo um aviso visual (toast) na aba ativa.
```

*(Em inglês, se preferir preencher em inglês):*
```text
The single purpose of this extension is to allow users to convert geographic coordinates (latitude and longitude) copied to their clipboard into a Google Maps Plus Code (Open Location Code) with a single click, automatically copying the result back and showing an on-screen toast notification on the active tab.
```

---

### 2.2 Justificativas Técnicas de Cada Permissão Solicitada

| Permissão (`manifest.json`) | Justificação Técnica Detalhada para o Painel da Chrome Web Store |
| :--- | :--- |
| **`activeTab`** | Necessária para que a extensão possa exibir a notificação visual (toast) temporária de confirmação diretamente na aba atualmente aberta quando o usuário clica no ícone da extensão. |
| **`scripting`** | Necessária para executar o script pontual que lê as coordenadas da área de transferência acionada pelo clique do usuário, calcula o Plus Code via algoritmo OpenLocationCode e injeta o elemento de toast com o resultado. |
| **`clipboardRead`** | Necessária exclusivamente para ler o texto com as coordenadas (latitude e longitude) previamente copiadas pelo usuário no momento em que ele clica no ícone da ação. Nenhum outro conteúdo da área de transferência é armazenado ou transmitido. |
| **`clipboardWrite`** | Necessária para gravar automaticamente o Plus Code gerado na área de transferência do usuário, permitindo colá-lo imediatamente em outros aplicativos ou no Google Maps. |
| **`host_permissions` (`<all_urls>`)** | Necessária para que a extensão funcione sob demanda e possa exibir o toast de notificação em qualquer página da web onde o usuário estiver navegando ao acionar a ferramenta. |

---

### 2.3 Declaração de Uso de Código Remoto (Remote Code)
- **Resposta obrigatória no painel:** Marque **"Não, não estou usando código remoto"** (*"No, I am not using remote code"*).
- **Justificativa interna:** Todo o código JavaScript (incluindo a biblioteca OpenLocationCode e os arquivos de localização de idioma) está 100% empacotado localmente dentro da extensão.
