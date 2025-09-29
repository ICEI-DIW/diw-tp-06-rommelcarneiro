# Relatório de Desempenho - Portal de Notícias Dinâmico
<sup>Este é um feedback gerado por IA e pode conter erros. Você tem 9 créditos restantes.</sup>

Olá, **rommelcarneiro**! Aqui está um feedback detalhado sobre sua atividade.
> **Nota Final:** **`0.00 / 100`**
---
# Feedback sobre a Atividade

Olá! Parece que você teve alguns problemas ao enviar seu projeto. Infelizmente, não consegui encontrar nenhum dos arquivos esperados (`index.html`, `detalhes.html`, `css/styles.css` e `app.js`). É importante que você verifique se todos os arquivos necessários foram incluídos antes de enviar novamente seu projeto.

Vou compartilhar algumas dicas gerais com base nos objetivos da atividade para que você possa começar a trabalhar neles:

1. **Estrutura de Dados em `app.js`**: Você precisa criar uma estrutura de dados (como um array de objetos) que contém as informações de cada notícia. Cada objeto deve ter um 'id' único. Isso permitirá que você carregue dinamicamente as informações na página. Para aprender mais sobre como trabalhar com JSON em JavaScript, você pode verificar este guia: [Aprenda a trabalhar com a estrutura de dados JSON em JavaScript](https://developer.mozilla.org/pt-BR/docs/Learn/JavaScript/Objects/JSON).

2. **Renderização Dinâmica dos Cards em `index.html`**: Você precisa usar a manipulação do DOM para criar e inserir os cards de notícias na página `index.html`. Cada card deve ser criado com base nas informações da sua estrutura de dados em `app.js`. Para aprender mais sobre manipulação do DOM, você pode verificar este guia: [Guia sobre Manipulação do DOM (Document Object Model) para criar conteúdo dinâmico](https://developer.mozilla.org/pt-BR/docs/Web/API/Document_Object_Model/Introduction).

3. **Links nos Cards**: Cada card deve conter um link para a página `detalhes.html`, com o 'id' do item na query string (ex: `detalhes.html?id=1`). Isso permitirá que a página `detalhes.html` saiba qual notícia exibir.

4. **Página `detalhes.html`**: Esta página deve ser capaz de ler o 'id' da URL, encontrar o item correspondente na estrutura de dados e exibir suas informações. Para aprender mais sobre como ler parâmetros da query string, você pode verificar este tutorial: [Tutorial sobre como usar URLSearchParams para ler parâmetros da query string da URL](https://developer.mozilla.org/pt-BR/docs/Web/API/URLSearchParams).

5. **Sem Frameworks de JavaScript**: Lembre-se de que o uso de frameworks de JavaScript como React, Vue ou Angular não é permitido neste projeto. Você deve usar apenas JavaScript puro para manipulação do DOM e interação com a página.

Espero que essas dicas sejam úteis! Não se esqueça de verificar se todos os arquivos necessários estão presentes antes de enviar novamente seu projeto. Mantenha o bom trabalho e continue aprendendo! Se tiver mais perguntas, fique à vontade para perguntar. 😊


---

### 📝 Resumo dos Pontos de Atenção
| Ação | Tópico | Detalhes do Teste |
|:---|:---|:---|
| Revisar | `structure` | **Teste:** `has_tag`<br>**O que ele faz:** *Verifica se uma tag HTML específica aparece um número mínimo de vezes.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `structure` | **Teste:** `has_attribute`<br>**O que ele faz:** *Verifica se um atributo HTML específico está presente em qualquer tag, um número mínimo de vezes.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `link` | **Teste:** `check_css_linked`<br>**O que ele faz:** *Verifica se uma folha de estilo CSS externa está vinculada no HTML.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `link` | **Teste:** `check_internal_links_to_article`<br>**O que ele faz:** *Verifica a existência de um número mínimo de links âncora internos apontando para IDs em tags `<article>`.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `responsivity` | **Teste:** `uses_relative_units`<br>**O que ele faz:** *Verifica se o arquivo CSS usa unidades relativas como em, rem, %, vh, vw.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `responsivity` | **Teste:** `check_media_queries`<br>**O que ele faz:** *Verifica se existem media queries no arquivo CSS.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `responsivity` | **Teste:** `check_flexbox_usage`<br>**O que ele faz:** *Verifica se propriedades Flexbox são usadas no arquivo CSS.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `style` | **Teste:** `has_style`<br>**O que ele faz:** *Verifica se uma regra de estilo CSS específica aparece um número mínimo de vezes.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `bootstrap_fundamentals` | **Teste:** `check_bootstrap_linked`<br>**O que ele faz:** *Verifica se o framework Bootstrap (CSS ou JS) está vinculado no arquivo HTML.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `bootstrap_fundamentals` | **Teste:** `check_internal_links`<br>**O que ele faz:** *Verifica a existência de um número mínimo de links âncora internos que apontam para IDs de elementos válidos.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `bootstrap_fundamentals` | **Teste:** `has_class`<br>**O que ele faz:** *Verifica a presença de classes CSS específicas, com suporte a curingas, um número mínimo de vezes.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `css_and_docs` | **Teste:** `check_media_queries`<br>**O que ele faz:** *Verifica se existem media queries no arquivo CSS.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `css_and_docs` | **Teste:** `has_style`<br>**O que ele faz:** *Verifica se uma regra de estilo CSS específica aparece um número mínimo de vezes.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `dynamic_js` | **Teste:** `js_has_json_array_with_id`<br>**O que ele faz:** *Verifica a existência de um array de objetos JS onde cada objeto possui uma chave específica obrigatória.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `dynamic_js` | **Teste:** `js_uses_dom_manipulation`<br>**O que ele faz:** *Verifica se o código JS usa um número mínimo de métodos comuns de manipulação do DOM.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `dynamic_js` | **Teste:** `js_uses_query_string_parsing`<br>**O que ele faz:** *Verifica se o código JavaScript contém padrões para ler query strings da URL.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `linking_and_integrity` | **Teste:** `link_points_to_page_with_query_param`<br>**O que ele faz:** *Verifica a existência de tags âncora que levam a uma página específica com um parâmetro de query string obrigatório.*<br>**Parâmetros:** <sub>N/A</sub> |
| Corrigir (Penalidade) | `html` | **Teste:** `check_id_selector_over_usage`<br>**O que ele faz:** *Conta o número de seletores de ID usados e penaliza se exceder o máximo permitido.*<br>**Parâmetros:** <sub>N/A</sub> |
| Corrigir (Penalidade) | `html` | **Teste:** `has_forbidden_tag`<br>**O que ele faz:** *Verifica a presença de uma tag HTML proibida.*<br>**Parâmetros:** <sub>N/A</sub> |
| Corrigir (Penalidade) | `html` | **Teste:** `check_html_direct_children`<br>**O que ele faz:** *Garante que os únicos filhos diretos da tag `<html>` são `<head>` e `<body>`.*<br>**Parâmetros:** <sub>N/A</sub> |
| Corrigir (Penalidade) | `html` | **Teste:** `check_tag_not_inside`<br>**O que ele faz:** *Verifica se uma tag específica não está aninhada em nenhum lugar dentro de outra tag específica.*<br>**Parâmetros:** <sub>N/A</sub> |
| Corrigir (Penalidade) | `project_structure` | **Teste:** `check_dir_exists`<br>**O que ele faz:** *Verifica se um diretório específico existe no envio.*<br>**Parâmetros:** <sub>`dir_path`: `css`</sub> |
| Corrigir (Penalidade) | `project_structure` | **Teste:** `check_dir_exists`<br>**O que ele faz:** *Verifica se um diretório específico existe no envio.*<br>**Parâmetros:** <sub>`dir_path`: `imgs`</sub> |
| Corrigir (Penalidade) | `project_structure` | **Teste:** `check_project_structure`<br>**O que ele faz:** *Verifica se o caminho da estrutura esperada existe nos arquivos de envio.*<br>**Parâmetros:** <sub>`expected_structure`: `css/styles.css`</sub> |


---
> Caso queira tirar uma dúvida específica, entre em contato com o Chapter.