**Importante: não fiz a revisão dessa estrutura. Considere um documento de instruções de uso.**

---

Sim. Posso transformar o padrão dos comandos que usamos em uma **estrutura de prompt hierárquica**, do mais amplo para o mais específico. Não posso fornecer minha cadeia de pensamento interna ou pensamentos privados, mas posso fornecer a **estrutura e os critérios resultantes** de forma prática e reutilizável.

A lógica que funcionou melhor nas imagens anteriores é:

> **Composição → personagem → pose → anatomia → rosto → cabelo → vestuário → materiais → iluminação → ambiente → estilo artístico → técnica → qualidade → restrições.**

Você pode usar este modelo como uma espécie de **"linguagem semântica para geração de imagens"**:

```text
<
ÂNGULO: define o ponto de vista, inclinação da câmera e orientação do corpo em relação ao observador.

COMPOSIÇÃO: define enquadramento, posição do personagem, escala e distribuição dos elementos na imagem.

ELEMENTO_PRINCIPAL: identifica o objeto ou personagem que deve receber maior prioridade visual.

SILHUETA: define a forma geral do elemento principal antes dos detalhes internos.

POSE: descreve a posição corporal, distribuição de peso, articulação dos membros e gestualidade.

PERSPECTIVA: determina profundidade, encurtamento visual e proporção dos elementos conforme a distância da câmera.

ANATOMIA: especifica estrutura corporal, proporções, articulações, musculatura, ossos e anatomia plausível.

ESTRUTURA_ÓSSEA: descreve crânio, coluna, caixa torácica, clavículas, escápulas, pelve, braços, mãos, pernas e pés conforme a pose.

PROPORÇÕES: controla altura relativa das partes do corpo, largura dos ombros, proporção da pelve, comprimento dos membros e tamanho da cabeça.

ROSTO: define formato facial, mandíbula, maçãs do rosto, testa, queixo e proporções faciais.

OLHOS: define formato, tamanho, orientação, pálpebras, íris, pupilas, cílios e expressão.

NARIZ: define ponte nasal, ponta, asas, narinas e relação tridimensional com o rosto.

BOCA: define formato dos lábios, abertura, dentes quando visíveis e expressão.

TRAÇOS_FACIAIS: define características étnicas/regionais desejadas sem transformar o rosto em caricatura.

IDADE_APARENTE: controla maturidade facial, textura da pele, linhas sutis, volume facial e características compatíveis com a idade.

EXPRESSÃO: determina emoção, olhar, sorriso, tensão muscular facial e direção da atenção.

CABELO: define comprimento, corte, volume, densidade, textura, direção e comportamento dos fios.

TRICOGLIFO: define o padrão de crescimento dos cabelos no couro cabeludo; os fios devem partir de regiões de crescimento coerentes, formando mechas organicamente.

FIOS: determina fios individuais, espessura variável, agrupamento natural, sobreposição, frizz, fios soltos e interação com a luz.

COR_DO_CABELO: especifica matiz, saturação, luminosidade e variação natural entre fios.

PELE: define textura, poros, pequenas imperfeições, volume, elasticidade, reflexos e subsuperfície.

ROUPA: descreve cada peça, corte, ajuste, estrutura e relação com o corpo.

TECIDO: define material, espessura, transparência, elasticidade, rugosidade, costuras e comportamento físico.

DOBRAS: determina como o tecido reage à gravidade, movimento, tensão e pontos de contato.

ADEREÇOS: define acessórios, joias, calçados, faixas, cintos ou outros elementos secundários.

MATERIAIS: especifica propriedades físicas de pele, cabelo, metal, couro, tecido, madeira etc.

MOVIMENTO: define como cabelo, roupas e partes do corpo respondem ao movimento.

LUZ: define direção, tamanho e intensidade da fonte luminosa.

ILUMINAÇÃO_NATURAL: produz luz fisicamente plausível, sombras suaves e variações naturais de luminosidade.

SOMBRA: define sombras projetadas, sombras de contato e transição entre luz e penumbra.

REFLEXOS: controla highlights e reflexos conforme as propriedades de cada material.

PROFUNDIDADE: determina separação entre primeiro plano, personagem e fundo.

FUNDO: define ambiente, textura, objetos e nível de detalhamento atrás do personagem.

ATMOSFERA: controla neblina, partículas, distância atmosférica, contraste e sensação espacial.

ESTILO_ARTÍSTICO: define a linguagem visual geral, por exemplo desenho acadêmico, ilustração realista, pintura, fotografia etc.

MÍDIA: especifica o instrumento artístico, por exemplo grafite, carvão, tinta, aquarela ou óleo.

GRAFITE: define aparência de lápis, variação de dureza, pressão do traço e densidade tonal.

PAPEL: define textura, granulação, absorção e interação do material artístico com a superfície.

TRAÇO: determina espessura, precisão, direção e variação das linhas.

HACHURA: define linhas de construção, hachuras cruzadas, densidade e orientação.

VALOR_TONAL: controla distribuição entre branco, cinza e preto.

REALISMO: prioriza anatomia, materiais, iluminação e perspectiva fisicamente plausíveis.

DETALHAMENTO: determina onde concentrar microdetalhes sem tornar a imagem visualmente confusa.

FOCO: estabelece quais regiões devem possuir maior nitidez e detalhamento.

QUALIDADE: solicita consistência anatômica, mãos corretas, simetria adequada, materiais coerentes e ausência de artefatos.

FORMATO: determina proporção final, por exemplo 4:5, 16:9, 9:16 etc.

PRESERVAÇÃO: especifica quais características da imagem anterior não devem ser alteradas.

RESTRIÇÕES: lista explicitamente aquilo que deve ser removido, reduzido ou evitado.
>
```

