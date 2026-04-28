# 🏎️ Engenharia de Prompt - Estética Automotiva

## 📝 Descrição do Projeto
Este projeto foi desenvolvido como parte da disciplina **Engenharia de Prompt e Aplicações em IA**. O objetivo principal foi testar a eficiência de um **Prompt Estruturado em XML** na geração de uma página HTML Single Page voltada para o setor de estética automotiva.

O experimento consistiu em submeter o mesmo conjunto de instruções a diversos modelos de linguagem (LLMs) para avaliar critérios como precisão técnica, criatividade e consumo de recursos (tokens).

## 🚀 Tecnologias e Modelos Testados
* **Estrutura de Prompt:** XML para organização de diretrizes.
* **Linguagens Geradas:** HTML5 e CSS3 integrado (Single Page).
* **Modelos Avaliados:** GPT, Gemini, DeepSeek, Qwen, Grok, Maritaca e Claude.

## 📊 Quadro de Análise Comparativa
Abaixo estão os dados coletados durante a execução do protocolo de testes, comparando a performance entre os modelos:

| Critérios de Avaliação | GPT | Gemini | DeepSeek | Qwen | Grok | Maritaca | Claude |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Precisão Estimada** | 95% | 90-95% | 100% | 98-100% | 94% | 100% | 92% |
| **Precisão do HTML** | 96% | 78% | 98% | 100% | 98% | 100% | 94% |
| **Criatividade** | 85% | 95% | 95% | 95% | 87% | 95% | 88% |
| **Tokens Gastos** | 750 | 1450 | 2850 | 1550 | 1100 | 3059 | 6000 |

## 🧠 Reflexão Crítica
Com base nos testes realizados pelos alunos **Rubens da Silva** e **Ana Beatriz Moura Torres**:

1. **Compreensão de Estrutura:** O modelo **Claude** demonstrou a melhor compreensão da estrutura XML proposta.
2. **Variação de Verbosidade:** Houve uma diferença significativa no gasto de tokens para o mesmo resultado, variando de **750 a 6.000 tokens**.
3. **Melhor Escolha:** O **Claude** foi selecionado como a melhor ferramenta para o projeto devido ao seu alto nível de criatividade e precisão na interpretação do prompt estruturado.

## 🔧 Estrutura do Prompt Utilizada
O prompt foi construído seguindo este modelo hierárquico para garantir que a IA seguisse todas as restrições:

```xml
<tarefa>
 <objetivo>Criar uma página HTML5 única com CSS3 interno (single page).</objetivo>
 <tema>estética automotiva</tema>
 <diretrizes_design>
    <layout>Responsivo e minimalista.</layout>
    <paleta_cores>laranja e preto</paleta_cores>
    <tipografia>Sans-serif para títulos, Serif para corpo.</tipografia>
 </diretrizes_design>
 <obrigatoriedades_tecnicas>
    <item>Menu de navegação funcional (âncoras).</item>
    <item>Seção de portfólio ou galeria.</item>
    <item>Rodapé com informações de contato simuladas.</item>
    <item>Carros esportivos</item>
 </obrigatoriedades_tecnicas>
 <metrica_obrigatoria>
    Ao final da resposta, informe uma estimativa de quantos tokens foram gerados.
 </metrica_obrigatoria>
</tarefa>
