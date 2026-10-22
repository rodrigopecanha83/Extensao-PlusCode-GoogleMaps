# Copiar Plus Code do Google Maps (Extensao-PlusCode-GoogleMaps)

Extensão para o Google Chrome que lê coordenadas geográficas da área de transferência (latitude e longitude), converte automaticamente para o respectivo Plus Code (Open Location Code) e copia o resultado de volta para a área de transferência.

## Funcionalidades Principais

* **Conversão Automática:** Converte coordenadas no formato latitude e longitude copiadas diretamente em Plus Codes do Google Maps.
* **OpenLocationCode Integrado:** Processamento e cálculo de geolocalização totalmente local e offline utilizando a biblioteca OpenLocationCode.
* **Notificação Toast:** Exibe feedback visual na aba ativa informando o Plus Code gerado e copiado.

## Pré-requisitos

* Google Chrome ou qualquer navegador baseado em Chromium compatível com extensões Manifest V3.

## Instalação e Configuração

1. Abra o Google Chrome e acerte o endereço `chrome://extensions/`.
2. Ative a chave **Modo do desenvolvedor** no canto superior direito.
3. Clique no botão **Carregar sem compactação** e selecione a pasta raiz desta extensão (`Extensao-PlusCode-GoogleMaps`).

## Como Usar

1. Copie as coordenadas geográficas (exemplo: `-22.9068, -43.1729`) para a área de transferência.
2. Clique no ícone da extensão na barra de ferramentas do navegador.
3. O Plus Code correspondente será copiado automaticamente e uma notificação na tela confirmará a conversão.

## Histórico de Versões

### v1.0.0 - 2026-10-22
- Lançamento inicial da extensão em Manifest V3.
- Leitura e validação de coordenadas a partir do clipboard.
- Conversão offline para Plus Code com a biblioteca OpenLocationCode.
- Notificação toast na página e cópia automática do código resultante.

## Contribuindo

Sugestões e correções são bem-vindas. Abra uma Issue ou envie um Pull Request.

## Licença

TODO: definir licença. Veja o arquivo `LICENSE` para mais detalhes.

## Autor

Rodrigo Peçanha