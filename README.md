# Path Scripting (.ps)

<p align="center">
  <img src="ps-logo.png" width="150" alt="Path Scripting Logo">
</p>

**Path Scripting** é uma linguagem de programação ultra-minimalista que transpila para JavaScript. Ela foi desenhada para ser elegante, rápida e focar no que realmente importa: o fluxo dos seus dados.

## Destaques

- **Zero Boilerplate**: Esqueça `let`, `const` ou `var`. O compilador entende suas atribuições automaticamente.
- **Operador Path (`..>`)**: Encadeie funções de forma legível e linear. Chega de parênteses aninhados!
- **Sintaxe Minimalista**: Defina funções e variáveis com o mínimo de caracteres possível.
- **Print Inteligente**: Suporte nativo para interpolação de strings com `{variável}`.

## Exemplo de Código

```ps
// Defina uma função de forma simples
greet user -> "Hello, " + user.name + "!"

// Atribuição automática
name = "_yWizerX"
userObj = name ..> (n -> ({ name: n }))

// Print com interpolação mágica
print "Welcome to the path, {name}!"

// O poder do Pipe (Caminho)
userObj ..> greet ..> print
```

## Como Iniciar

### 1. Instalação
Clone o repositório e instale as dependências (se houver):
```bash
git clone https://github.com/yWizerX/Path-Scripting.git
cd Path-Scripting
```

### 2. Compilação
Para transformar um arquivo `.ps` em `.js`, use o nosso CLI:
```bash
node src/cli.js examples/hello.ps
```

### 3. Execução
Para compilar e já executar o código imediatamente:
```bash
node src/cli.js examples/hello.ps --run
```

## Comunidade e Suporte

- **Discord**: [Junte-se à nossa comunidade](https://discord.gg/Na5gYTMDCu)
- **Website**: Em breve

---

Obrigado!
