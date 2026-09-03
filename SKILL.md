---
name: portugues-natural
description: Remove vícios de linguagem de IA de textos em português brasileiro. Use sempre que escrever, editar ou revisar qualquer texto em pt-BR (respostas, e-mails, posts, artigos, documentação, legendas) para soar como uma pessoa real escreveu, não como um modelo de linguagem traduzido do inglês. Acione mesmo sem pedido explícito de "revisão de estilo" — qualquer geração de texto em português corrido se beneficia disso.
metadata:
  trigger: Escrever ou editar qualquer texto em português brasileiro
---

# Português Natural

Textos de IA em português quase sempre carregam vícios importados do inglês (que soam artificiais em pt-BR) somados a vícios próprios da nossa língua formal — o "português de redação escolar" ou "português de e-mail corporativo". O objetivo aqui não é traduzir as regras do inglês, é atacar os tiques que aparecem especificamente quando o modelo escreve em português.

## Regras Centrais

1. **Travessão é raro fora de diálogo.** IA usa travessão como muleta universal, para quase toda ideia intercalada, quando vírgula, parênteses ou uma frase nova resolveriam melhor. Fora da fala de personagem em narrativa, trate o travessão como recurso raro: praticamente todo aposto ou explicação intercalada se resolve melhor com vírgula, parênteses ou reescrevendo a frase. Se usar mesmo assim, no máximo um por página, e só quando nenhuma outra pontuação resolver. Revise cada um individualmente antes de entregar: um travessão usado como separador preguiçoso (ex.: "MIT — veja LICENSE", onde dois-pontos ou ponto resolvem melhor) deve virar outra pontuação, não é poupado só por ser o único da página.

2. **Não abra parágrafo com conector de manual.** "Além disso", "por fim", "por outro lado", "nesse sentido", "dessa forma", "vale ressaltar", "cabe destacar" — são a assinatura mais óbvia de texto gerado. Ligue as ideias pelo conteúdo, não por advérbio de transição. Veja [regras/conectivos.md](regras/conectivos.md).

3. **Corte adjetivo vazio.** "Fascinante", "incrível", "essencial", "notável", "vasto", "fundamental", "poderoso" — palavras que anunciam importância sem mostrar nada concreto. Se o adjetivo sumir e a frase não perder informação, ele não deveria estar lá. Veja [regras/adjetivos.md](regras/adjetivos.md).

4. **Fuja da fórmula "não é X, é Y".** E das variações "não se trata de X, mas de Y" / "mais do que X, é Y" / "X, não Y" (mesma negação disfarçada, sem o "é" explícito — ex.: "é hábito, não estratégia"). Vire uma vez, no máximo, por texto — nunca estrutura recorrente. Diga Y direto.

5. **Nem tudo é lista.** IA converte qualquer sequência de duas ideias em bullet points. Se as ideias têm uma relação lógica ou temporal, escreva em prosa. Reserve listas para quando a enumeração for realmente o ponto (passos de um processo, itens comparáveis).

6. **Não repita a mesma ideia com sinônimos.** Textos de IA "engordam" reafirmando o que já foi dito com outras palavras, para parecer mais elaborado. Se a segunda frase não acrescenta informação nova, corte-a.

7. **Evite vocabulário etéreo.** "Jornada", "essência", "universo (de possibilidades)", "panorama", "cenário", "trajetória", "protagonismo", "consolidar-se como" — vocabulário de press release que soa grandioso e não diz nada específico. Nomeie a coisa real.

8. **Ponto e vírgula é exceção, não hábito.** Use vírgula ou ponto final na maioria das vezes. Ponto e vírgula só quando dividir de fato duas orações independentes fortemente relacionadas — não para parecer mais formal ou sofisticado.

9. **Tenha posição.** IA tende à neutralidade performática: "por um lado... por outro", "cada abordagem tem seus prós e contras", terminando sem dizer nada. Quando o texto pede uma opinião ou recomendação, dê uma. Reserve o "depende" para quando genuinamente depender — e diga do quê.

10. **Cuidado com o gerúndio decorativo e a voz passiva.** "Vale destacar que...", "sendo assim...", "podendo ser considerado..." engordam a frase sem sujeito agindo. Prefira sujeito + verbo direto: quem fez o quê.

11. **Varie o ritmo.** Frases próprias do "português de redação" alternam sempre no mesmo comprimento e model. Misture frases curtas e longas. Não feche todo parágrafo com uma frase de efeito.

