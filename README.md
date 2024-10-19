# Biblioteca SQLite

Este é um projeto de gerenciamento de biblioteca utilizando SQLite. O sistema permite gerenciar autores, livros e empréstimos, facilitando a organização do acervo e o controle de empréstimos.

## Funcionalidades

- Cadastro de autores
- Cadastro de livros
- Registro de empréstimos
- Consultas de dados inseridos

## Estrutura do Banco de Dados

O banco de dados contém três tabelas principais:

1. **Autores**: Armazena informações sobre os autores.
   - `AutorID`: Identificador único do autor.
   - `Nome`: Nome do autor.
   - `Nacionalidade`: Nacionalidade do autor.

2. **Livros**: Armazena informações sobre os livros.
   - `LivroID`: Identificador único do livro.
   - `Titulo`: Título do livro.
   - `AutorID`: Referência ao autor do livro.
   - `AnoPublicacao`: Ano de publicação do livro.
   - `Genero`: Gênero do livro.

3. **Emprestimos**: Registra os empréstimos dos livros.
   - `EmprestimoID`: Identificador único do empréstimo.
   - `LivroID`: Referência ao livro emprestado.
   - `DataEmprestimo`: Data em que o livro foi emprestado.
   - `DataDevolucao`: Data de devolução do livro.
   - `NomeUsuario`: Nome do usuário que emprestou o livro.

## Como Usar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu_usuario/biblioteca-sqlite.git
Instale o SQLite, se ainda não tiver instalado.

Execute o script Python para criar o banco de dados e inserir dados:
python seu_script.py

Consulte os dados inseridos na saída do terminal.

Licença
Este projeto está licenciado sob a MIT License.

