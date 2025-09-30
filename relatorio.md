# Relatório de Desempenho - Portal de Notícias Dinâmico
<sup>Este é um feedback gerado por IA e pode conter erros. Você tem 9 créditos restantes.</sup>

Olá, **rommelcarneiro**! Aqui está um feedback detalhado sobre sua atividade.
> **Nota Final:** **`48.66 / 100`**
---
# Feedback do Code Review

Olá, colega! Parabéns pelo esforço que você colocou no seu projeto até agora! Vamos passar por algumas áreas que precisam de aprimoramento e eu vou oferecer algumas sugestões para te ajudar a melhorar ainda mais seu código.

## Pontos de Atenção 🚩

Primeiramente, percebi que seu arquivo `public/detalhes.html` está faltando. Não se esqueça de que você precisa de uma página de detalhes para exibir o conteúdo completo de uma notícia. Essa página deve ser capaz de ler o 'id' da URL, encontrar o item correspondente na estrutura de dados e exibir suas informações.

Em segundo lugar, a estrutura de dados em seu arquivo `app.js` não está correta. Você precisa criar um array de objetos, onde cada objeto representa uma notícia e possui um 'id'. Se tiver dúvidas sobre como fazer isso, confira [este tutorial](https://developer.mozilla.org/pt-BR/docs/Learn/JavaScript/Objects/JSON).

Terceiro, você precisa usar a manipulação do DOM para renderizar os cards de notícias na sua página inicial de forma dinâmica. Isso significa que você precisa criar elementos HTML em seu JavaScript e preenchê-los com dados de suas notícias. Se você não tem certeza de como fazer isso, [este guia](https://developer.mozilla.org/pt-BR/docs/Web/API/Document_Object_Model/Introduction) pode te ajudar.

Por último, cada card de notícia na sua página inicial deve ter um link que aponte para a página de detalhes, com o 'id' da notícia na query string (por exemplo, `detalhes.html?id=1`). Isso permitirá que a página de detalhes saiba qual notícia exibir. Para fazer isso, você precisará usar [URLSearchParams](https://developer.mozilla.org/pt-BR/docs/Web/API/URLSearchParams) para ler os parâmetros da URL.

## Oportunidades de Melhoria 💡

Em relação ao CSS, notei que você usou medidas absolutas (como `px`) em vez de medidas relativas (como `em`, `rem`, `%`, `vh`, `vw`). Recomendo que você mude para medidas relativas, pois elas tornarão seu design mais flexível e melhor adaptado a diferentes tamanhos de tela.

Além disso, percebi que você usou seletores de ID em seu CSS mais do que o recomendado. Embora os IDs sejam úteis para referenciar elementos específicos em seu JavaScript, eles podem tornar seu CSS difícil de manter e reutilizar, pois têm uma especificidade muito alta. Recomendo que você mude para o uso de classes sempre que possível.

## Coisas que você fez bem! 🎉

Quero destacar alguns aspectos positivos do seu trabalho:

- Muito bem ao garantir que todas as suas imagens tenham um atributo `alt`! Isso é ótimo para a acessibilidade.
- Parabéns por configurar corretamente as tags `meta` e `title` no cabeçalho do seu HTML! Isso é importante para a otimização de mecanismos de busca (SEO).
- Você fez um ótimo trabalho ao usar classes em seus elementos HTML! Isso torna seu CSS mais reutilizável e fácil de manter.

Espero que este feedback seja útil para você! Lembre-se de que a prática leva à perfeição. Continue trabalhando duro e você verá melhorias constantes. 🚀

---

### 📝 Resumo dos Pontos de Atenção
| Ação | Tópico | Detalhes do Teste |
|:---|:---|:---|
| Revisar | `link` | **Teste:** `check_internal_links_to_article`<br>**O que ele faz:** *Verifica a existência de um número mínimo de links âncora internos apontando para IDs em tags `<article>`.*<br>**Parâmetros:** <sub>`required_count`: `4`</sub> |
| Revisar | `responsivity` | **Teste:** `uses_relative_units`<br>**O que ele faz:** *Verifica se o arquivo CSS usa unidades relativas como em, rem, %, vh, vw.*<br>**Parâmetros:** <sub>N/A</sub> |
| Revisar | `style` | **Teste:** `has_style`<br>**O que ele faz:** *Verifica se uma regra de estilo CSS específica aparece um número mínimo de vezes.*<br>**Parâmetros:** <sub>`style`: `text-align`, `required_count`: `1`</sub> |
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