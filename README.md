Ransomware - Criptografia e Descriptografia de Arquivos em Python
Este projeto tem como objetivo demonstrar a criação de um simples ransomware, utilizando a linguagem Python para criptografar e descriptografar arquivos. O ransomware simula o processo de criptografia de um arquivo e a criação de um arquivo "sequestrado", que pode ser revertido utilizando uma chave de descriptografia.

Funcionalidades
Criptografia de Arquivos
O código criptografa um arquivo de texto e cria uma versão "sequestrada" do arquivo com uma extensão customizada. O arquivo original é removido após a criptografia.

Descriptografia de Arquivos
O código descriptografa um arquivo criptografado, retornando o arquivo original para seu formato legível. O arquivo criptografado é removido após a descriptografia.

Tecnologias Utilizadas
Python 3.x
Biblioteca pyaes: Utilizada para implementar o algoritmo de criptografia AES (Advanced Encryption Standard) no modo CTR (Counter).
Como Funciona
O projeto consiste em dois scripts principais: um para criptografar e outro para descriptografar um arquivo. A criptografia e a descriptografia utilizam o algoritmo AES, que é um dos mais seguros para criptografia de dados.

Fluxo do Código 1 (Criptografia)
Abrir Arquivo: O arquivo de texto a ser criptografado (exemplo: teste.txt) é aberto em modo binário (rb).
Remover Arquivo Original: O arquivo original é removido do sistema para simular um ataque de ransomware.
Configuração da Chave de Criptografia: Define-se uma chave secreta de criptografia, no caso testeransomwares, utilizada no processo de criptografia.
Criptografar Dados: O arquivo é criptografado utilizando o algoritmo AES no modo CTR.
Criar Arquivo Criptografado: Um novo arquivo com a extensão .ransomwaretroll é criado contendo os dados criptografados.
Fluxo do Código 2 (Descriptografia)
Abrir Arquivo Criptografado: O arquivo criptografado (exemplo: teste.txt.ransomwaretroll) é aberto.
Configuração da Chave de Descriptografia: A mesma chave testeransomwares é utilizada para a descriptografia.
Descriptografar Dados: O conteúdo do arquivo criptografado é revertido para o seu formato original.
Remover Arquivo Criptografado: O arquivo criptografado é removido após a descriptografia.
Criar Arquivo Original: Um novo arquivo (exemplo: teste.txt) é criado contendo os dados descriptografados.
Como Executar o Projeto
Pré-requisitos
Python 3.x instalado no seu sistema.

Biblioteca pyaes instalada. Para instalar, execute o seguinte comando no terminal:

bash
Copiar código
pip install pyaes
Execução
Criptografar o Arquivo

Execute o script de criptografia para criar um arquivo criptografado:

bash
Copiar código
python criptografar.py
O arquivo original será removido e um novo arquivo com a extensão .ransomwaretroll será criado.

Descriptografar o Arquivo

Execute o script de descriptografia para restaurar o arquivo original:

bash
Copiar código
python descriptografar.py
O arquivo criptografado será removido e o arquivo original será restaurado.
