# BASE CIENTÍFICA

## Objetivo

Este documento reúne a base científica inicial para orientar o desenvolvimento de um sistema portátil de crioterapia com compressão pneumática aplicado ao joelho.

O foco é definir parâmetros seguros, efeitos fisiológicos e implicações de engenharia para o protótipo V1.

---

## 1. Efeitos fisiológicos do frio

A crioterapia reduz a temperatura dos tecidos superficiais, promovendo:

- analgesia (redução da dor)
- diminuição do metabolismo local
- redução da inflamação
- vasoconstrição

Estudos indicam que:

- analgesia ocorre por volta de **13–14 °C na pele**
- redução da condução nervosa ocorre próximo de **12,5 °C**

Isso explica o efeito terapêutico do frio, mas também mostra que temperaturas muito baixas aumentam o risco de lesão.

Referência:
- Kennet J. et al. (2007)

---

## 2. Evidência clínica em joelho

A literatura recente indica que a crioterapia é eficaz principalmente em:

- redução de dor pós-operatória
- redução de edema
- melhora da mobilidade inicial

Uma revisão sistemática de 2024 mostrou benefícios na reabilitação após artroplastia total de joelho.

Referência:
- Liang Z. et al. (2024)

---

## 3. Crioterapia com compressão

A combinação de frio com compressão pneumática apresenta vantagens em relação ao uso isolado de frio.

Estudos mostram:

- melhor controle de edema
- melhora funcional inicial
- redução de dor em movimento

Referência:
- Quesnot A. et al. (2024)
- Song M. et al. (2016)

---

## 4. Faixa térmica terapêutica

Estudos com dispositivos de criocompressão indicam que:

- a faixa ideal de temperatura da pele é **10–15 °C**

Essa faixa proporciona efeito terapêutico com menor risco.

Importante:

- temperatura da água ≠ temperatura da pele
- há perda térmica no sistema

Referência:
- Belsey J. et al. (2024)

---

## 5. Temperaturas extremas e risco

Temperaturas muito baixas podem causar:

- queimadura por frio
- dano nervoso
- lesão tecidual

Estudos indicam que:

- temperaturas muito baixas não aumentam necessariamente o benefício clínico
- valores moderados são mais seguros e eficazes

Referência:
- Cryotherapy and thermotherapy review (2024)
- Kennet J. et al. (2007)

---

## 6. Compressão pneumática

A compressão auxilia em:

- drenagem linfática
- retorno venoso
- redução de edema

Porém:

- deve ser controlada
- não deve ser excessiva

Referência:
- Quesnot A. et al. (2024)

---

## 7. Implicações de engenharia

Para o projeto V1:

- não controlar apenas temperatura da água
- considerar efeito na pele
- usar limites conservadores
- implementar temporização obrigatória
- limitar pressão

---

## 8. Requisitos preliminares de segurança

Para o protótipo:

- limitar tempo de uso (até 30 min)
- limitar pressão
- desligamento automático
- evitar temperaturas extremas
- validar comportamento real em testes

---

## 9. Limites adotados no projeto V1

### Temperatura
- alvo: 10–15 °C (na pele)
- operação da água: controlada (não extrema)

### Pressão
- faixa conservadora (abaixo do máximo comercial)

### Tempo
- até 30 minutos por sessão

Base adicional:
- Manual do Game Ready GRPro 2.1:
  - temperatura: 4,5 °C a 15,5 °C
  - pressão: 5–75 mmHg

---

## 10. Conclusão

A literatura científica apoia o uso de crioterapia para reabilitação de joelho, especialmente no controle de dor e edema.

A combinação com compressão apresenta benefícios adicionais.

Para engenharia do produto, os fatores críticos são:

- controle indireto da temperatura da pele
- limites seguros de pressão
- controle de tempo
- abordagem conservadora no V1

---

## Referências

1. Liang Z. et al. Cryotherapy for Rehabilitation After Total Knee Arthroplasty: A Comprehensive Systematic Review and Meta-Analysis. 2024.

2. Belsey J. et al. A randomised crossover trial of five cryocompression devices' ability to reduce skin temperature of the knee. 2024.

3. Quesnot A. et al. Randomized controlled trial of compressive cryotherapy versus cryotherapy alone after total knee arthroplasty. 2024.

4. Kennet J. et al. Cooling Efficiency of 4 Common Cryotherapeutic Agents. Journal of Athletic Training. 2007.

5. Song M. et al. Compressive cryotherapy versus cryotherapy alone in patients undergoing knee surgery: a meta-analysis. 2016.

6. Ni SH. et al. Cryotherapy on postoperative rehabilitation of joint arthroplasty. 2014.

7. Game Ready GRPro 2.1 — Manual do usuário.
