# Português Natural

Skill do Claude Code que remove vícios de linguagem de IA em textos escritos em português brasileiro: o "português traduzido do inglês" e o "português de redação escolar / e-mail corporativo" que entregam um texto como gerado por IA antes mesmo do conteúdo ser lido.

A skill entra em ação sempre que você (ou o Claude) for escrever, editar ou revisar um texto em português corrido: resposta de chat, e-mail, post, artigo, documentação, legenda. Não precisa pedir "revisão de estilo" explicitamente. Ela aplica um conjunto de regras e uma checklist antes de entregar o texto final. Cobre, entre outros:

- Travessão usado como muleta universal
- Conectivos de manual ("além disso", "por fim", "vale ressaltar")
- Adjetivos vazios e vocabulário etéreo ("fascinante", "jornada", "essência")
- A fórmula "não é X, é Y"
- Listas usadas onde prosa serviria melhor
- Redundância disfarçada de elaboração
- Padrões tipográficos reconhecíveis (Título Com Cada Palavra Maiúscula, "A verdade? ...", "Sem X. Sem Y. Só Z.")
- Preposições de conexão vaga ("em conexão com", "associado a")

Depois de limpar os vícios, ela acrescenta traços de texto humano: ritmo irregular, detalhe específico em vez de exemplo genérico, registro coloquial quando o canal permite, palavras menos previsíveis e alguma aresta (um comentário lateral, uma opinião, uma dúvida que fica em aberto).

## O que essa skill não faz

O objetivo aqui é só fazer o texto soar como se uma pessoa tivesse escrito, para quem lê. Não é driblar detector de IA.

Desde agosto de 2026, a Anthropic embute nos modelos Claude uma marca d'água estatística, aplicada na escolha de cada token durante a geração, para cumprir o AI Act da União Europeia. É diferente de vocabulário ou de estilo: nenhuma regra de escrita consegue remover, porque ela não está nas palavras escolhidas, está em como o modelo escolhe cada palavra. Se o texto final sai do Claude, essa marca vai junto, por mais que o texto seja revisado.

## Instalação

Copie a pasta `portugues-natural/` para dentro de `.claude/skills/`, global (`~/.claude/skills/`) ou do projeto (`.claude/skills/` na raiz do repo):

```bash
git clone https://github.com/<seu-usuario>/portugues-natural.git ~/.claude/skills/portugues-natural
```

Se já tem o repo clonado em outro lugar, basta copiar a pasta para um desses destinos.

## Uso

Para forçar o uso manualmente, chame por nome:

```
/portugues-natural
```

## Estrutura

```
portugues-natural/
├── SKILL.md                    # regras centrais e checklist de verificação
├── regras/
│   ├── conectivos.md           # conectivos, aberturas e fechos formulaicos
│   ├── adjetivos.md            # adjetivos vazios e vocabulário etéreo
│   ├── estruturas.md           # padrões tipográficos e retóricos reconhecíveis
│   └── exemplos.md             # transformações completas de antes/depois
└── LICENSE
```

## Licença

MIT. Veja [LICENSE](LICENSE).
