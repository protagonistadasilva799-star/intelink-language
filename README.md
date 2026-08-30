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
