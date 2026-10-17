# Desafio de Projeto: Entendendo um Ransomware na Prática com Python

Este projeto foi desenvolvido como parte do bootcamp de Cybersecurity na **Digital Innovation One (DIO)**. O objetivo é demonstrar didaticamente o funcionamento básico da criptografia e descriptografia de dados utilizada por malwares do tipo Ransomware.

> ⚠️ **Aviso de Isenção de Responsabilidade**: Este código possui finalidade estritamente educacional no âmbito de estudos de Segurança da Informação.

---

## 🛠️ Tecnologias e Bibliotecas Utilizadas

- **Python 3.x**
- **pyaes**: Biblioteca para criptografia utilizando o algoritmo AES (Advanced Encryption Standard).
- **os**: Módulo nativo para manipulação de arquivos do sistema operacional.

---

## 📂 Estrutura do Projeto

- `encrypter.py`: Lê o arquivo original `teste.txt`, criptografa o seu conteúdo utilizando AES no modo CTR e substitui o arquivo por uma versão criptografada (`teste.txt.ransomwaretroll`).
- `decrypter.py`: Lê o arquivo criptografado `teste.txt.ransomwaretroll`, reverte o processo com a chave simétrica e restaura o arquivo original `teste.txt`.
- `teste.txt`: Arquivo de texto utilizado para testes.

---

## 🚀 Como Executar

### 1. Pré-requisitos
Certifique-se de ter o Python 3 e a biblioteca `pyaes` instalados:

```bash
pip install pyaes
```

### 2. Criptografando o arquivo
Execute o script de encriptação:

```bash
python3 encrypter.py
```

*Resultado*: O arquivo `teste.txt` será removido e o arquivo `teste.txt.ransomwaretroll` será gerado com o conteúdo cifrado.

### 3. Descriptografando o arquivo
Execute o script de decriptação:

```bash
python3 decrypter.py
```

*Resultado*: O arquivo `.ransomwaretroll` será removido e o `teste.txt` original será restaurado.


