# Aluguel

## Previsão de Custos de Aluguel de Imóveis

Este projeto tem como objetivo prever os custos de aluguel de imóveis com base em diversos fatores.

## Entendimento do Problema

Muitos fatores influenciam o valor que você pagará pelo aluguel de um imóvel. É importante entender o que afeta essa variação de preço, tanto para cima quanto para baixo. Abaixo, listamos alguns dos principais fatores que podem impactar os custos de aluguel.

Entre os atributos considerados neste estudo estão:

- Área do imóvel (em metros quadrados)
- Número de quartos
- Número de banheiros
- Vagas na garagem
- Andar do imóvel
- Aceita animais
- Imóvel mobiliado
- Valor do condomínio
- Valor do aluguel
- Valor do IPTU
- Valor do seguro

Esses fatores desempenham papéis importantes na determinação do preço final do aluguel e serão analisados no modelo de machine learning para prever o custo com base nesses atributos.

## Resultados do Modelo de Regressão Linear

1. **EQM com Apenas Área:** R$ 11,059,335.47
   - Este valor indica que, em média, as previsões do modelo que considera apenas a área do imóvel estão distantes dos valores reais de aluguel.

2. **EQM com Área e Mobiliado:** R$ 10,846,667.20
   - A inclusão da variável "Mobiliado" resultou em uma melhoria no modelo, reduzindo o EQM em R$ 212,668.27. Isso sugere que o status de mobiliado tem um impacto significativo no valor do aluguel, permitindo que o modelo faça previsões mais precisas.

3. **EQM com Área, Mobiliado e Quartos:** R$ 7,526,800.07
   - A adição da variável "Número de Quartos" resultou em uma nova redução do EQM, indicando que este modelo é o mais eficaz entre os três testados. O EQM significativamente menor sugere que a inclusão do número de quartos melhora ainda mais a capacidade do modelo de prever o valor do aluguel.

### Interpretação dos Resultados

- **Melhoria Progressiva:** A análise dos EQMs mostra uma melhoria progressiva na precisão das previsões à medida que mais variáveis são incluídas no modelo. A diferença entre os EQMs indica que tanto a variável "Mobiliado" quanto a variável "Número de Quartos" têm um papel importante na determinação do valor do aluguel.

- **Conclusão Final:** O modelo que inclui "Área", "Mobiliado" e "Número de Quartos" é o mais robusto, com um EQM de R$ 7,526,800.07. Isso significa que, em média, as previsões do valor do aluguel estão mais próximas dos valores reais, o que é crucial para decisões informadas em investimentos imobiliários e estratégias de precificação.

---
