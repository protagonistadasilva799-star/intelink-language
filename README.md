# Intelink Language — Termux

## O que é

O **Intelink Language** é o executor e runtime da linguagem de programação Intelink preparado para o **Termux no Android**. A linguagem Intelink é o conjunto de regras, comandos e formatos que o programador utiliza; o Python aparece neste repositório como tecnologia usada para implementar o executor e ferramentas auxiliares.

Este projeto é a referência do ambiente Termux. A versão para computador na nuvem ou sandbox fica separada no repositório [intelink-sandbox](https://github.com/protagonistadasilva799-star/intelink-sandbox).

## Para que serve

O runtime permite estudar e executar programas Intelink no Termux, com modo interativo e operações integradas ao ambiente Android. A implementação contém mecanismos para interpretar entradas da linguagem, manter valores em memória, executar funções disponíveis e encaminhar somente comandos de sistema autorizados. A gramática completa deve ser conferida no executor, nos exemplos e nos testes do próprio repositório.

## Instalação no Termux

Quando o pacote Debian estiver disponível para a arquitetura do aparelho:

```bash
pkg install python dpkg
dpkg -i packages/intelink-language_*.deb
```

Também é possível estudar a implementação diretamente:

```bash
python3 src/intelink_runtime.py
```

## Programação

O primeiro passo é criar um arquivo no formato aceito pelo executor e executar o arquivo com o comando disponibilizado pelo pacote. Não use construções apenas mencionadas em planos ou descrições sem confirmar que o parser atual as reconhece.

Recursos como atribuições, funções, retorno, operações de IA, memória local e execução controlada de comandos devem ser tratados de acordo com o comportamento observado no código. Exemplos não confirmados devem ser marcados como experimentais ou não implementados.

## Segurança

A execução de comandos externos é limitada por uma lista de comandos autorizados. Comandos Termux, permissões do Android, acesso a arquivos, clipboard, bateria e outros recursos dependem do que está efetivamente implementado e das permissões concedidas ao Termux. Nunca execute código de fonte desconhecida sem revisar suas operações.

## Compatibilidade

O alvo principal é Termux/Android. Pacotes `.deb` deste repositório não devem ser instalados automaticamente em um computador Linux comum ou no sandbox, porque podem conter caminhos, comandos e pressupostos específicos do Termux. Para o sandbox, use a adaptação separada.

## Arquivos principais

| Caminho | Função |
|---|---|
| `src/intelink_runtime.py` | Runtime e executor principal |
| `packages/` | Pacotes Debian quando publicados |
| `TERMS.md` | Termos e condições de uso |

## Criador e termos

**Criador:** Samuel Artulino.

Este projeto utiliza tecnologia da Intelink. Antes de usar, modificar, redistribuir ou publicar derivados, leia [TERMS.md](TERMS.md) e preserve os créditos e as restrições estabelecidas nele.
