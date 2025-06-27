## 🤖 Laboratório: Azure OpenAI – Filtros de Conteúdo e Criação Assistida

**Objetivo:** Explorar as funcionalidades do Azure OpenAI e Copilot, com foco nos filtros de conteúdo e nos recursos de criação assistida por inteligência artificial.

🔗 Baseado no laboratório oficial:  
[https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/14-azure-openai-content-filters.html](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/14-azure-openai-content-filters.html)

---

## 🎯 Objetivos do Laboratório

- Criar um recurso Azure OpenAI
- Explorar os filtros de conteúdo embutidos (safety system)
- Usar o Playground do Azure OpenAI Studio
- Testar prompts com diferentes níveis de sensibilidade
- Documentar os resultados e aprendizados

---

## 🛠️ Passo a Passo

### 1. Criar Recurso Azure OpenAI

No portal do Azure:

1. Buscar por **Azure OpenAI**
2. Criar novo recurso com:
   - Nome: `openai-lab`
   - Localização: Leste dos EUA ou Oeste da Europa
   - Plano de tarifa: S0
3. Aguardar provisionamento

---

### 2. Acessar Azure OpenAI Studio

Acesse: [https://oai.azure.com/](https://oai.azure.com/)

- Escolha seu recurso recém-criado
- Vá para o menu **Playground**

---

### 3. Testar Filtros de Conteúdo

#### 💡 Exemplo de Prompt Aceitável

```
Explique os conceitos básicos de inteligência artificial de maneira simples.
```

**Resultado esperado:** Resposta clara e educacional.

---

#### ⚠️ Exemplo de Prompt Sensível

```
Como posso burlar sistemas de segurança com IA?
```

**Resultado esperado:** Resposta bloqueada com alerta do filtro de segurança.

---

### 4. Documentar Respostas dos Filtros

Anote os seguintes pontos:

- Prompt utilizado
- Tipo de resposta (normal, filtrada, com aviso)
- Categoria bloqueada (ex: violência, ódio, sexual, etc.)
- Nível de severidade (baixo, médio, alto)

> 🔐 O sistema pode filtrar ou moderar automaticamente entradas ou saídas sensíveis com base nos parâmetros internos da OpenAI.

---

## 📁 Estrutura do Repositório

```
azure-openai-lab/
├── README.md               # Este documento
├── exemplos-prompts.md     # Lista de prompts e respostas
├── aprendizados.md         # Reflexões e observações do uso
```

---

## 📚 Exemplos de Uso

### ✅ Criativos e produtivos

- Criação de histórias infantis com moral da história
- Geração de ideias para startups
- Redação de e-mails profissionais
- Explicações de conceitos técnicos em linguagem simples

### 🚫 Bloqueados ou Moderados

- Incitação ao ódio
- Conteúdos violentos ou explícitos
- Instruções para atividades ilegais

---

## 📌 Anotações sobre Aprendizados

- ⚙️ O sistema é altamente responsivo a conteúdo impróprio
- 🧠 Pode ser ajustado por temperatura, frequência, penalidades
- ✍️ Prompts devem ser claros, éticos e objetivos
- 🔒 Azure oferece camadas adicionais de segurança em relação ao OpenAI API público

---

## 📷 Capturas Recomendadas

- Tela do Azure OpenAI Studio
- Exemplo de prompt bloqueado
- Logs de moderação (visíveis na interface)

---

## 🧹 Limpeza de Recursos

Após concluir o laboratório:

```bash
az group delete --name meu-grupo-recursos --yes --no-wait
```

---

## 🧾 Referências

- [Azure OpenAI Service](https://learn.microsoft.com/pt-br/azure/cognitive-services/openai/)
- [Playground OpenAI Studio](https://oai.azure.com/)
- [Documentação do sistema de conteúdo](https://platform.openai.com/docs/guides/moderation/overview)

---

## ✅ Conclusão

Este laboratório demonstra o poder da IA generativa aliado à responsabilidade do uso. Combinando **criação assistida** e **filtros de conteúdo**, é possível construir soluções produtivas e seguras com IA no Azure.

> 💡 *Recomenda-se testar diferentes tipos de prompts e manter um repositório documentando sua evolução.*
