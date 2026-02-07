# 🐍 Quiz Python - Clube de Código CICF

## 📖 Sobre o Projeto

Este é um projeto educativo desenvolvido para o **Clube de Código do Centro de Inovação Carlos Fiolhais**, que permite aos participantes criarem os seus próprios quizzes em Python de forma interativa e divertida!

### ✨ O que faz este projeto?

- **Editor de Código Integrado**: Escreve código Python diretamente no navegador
- **Análise Automática**: O sistema lê o teu código e extrai automaticamente as perguntas e respostas
- **Quiz Interativo**: Executa o quiz numa interface bonita e divertida com emojis
- **Feedback Instantâneo**: Recebe feedback imediato se acertaste ou erraste
- **Pontuação Final**: Vê quantas perguntas acertaste com animações e confetti! 🎊

---

## 🚀 Como Usar

1. **Abre o ficheiro `quiz-builder.html`** no teu navegador
2. **Escreve o teu código Python** no editor à direita (ou usa o exemplo abaixo)
3. **Clica no botão "🚀 Executar Quiz"**
4. **Responde às perguntas** que aparecem na janela popup
5. **Vê a tua pontuação!** 🏆

---

## 💡 Exemplo de Quiz (3 Perguntas)

Copia e cola este código no editor para testares:

```python
pontos = 0
print('🎯 Bem-vindo ao Quiz de Cultura Geral! 🎯')
print('Boa sorte! 🍀')
print()

# Pergunta 1 - Geografia
resposta1 = input('Qual é a capital de França? ')
if resposta1.lower() == 'paris':
    print('✅ Correto! Paris é a Cidade Luz!')
    pontos += 1
else:
    print('❌ Errado! A resposta correta é Paris.')
print()

# Pergunta 2 - Astronomia
resposta2 = input('Quantos planetas existem no Sistema Solar? ')
if resposta2 == '8':
    print('✅ Correto! São 8 planetas desde 2006!')
    pontos += 1
else:
    print('❌ Errado! A resposta correta é 8.')
print()

# Pergunta 3 - Informática
resposta3 = input('Qual é a linguagem de programação deste quiz? ')
if resposta3.lower() == 'python':
    print('✅ Correto! Python é incrível! 🐍')
    pontos += 1
else:
    print('❌ Errado! A resposta correta é Python.')
print()

# Resultado Final
print('=' * 40)
print(f'🏆 Pontuação Final: {pontos}/3')
if pontos == 3:
    print('🌟 Perfeito! És um génio! 🌟')
elif pontos == 2:
    print('👍 Muito bom! Quase lá!')
elif pontos == 1:
    print('💪 Continua a praticar!')
else:
    print('📚 Estuda mais e tenta outra vez!')
print('=' * 40)
```

---

## 🔄 Exemplo Avançado com Ciclo `for` (5 Perguntas)

Copia e cola este código para veres como usar um ciclo `for`:

```python
pontos = 0
total_perguntas = 5

print('🎮 Quiz de Conhecimentos Gerais - Versão Pro! 🎮')
print('Responde a 5 perguntas e testa os teus conhecimentos!')
print('=' * 50)
print()

# Lista de perguntas e respostas
perguntas = [
    'Qual é o maior oceano do mundo? ',
    'Em que ano começou a Segunda Guerra Mundial? ',
    'Qual é o planeta mais próximo do Sol? ',
    'Quem pintou a Mona Lisa? ',
    'Qual é a capital de Portugal? '
]

respostas_corretas = ['pacífico', '1939', 'mercúrio', 'leonardo da vinci', 'lisboa']

respostas_alternativas = [
    ['pacífico', 'pacifico'],  # Aceita com e sem acento
    ['1939'],
    ['mercúrio', 'mercurio'],  # Aceita com e sem acento
    ['leonardo da vinci', 'da vinci', 'leonardo'],  # Aceita várias formas
    ['lisboa']
]

# Ciclo for para fazer todas as perguntas
for i in range(total_perguntas):
    print(f'📌 Pergunta {i + 1}/{total_perguntas}')
    resposta = input(perguntas[i])
    
    # Verifica se a resposta está correta
    if resposta.lower() in respostas_alternativas[i]:
        print('✅ Correto! Muito bem! 🎉')
        pontos += 1
    else:
        print(f'❌ Errado! A resposta correta é: {respostas_corretas[i]}')
    
    print('-' * 50)
    print()

# Resultado Final com mensagens personalizadas
print('=' * 50)
print(f'🏆 RESULTADO FINAL: {pontos}/{total_perguntas}')
print('=' * 50)

# Percentagem
percentagem = (pontos / total_perguntas) * 100

if percentagem == 100:
    print('🌟 PERFEITO! És um verdadeiro génio! 🌟')
    print('🎊 Acertaste TODAS as perguntas! 🎊')
elif percentagem >= 80:
    print('🎉 EXCELENTE! Estás muito bem preparado!')
elif percentagem >= 60:
    print('👍 BOM TRABALHO! Continua assim!')
elif percentagem >= 40:
    print('💪 RAZOÁVEL! Podes melhorar!')
else:
    print('📚 Precisas estudar mais! Não desistas!')

print(f'📊 Percentagem de acerto: {percentagem:.0f}%')
print('=' * 50)
```

