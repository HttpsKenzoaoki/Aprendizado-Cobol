# 📚 Aprendizado COBOL

Repositório dedicado a anotações, pequenos programas e exercícios práticos para estudo da linguagem **COBOL** no Linux.

---

## 🛠️ Pré-requisitos

Para compilar e executar os códigos, é necessário ter o compilador **GnuCOBOL** instalado no sistema.

### Instalação (Linux)

No **Debian / Ubuntu** e derivados:

```bash
sudo apt update
sudo apt install gnucobol
```

No **Arch Linux**:

```bash
sudo pacman -S gnucobol
```

Para verificar se a instalação foi concluída com sucesso:

```bash
cobc --version
```

---

## 🚀 Como compilar e executar

O fluxo básico consiste em compilar o fonte `.cbl` gerando um binário executável e rodá-lo diretamente no terminal.

### 1. Compilação

Para compilar gerando um executável autônomo (substitua pelo nome do arquivo desejado):

```bash
cobc -x Helloworld.cbl
```

> **Nota:** A flag `-x` instrui o `cobc` a gerar um binário executável. Por padrão, ele criará um arquivo com o mesmo nome do fonte, porém sem a extensão `.cbl`.

Se preferir definir explicitamente o nome do executável gerado:

```bash
cobc -x -o helloworld Helloworld.cbl
```

### 2. Execução

Execute o binário gerado:

```bash
./Helloworld
```

---

## 📂 Estrutura do Repositório

```text
.
├── .gitignore
├── README.md
├── Comovai.cbl
└── Helloworld.cbl
```

> Arquivos binários compilados são ignorados pelo `.gitignore` para manter o versionamento apenas dos arquivos-fonte.