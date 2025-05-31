# 🤖 Chatbot EndoLog Store

## Descrição

O **Chatbot EndoLog Store** é um assistente virtual inteligente desenvolvido em Python para simular o atendimento ao cliente de uma loja de tecnologia. O sistema utiliza processamento de linguagem natural para compreender as solicitações dos usuários e fornecer respostas contextualizadas sobre produtos, serviços e informações da loja.

## 🎯 Funcionalidades

- **Consulta de Produtos**: Visualização completa do catálogo organizado por categorias
- **Sistema de Recomendação**: Sugestões personalizadas baseadas na categoria de interesse
- **FAQ Automatizado**: Respostas instantâneas para perguntas frequentes
- **Informações da Loja**: Localização, horários e contatos de suporte
- **Transferência para Atendente**: Escalação para atendimento humano quando necessário
- **Interface Intuitiva**: Menu visual com emojis e navegação simplificada

## 🛠️ Tecnologias Utilizadas

- **Python 3.x**
- **spaCy** - Processamento de linguagem natural
- **Biblioteca random** - Sistema de recomendações
- **Biblioteca time** - Simulação de delays realistas

## 📋 Pré-requisitos

Antes de executar o chatbot, certifique-se de ter instalado:

```bash
# Python 3.6 ou superior
python --version

# spaCy
pip install spacy

# Modelo de linguagem portuguesa
python -m spacy download pt_core_news_sm
```

## 🚀 Como Executar

1. **Clone ou baixe o arquivo do chatbot**
```bash
# Se usando Git
git clone [url-do-repositorio]
cd chatbot-endolog
```

2. **Execute o programa**
```bash
python chatbot.py
```

3. **Interaja com o chatbot**
   - Siga as instruções apresentadas no menu
   - Digite suas perguntas em linguagem natural
   - Use comandos como "ajuda" para voltar ao menu principal

## 💬 Exemplos de Uso

```
Você: Olá, bom dia!
Bot: 🤖 Olá! Em que posso ajudá-lo(a)?

Você: Quais produtos vocês têm?
Bot: 🔍 Confira nossos produtos disponíveis no momento:
     🗂️ Celular:
        - Apple iPhone 14
        - Samsung Galaxy S23
        - Motorola Edge 30 Neo

Você: Me recomenda um notebook
Bot: 👍 Ótima escolha! Baseado na categoria 'notebook', 
     recomendamos: *Dell XPS 13 Plus*.

Você: Onde fica a loja?
Bot: 📍 Nossa loja fica na Rua do Sol, nº 266 - Recife - PE, 
     CEP: 53250-320.
```

## 📂 Estrutura do Projeto

```
chatbot-endolog/
│
├── chatbot.py              # Arquivo principal do chatbot
├── README.md              # Este arquivo
```

## 🔧 Funcionalidades Detalhadas

### Reconhecimento de Intenções
O chatbot identifica as seguintes intenções do usuário:
- Saudações
- Consulta de produtos
- Solicitação de recomendações
- Perguntas sobre localização
- Informações sobre horários
- Suporte técnico
- Status de pedidos
- Transferência para atendente
- Encerramento da conversa

### Base de Produtos
Categorias disponíveis:
- **Celulares**: iPhone 14, Galaxy S23, Motorola Edge 30 Neo
- **Notebooks**: Dell XPS 13 Plus, MacBook Air M2, ThinkPad X1 Carbon
- **Acessórios**: Fone JBL, Carregador Samsung, Mouse Logitech

### Informações da Loja
- **Endereço**: Rua do Sol, nº 266 - Recife - PE
- **Horário**: Segunda a sexta (08h-18h), Sábado (08h-12h)
- **Suporte**: suporte@endolog.com | (81) 4002-9230

## 🎨 Personalização

Para personalizar o chatbot:

1. **Adicionar novos produtos**:
```python
produtos = {
    "celular": ["Seu novo produto aqui"],
    # ... outras categorias
}
```

2. **Modificar informações da loja**:
```python
faq = {
    "localizacao": "Seu novo endereço aqui",
    # ... outras informações
}
```

3. **Adicionar novas intenções**:
```python
def entender_intencao(texto):
    # Adicione suas novas condições aqui
```

## 🐛 Resolução de Problemas

**Erro: "Can't find model 'pt_core_news_sm'"**
```bash
python -m spacy download pt_core_news_sm
```

**Erro: "ModuleNotFoundError: No module named 'spacy'"**
```bash
pip install spacy
```

## 📈 Possíveis Melhorias

- [ ] Interface gráfica (Tkinter/Flask)
- [ ] Integração com base de dados real
- [ ] Sistema de aprendizado incremental
- [ ] Análise de sentimento
- [ ] API de produtos em tempo real
- [ ] Histórico de conversas
- [ ] Múltiplos idiomas

## 👥 Contribuição

Contribuições são bem-vindas! Para contribuir:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-funcionalidade`)
3. Commit suas mudanças (`git commit -am 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/nova-funcionalidade`)
5. Abra um Pull Request