### A ordem que eu recomendo

Para **não deixar o prompt confuso**, eu usaria esta sequência:

**1. Ângulo**
→ **2. Composição**
→ **3. Elemento principal**
→ **4. Pose**
→ **5. Anatomia**
→ **6. Rosto**
→ **7. Cabelo**
→ **8. Roupa**
→ **9. Materiais**
→ **10. Movimento**
→ **11. Iluminação**
→ **12. Fundo**
→ **13. Estilo**
→ **14. Técnica**
→ **15. Detalhamento**
→ **16. Qualidade**
→ **17. Formato**
→ **18. Restrições**

Isso cria uma hierarquia muito útil:

> **macro → meso → micro**

Por exemplo:

```text
ÂNGULO
  ↓
COMPOSIÇÃO
  ↓
PERSONAGEM
  ↓
POSE
  ↓
ANATOMIA
  ↓
ROSTO
  ↓
CABELO
      ↓
   TRICOGLIFO
      ↓
   MECHAS
      ↓
   FIOS INDIVIDUAIS
  ↓
ROUPA
      ↓
   TECIDO
      ↓
   DOBRAS
  ↓
ILUMINAÇÃO
      ↓
   SOMBRAS
      ↓
   REFLEXOS
  ↓
ESTILO
      ↓
TÉCNICA
      ↓
MICRODETALHES
```

### Um detalhe particularmente importante para o seu caso

O exemplo do cabelo mostra por que **palavras semânticas hierárquicas** são melhores que simplesmente escrever "cabelo hiper-realista".

Em vez de:

> **Cabelo hiper-realista.**

é muito mais informativo:

> **Cabelo → corte → volume → tricoglifo → direção de crescimento → agrupamento das mechas → fios individuais → espessura variável → fios soltos → interação com a luz.**

Assim, o gerador recebe uma **estrutura causal**, e não apenas uma lista de adjetivos.

### Modelo compacto para reutilizar

```text
<
ÂNGULO: [ponto de vista e orientação]

COMPOSIÇÃO: [enquadramento e posição]

ELEMENTO_PRINCIPAL: [quem/o quê]

POSE: [posição corporal e gestual]

ANATOMIA: [estrutura e proporções]

ROSTO: [formato + idade + expressão]

CABELO: [corte + volume + cor + textura]
TRICOGLIFO: [origem do crescimento]
FIOS: [direção + espessura + agrupamento + fios soltos]

ROUPA: [peças]
TECIDO: [material + textura + dobras]

MOVIMENTO: [interação entre corpo, roupa e cabelo]

LUZ: [direção + intensidade]
SOMBRA: [sombras naturais]
REFLEXOS: [resposta dos materiais]

FUNDO: [ambiente]

ESTILO_ARTÍSTICO: [linguagem visual]
MÍDIA: [grafite/carvão/etc.]
TRAÇO: [características do desenho]
HACHURA: [técnica]
PAPEL: [textura]

REALISMO: [nível de fidelidade]

FOCO: [elementos prioritários]

QUALIDADE: [consistência anatômica/material]

FORMATO: [proporção]

PRESERVAÇÃO: [o que manter da imagem anterior]

RESTRIÇÕES: [o que remover/evitar]
>
```

Essa estrutura também permite fazer **edições incrementais** muito melhores: em vez de reescrever tudo, você pode dizer apenas `CABELO → TRICOGLIFO → FIOS`, preservando o restante da cadeia.