12. **Cuidado com os padrões tipográficos e retóricos reconhecíveis de IA.** Título Com Todas As Palavras Maiúsculas, título com dois-pontos ("Substantivo: gancho chamativo"), maiúscula errada depois de dois-pontos, pergunta retórica em série ("A verdade? ..."), repetição em escadinha ("Você não precisa de X. Você não precisa de Y.") e a fórmula "Sem X. Sem Y. Só Z." são assinaturas visuais que entregam o texto como gerado antes mesmo do conteúdo ser lido. Veja [regras/estruturas.md](regras/estruturas.md) para cada um com exemplos.

13. **Diga a relação direto, sem preposição de manual.** "Em conexão com", "associado a", "relacionado a", "no contexto de" são formas indiretas de descrever um vínculo que quase sempre tem um verbo ou preposição mais simples por trás. Nomeie a relação real (quem fez o quê, o que causa o quê) em vez de só apontar que ela existe. Veja [regras/conectivos.md](regras/conectivos.md).

14. **Evite frase clivada de ênfase forçada.** "O que realmente importa é X", "O horário que funciona é Y", "É aí que X acontece", "Foi isso que resolveu" — construções que separam sujeito e predicado só para simular ênfase. Reescreva na ordem direta: sujeito, verbo, complemento. "O horário que realmente funciona é entre 9h30 e 11h" vira "O melhor horário é entre 9h30 e 11h" ou simplesmente "Funciona melhor entre 9h30 e 11h".

15. **Não afirme importância sem provar.** "Não foi coincidência", "não é à toa", "isso não é aleatório" — frases que reivindicam significância sem mostrar o dado ou o motivo por trás. Ou mostra a causa na mesma frase, ou corta a afirmação.

16. **Não repita o mesmo molde sintático para listar dados.** IA gosta de listar pontos de uma série sempre na mesma forma gramatical, trocando só o dado: "Tomando às 7h, a energia caía às 14h. Adiando para as 10h, o pico durou até a tarde." Mesmo sem repetir palavra, a estrutura idêntica (gerúndio + vírgula + resultado, ou "Em [ano], X. Em [ano], Y.") entrega o texto como gerado — é a mesma lógica da repetição em escadinha (regra 12), só que na sintaxe, não no léxico. Varie a construção de cada frase da série, mesmo contando fatos parecidos.

## Verificação Rápida

Antes de entregar o texto, revise:

- Algum travessão fora de diálogo? Verifique se vírgula, parênteses, dois-pontos ou reescrever a frase não resolvem melhor — na dúvida, tire o travessão. Mais de um na página é sinal quase certo de excesso.
- Algum parágrafo começa com "além disso / por fim / por outro lado / nesse sentido / vale ressaltar"? Reescreva a transição.
- Adjetivo vazio (fascinante, essencial, incrível, notável)? Corte ou substitua pelo dado concreto.
- Estrutura "não é X, é Y" (ou variante sem "é", tipo "X, não Y") mais de uma vez? Elimine a repetição.
- Frase clivada de ênfase forçada ("o que X é Y", "é aí que...", "foi isso que...")? Reescreva na ordem direta.
- Frase que afirma importância/causalidade sem provar ("não foi coincidência", "não é à toa")? Mostre a causa ou corte.
- Duas ou mais frases seguidas listando dados no mesmo molde sintático (mesma ordem de gerúndio/vírgula/resultado, mesmo "Em X, aconteceu Y")? Varie a construção de cada uma.
- Lista de bullets para algo que poderia ser uma frase corrida? Transforme em prosa.
- Duas frases seguidas dizendo a mesma coisa com palavras diferentes? Corte uma.
- Palavra etérea (jornada, essência, panorama, cenário, protagonismo)? Substitua por algo específico.
- Ponto e vírgula usado por hábito, não por necessidade real? Troque por ponto ou vírgula.
- O texto termina sem tomar posição quando deveria? Adicione uma conclusão real.
- Frase sem sujeito agente ("é importante destacar que", "pode-se considerar")? Reescreva com sujeito claro.
- Título Com Todas As Palavras Maiúsculas? Deixe só a primeira maiúscula.
- Pergunta retórica seguida de resposta seca ("A verdade? ...") mais de uma vez no texto? Reduza.
- Título no formato "Substantivo: complemento chamativo"? Considere trocar por afirmação ou pergunta direta.
- Maiúscula logo depois de dois-pontos sem ser citação/enumeração/nome próprio? Corrija para minúscula.
- Frases curtas repetindo a mesma abertura em sequência ("Você não precisa de..." três vezes)? Deixe só uma, se fizer sentido.
- Estrutura "Sem X. Sem Y. Só Z."? Reescreva em prosa normal.
- "Em conexão com / associado a / relacionado a / no contexto de" no lugar de um verbo ou preposição direta? Nomeie a relação real.

## Exemplos

Veja [regras/exemplos.md](regras/exemplos.md) para transformações completas de antes/depois.

## Licença

MIT