### 🎯 O que este exemplo ensina:

- **Listas** para guardar múltiplas perguntas e respostas
- **Ciclo `for`** com `range()` para repetir código
- **Indexação** com `[i]` para aceder a elementos das listas
- **Operador `in`** para verificar se a resposta está numa lista de opções
- **Cálculo de percentagem** para dar feedback mais detalhado
- **Condições múltiplas** com `if/elif/else`

---

## 📚 Como Criar o Teu Próprio Quiz

### Passo 1: Inicializa os pontos
```python
pontos = 0
```

### Passo 2: Cria uma pergunta com `input()`
```python
resposta1 = input('A tua pergunta aqui? ')
```

### Passo 3: Verifica a resposta com `if`
```python
if resposta1.lower() == 'resposta correta':
    print('✅ Correto!')
    pontos += 1
else:
    print('❌ Errado!')
```

### Passo 4: Repete para mais perguntas
Copia e adapta o código acima para quantas perguntas quiseres!

### Passo 5: Mostra a pontuação final
```python
print(f'Pontuação final: {pontos}/total 🏆')
```

---

## 🎨 Funcionalidades do Sistema

### ✅ O que o sistema reconhece:
- Perguntas feitas com `input()`
- Respostas verificadas com `if ... ==`
- Texto dentro das aspas das perguntas
- Respostas corretas esperadas

### 💡 Dicas Importantes:

1. **Usa `.lower()`** nas respostas de texto para aceitar maiúsculas e minúsculas:
   ```python
   if resposta.lower() == 'lisboa':
   ```

2. **Para números**, não uses `.lower()`:
   ```python
   if resposta == '8':
   ```

3. **Adiciona emojis** para tornar o quiz mais divertido! 🎉

4. **Usa `print()` vazio** para dar espaço entre perguntas:
   ```python
   print()
   ```

---

## 🎯 Ideias de Temas para Quizzes

- 🌍 Geografia (capitais, países, continentes)
- 🔬 Ciências (física, química, biologia)
- 📚 Literatura (autores, livros, personagens)
- ⚽ Desporto (jogadores, equipas, recordes)
- 🎬 Cinema e Séries
- 🎮 Videojogos
- 💻 Programação e Tecnologia
- 🎵 Música
- 🍕 Gastronomia
- 🦕 Dinossauros e História

---

## 🛠️ Tecnologias Utilizadas

- **HTML5** - Estrutura da página
- **CSS3** - Design e animações
- **JavaScript** - Análise do código Python e interatividade
- **Google Fonts** - Tipografia (Fredoka + JetBrains Mono)

---

## 🎓 Conceitos de Python que vais Aprender

- ✅ Variáveis e tipos de dados
- ✅ Função `input()` para receber dados do utilizador
- ✅ Função `print()` para mostrar mensagens
- ✅ Condições `if`/`else` para tomar decisões
- ✅ Comparações com `==`
- ✅ Operadores de atribuição como `+=`
- ✅ Método `.lower()` para converter texto
- ✅ f-strings para formatar texto

---

## 🐛 Resolução de Problemas

### O quiz não aparece quando clico em "Executar"?
- Verifica se tens perguntas com `input()` no código
- Certifica-te que cada pergunta tem uma verificação com `if ... ==`

### As respostas não são aceites mesmo estando corretas?
- Verifica se usaste `.lower()` nas respostas de texto
- Confirma que a resposta no código está escrita exatamente igual

### Quero limpar o código e começar de novo
- Clica no botão "🔄 Limpar" para repor o exemplo inicial

---

## 👨‍💻 Sobre o Clube de Código

Este projeto foi desenvolvido para o **Centro de Inovação Carlos Fiolhais**, com o objetivo de ensinar programação Python de forma divertida e interativa aos jovens programadores!

---

## 📝 Licença

Projeto educativo de código aberto para o Clube de Código CICF.

---

## 🌟 Desafios Extra

Quando dominares o básico, tenta:

1. **Adicionar 5 ou mais perguntas** ao teu quiz
2. **Criar categorias** de perguntas (fácil, médio, difícil)
3. **Adicionar um cronómetro** para cada pergunta
4. **Criar um quiz de verdadeiro/falso**
5. **Fazer perguntas de escolha múltipla** (A, B, C, D)

---

**Diverte-te a programar! 🚀🐍**

*Desenvolvido com ❤️ para o Clube de Código CICF*
