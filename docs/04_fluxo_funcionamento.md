# FLUXO DE FUNCIONAMENTO

## Visão geral

O sistema opera em estados definidos, controlados pela unidade eletrônica.

---

## Estados do sistema

### 1. Desligado
Sistema inativo, aguardando interação do usuário.

---

### 2. Inicialização
- Inicialização do microcontrolador
- Verificação de sensores
- Checagem básica de segurança

---

### 3. Configuração
Usuário define:
- Tempo de operação
- Nível de compressão

---

### 4. Início
- Bomba de água é ativada
- Sistema aguarda estabilização do fluxo
- Compressão é iniciada

---

### 5. Operação

#### Sistema térmico
- Bomba permanece ligada continuamente
- Água gelada circula pelo sistema

#### Sistema pneumático
Ciclo de compressão:

1. Inflar (compressor ligado)
2. Manter pressão
3. Desinflar (válvula de alívio)
4. Espera
5. Repetição

---

### 6. Controle de tempo
- Contagem regressiva
- Ao atingir zero, sistema encerra operação

---

### 7. Finalização
- Compressor desligado
- Bomba desligada
- Pressão liberada
- Sistema retorna ao estado inicial

---

### 8. Tratamento de erros

O sistema deve interromper operação em caso de:

- Falha na bomba
- Pressão fora dos limites
- Problemas de circulação
- Condições inseguras

---

## Observações

- Sistema térmico não possui controle ativo de temperatura
- Compressão é controlada por tempo e/ou pressão
- Projeto focado em simplicidade para protótipo V1
