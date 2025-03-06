CREATE DATABASE Faculdade;
USE Faculdade;

CREATE TABLE professor (
    id_professor INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL,
    especializacao VARCHAR(100) DEFAULT 'Não Informado'
);

CREATE TABLE aluno (
    id_aluno INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL,
    data_nascimento DATE NOT NULL
);

CREATE TABLE disciplina (
    id_disciplina INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(100) NOT NULL,
    carga_horaria INT DEFAULT 40,
    id_professor INT,
    FOREIGN KEY (id_professor) REFERENCES professor(id_professor) ON DELETE SET NULL
);

/* Inserindo os dados*/
INSERT INTO professor (nome, email, especializacao) VALUES
('Carlos Silva', 'carlos.silva@email.com', 'Banco de Dados'),
('Ana Souza', 'ana.souza@email.com', 'Programação Web');

INSERT INTO aluno (nome, email, data_nascimento) VALUES
('João Pereira', 'joao.pereira@email.com', '2002-05-10'),
('Mariana Lima', 'mariana.lima@email.com', '2003-08-21');

INSERT INTO disciplina (nome, carga_horaria, id_professor) VALUES
('Banco de Dados', 60, 1),
('Desenvolvimento Web', 80, 2);

