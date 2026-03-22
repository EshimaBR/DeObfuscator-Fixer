# Arma 3 PBO Deobfuscator Fixer

Uma ferramenta automatizada em lotes e PowerShell para corrigir o arquivo `config.cpp` e organizar os modelos 3D após a desofuscação de arquivos PBO do Arma 3 com o `DeMikeroObfuscator`.

Geralmente, ao desofuscar um mod usando o DeMikeroObfuscator, o `config.cpp` perde nomes e quebra referências de modelos, sendo nomeados genericamente como `deobfuscated_modelXX`. Essa ferramenta varre a estrutura, reconstrói o seu `config.cpp` com as referências originais e renomeia os modelos extraídos corretamente!

## 🛠️ Conteúdo da Ferramenta

*   **`CorrigirDeobfuscator.exe`**: O executável único que contém o motor lógico da ferramenta já compilado e ofuscado. Basta usá-lo como um atalho "Drag-and-Drop" para processar os arquivos sem complicação.

## 🚀 Como usar em seus projetos

Depois de usar o seu `DeMikeroObfuscator` em um arquivo PBO e ele gerar o `config.cpp` bugado mais aqueles arquivos `.p3d/.paa` genéricos, siga os passos a seguir:

1. **Copie a ferramenta:** Copie o arquivo `CorrigirDeobfuscator.exe` para a **mesma pasta** onde o processo de desofuscação ocorreu e os arquivos estão.
2. **Arraste e Solte (Drag & Drop):** Clique, segure e **ARRASTE** o seu arquivo PBO **ORIGINAL** (ex: `MeuMod.pbo`), **soltando-o exatamente em cima do ícone** do arquivo `CorrigirDeobfuscator.exe`.

> **Pronto!** A ferramenta vai abrir uma tela de terminal verde, ela localizará todos os arquivos desofuscados de forma automática, vai checar o PBO original, consertar as peças com nomes genéricos e injetar/processar a substituição de 100% do seu `config.cpp`!
