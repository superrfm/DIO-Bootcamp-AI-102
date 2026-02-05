# Dev.to Article Translator

Este projeto é uma ferramenta desenvolvida em Python para extrair o conteúdo de artigos do site [dev.to](https://dev.to/) e traduzi-lo para o idioma desejado usando o serviço Azure Translator.

## Funcionalidades

- **Extração de Conteúdo:** Obtém o título e o corpo principal de artigos do dev.to.
- **Tradução:** Utiliza o Azure Translator para traduzir o conteúdo extraído para uma língua alvo.
- **Validação de URL:** Garante que apenas URLs do dev.to sejam processadas.
- **Configuração de Chave de API:** Permite a entrada da chave de assinatura e região do Azure Translator de forma interativa.

## Configuração

Para usar este projeto, você precisará de uma chave de assinatura e uma região de serviço para o Azure Translator.

1. **Instale as dependências:**
   ```bash
   !pip install requests beautifulsoup4
   ```

2. **Obtenha suas credenciais do Azure Translator:**
   - Vá para o [portal do Azure](https://portal.azure.com/).
   - Crie um recurso de **Text Translator**.
   - Anote a **Chave de Assinatura (Subscription Key)** e a **Região do Serviço (Location)**.

## Como usar

1. **Execute as células iniciais:** Certifique-se de que todas as células de importação (`pRUP7K60UiWY`), configuração de chaves (`2lcLdBAGGa5E`, `56chGBMmXvWz`), e definição de funções (`9td3TOMVUmW7`, `UYbofRNkDiV3`) tenham sido executadas.

2. **Extraia e traduza um artigo:**
   Execute a célula `XbHVMLn3Gnrh`. Ela irá:
   - Solicitar a **URL do artigo** (padrão: `https://dev.to/aaron_rose_0787cc8b4775a0/the-secret-life-of-python-the-silent-type-type-casting-5c57`).
   - Validar se a URL pertence ao `dev.to`.
   - Solicitar a **linguagem de destino** para a tradução (padrão: `pt-br`).
   - Exibir o conteúdo traduzido.

### Exemplo de Entrada

```
Por favor, insira a URL do site (padrão: https://dev.to): https://dev.to/aaron_rose_0787cc8b4775a0/the-secret-life-of-python-the-silent-type-type-casting-5c57
Por favor, insira a linguagem destino (padrão: 'pt-br'): pt-br
```

### Exemplo de Saída (Conteúdo Traduzido)

```
Extraindo conteúdo de: https://dev.to/aaron_rose_0787cc8b4775a0/the-secret-life-of-python-the-silent-type-type-casting-5c57
Traduzindo conteúdo para: pt-br
Conteúdo Traduzido:
Entendendo bugs de Conjuração de Tipo e Input().

Timothy se recostou na cadeira, olhando para a tela com uma mistura de confusão e diversão. "Margaret? Acho que meu computador perdeu a cabeça."
...
```

## Dependências

- `requests`
- `beautifulsoup4`
- `uuid` (módulo padrão do Python)

## Autor

Desenvolvido como parte de um projeto de demonstração de tradução de conteúdo web.
