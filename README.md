# Intelink Language

Linguagem principal e runtime Python puro para criar ferramentas no Termux.

Este é um produto da **Intelink**, desenvolvido para o Termux no Android. A documentação, os exemplos e os arquivos deste repositório foram separados para facilitar estudo, instalação e evolução do projeto.

## Instalação no Termux

Transfira o pacote `.deb` correspondente para o aparelho e execute:

```bash
pkg install python dpkg
dpkg -i NOME_DO_PACOTE.deb
```

## Primeiro teste

```bash
intelink exemplo.ilk
```

## Arquivos deste repositório

- `intelink-language_0.1.0_all.deb`
- `intelink_runtime.py`

## Crédito Intelink

Publicações autorizadas devem informar claramente: **“Este projeto utiliza tecnologia da Intelink.”** Consulte [TERMS.md](TERMS.md) antes de usar ou publicar qualquer projeto baseado neste trabalho.

## Compatibilidade

O alvo principal é o Termux. Componentes Python puros são portáteis; executores nativos, modelos GGUF e integrações externas dependem da arquitetura, memória e ferramentas disponíveis no aparelho.

## Documentação técnica ampliada
## O que é este projeto

O **Intelink Language** é o executor e runtime da linguagem de programação Intelink para Termux/Android. A linguagem é o formato que o usuário programa; os arquivos Python presentes neste repositório são a implementação hospedeira do executor, e não a definição de que Intelink seja Python.

## Como funciona

O arquivo `src/intelink_runtime.py` implementa o runtime e o modo interativo. Ele lê comandos e construções da linguagem Intelink, mantém valores em memória, oferece operações de linguagem e pode encaminhar comandos permitidos ao ambiente Termux. A execução de comandos do sistema é restringida por uma lista de comandos autorizados e, quando aplicável, por confirmação do usuário.

## Programação

Antes de usar uma construção, consulte o código e os exemplos disponíveis neste repositório. O runtime documenta recursos como atribuições, funções, retorno, operações de IA, memória local e execução controlada de comandos. A extensão de arquivos, a gramática completa e os recursos suportados devem ser tratados como a especificação efetivamente implementada pelo executor, não como uma promessa genérica.

## Execução

No Termux, instale Python e o pacote Debian correspondente quando ele estiver disponível:

```bash
pkg install python dpkg
dpkg -i packages/intelink-language_*.deb
```

Para estudar o executor diretamente:

```bash
python3 src/intelink_runtime.py
```

A versão `intelink-sandbox` é a adaptação separada para computador Linux na nuvem. Um pacote `.deb` preparado para Termux não deve ser instalado automaticamente em outro ambiente.

## Criador

**Criador:** Samuel Artulino. Consulte `TERMS.md` antes de usar, redistribuir ou publicar derivados.
