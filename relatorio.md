# Relatório de Desempenho - Portal de Notícias Dinâmico
<sup>Este é um feedback gerado por IA e pode conter erros. Você tem 9 créditos restantes.</sup>

Olá, **rommelcarneiro**! Aqui está um feedback detalhado sobre sua atividade.
> **Nota Final:** **`49.52 / 100`**
---
# Olá! 👋

Primeiramente, parabéns pelo seu progresso até agora! Seu código está bem estruturado e você já implementou muitas funcionalidades importantes. No entanto, há algumas melhorias que podemos fazer para aperfeiçoar ainda mais o seu projeto. Vamos lá!

## HTML

Você fez um bom trabalho garantindo que todas as suas imagens tenham um atributo `alt`, o que é ótimo para a acessibilidade. E também está cuidando bem da semântica do seu documento, utilizando as tags `header`, `main`, `section`, `article` e `footer`. Além disso, você está utilizando corretamente as meta tags no `head` do documento. Esses são ótimos hábitos a se manter!

No entanto, percebi que você está utilizando muitos seletores de ID em seu CSS. Isso pode tornar o código mais difícil de manter no futuro devido à especificidade alta dos seletores de ID. Como boa prática, recomendo utilizar classes sempre que possível.

## CSS

Sobre o CSS, você está usando uma estrutura bem organizada e fácil de entender. Mas percebi que você está usando unidades absolutas (`px`) em seu CSS. Isso pode dificultar a responsividade do design. Recomendo que você use unidades relativas, como `em`, `rem`, `%`, `vh`, `vw`, para que o design do seu site possa se adaptar melhor a diferentes tamanhos de tela e configurações de zoom. 

Você pode aprender mais sobre unidades relativas neste [link](https://www.w3schools.com/cssref/css_units.asp).

## JavaScript

Notei que você está usando um alerta no JavaScript para testar se o arquivo está sendo carregado corretamente. Isso é uma boa prática durante o desenvolvimento, mas lembre-se de removê-lo quando você começar a implementar a funcionalidade real no JavaScript.

Agora, então, vamos falar sobre as funcionalidades que ainda precisam ser implementadas no JavaScript. 

Primeiro, você precisa criar uma estrutura de dados (array de objetos) no JavaScript para armazenar as informações das notícias. Cada objeto deve ter um ID único. Esta estrutura de dados será usada para preencher dinamicamente os cards de notícias na página `index.html` e também para exibir os detalhes de uma notícia na página `detalhes.html`.

Depois de criar a estrutura de dados, você precisa usar a manipulação do DOM para criar os cards de notícias dinamicamente na página `index.html`. Cada card deve ter um link para a página `detalhes.html` com o ID da notícia na query string da URL.

Na página `detalhes.html`, você precisa ler o ID da notícia da query string da URL, encontrar a notícia correspondente na estrutura de dados e exibir seus detalhes.

Você pode aprender mais sobre como manipular o DOM neste [link](https://developer.mozilla.org/pt-BR/docs/Web/API/Document_Object_Model/Introduction) e como trabalhar com a estrutura de dados JSON neste [link](https://developer.mozilla.org/pt-BR/docs/Learn/JavaScript/Objects/JSON). E este [tutorial](https://developer.mozilla.org/pt-BR/docs/Web/API/URLSearchParams) pode te ajudar a entender como ler parâmetros da query string da URL.

## Resumo

Em resumo, aqui estão os pontos a serem trabalhados:

1. Tente usar classes em vez de IDs em seu CSS.
2. Use unidades relativas em vez de absolutas em seu CSS.
3. Crie uma estrutura de dados no JavaScript para armazenar as informações das notícias.
4. Use manipulação do DOM para criar dinamicamente os cards de notícias na página `index.html`.
5. Crie links para a página `detalhes.html` com o ID da notícia na query string da URL.
6. Na página `detalhes.html`, leia o ID da notícia da URL, encontre a notícia correspondente na estrutura de dados e exiba seus detalhes.

Espero que estas sugestões sejam úteis para você! Mantenha o ótimo trabalho e continue codificando! 💻🚀


---

### 📝 Resumo dos Pontos de Atenção
| Ação | Tópico | Detalhes do Teste |
|:---|:---|:---|
| Revisar | `link` | **Teste:** `check_internal_links_to_article`<br>**O que ele faz:** *Verifica a existência de um número mínimo de links âncora internos apontando para IDs em tags `<article>`.*<br>**Parâmetros:** <sub>`required_count`: `4`</sub> |
| Revisar | `responsivity` | **Teste:** `uses_relative_units`<br>**O que ele faz:** *Verifica se o arquivo CSS usa unidades relativas como em, rem, %, vh, vw.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `bootstrap_fundamentals` | **Teste:** `has_class`<br>**O que ele faz:** *Verifica a presença de classes CSS específicas, com suporte a curingas, um número mínimo de vezes.*<br>**Parâmetros:** <sub>`class_names`: `['d-flex', 'd-*-flex']`, `required_count`: `1`</sub> |
| Revisar | `dynamic_js` | **Teste:** `js_has_json_array_with_id`<br>**O que ele faz:** *Verifica a existência de um array de objetos JS onde cada objeto possui uma chave específica obrigatória.*<br>**Parâmetros:** <sub>`required_key`: `id`, `min_items`: `3`</sub> |
| Revisar | `dynamic_js` | **Teste:** `js_uses_dom_manipulation`<br>**O que ele faz:** *Verifica se o código JS usa um número mínimo de métodos comuns de manipulação do DOM.*<br>**Parâmetros:** <sub>`methods`: `['createElement', 'appendChild', 'innerHTML', 'querySelector']`, `required_count`: `4`</sub> |
| Revisar | `dynamic_js` | **Teste:** `js_uses_query_string_parsing`<br>**O que ele faz:** *Verifica se o código JavaScript contém padrões para ler query strings da URL.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `linking_and_integrity` | **Teste:** `link_points_to_page_with_query_param`<br>**O que ele faz:** *Verifica a existência de tags âncora que levam a uma página específica com um parâmetro de query string obrigatório.*<br>**Parâmetros:** <sub>`target_page`: `public/detalhes.html`, `query_param`: `id`, `required_count`: `3`</sub> |
| Corrigir (Penalidade) | `html` | **Teste:** `check_id_selector_over_usage`<br>**O que ele faz:** *Conta o número de seletores de ID usados e penaliza se exceder o máximo permitido.*<br>**Parâmetros:** <sub>`max_allowed`: `2`</sub> |
| Corrigir (Penalidade) | `html` | **Teste:** `has_forbidden_tag`<br>**O que ele faz:** *Verifica a presença de uma tag HTML proibida.*<br>**Parâmetros:** <sub>`tag`: `script`</sub> |
| Corrigir (Penalidade) | `project_structure` | **Teste:** `check_dir_exists`<br>**O que ele faz:** *Verifica se um diretório específico existe no envio.*<br>**Parâmetros:** <sub>`dir_path`: `css`</sub> |
| Corrigir (Penalidade) | `project_structure` | **Teste:** `check_dir_exists`<br>**O que ele faz:** *Verifica se um diretório específico existe no envio.*<br>**Parâmetros:** <sub>`dir_path`: `imgs`</sub> |


---
> Caso queira tirar uma dúvida específica, entre em contato com o Chapter.