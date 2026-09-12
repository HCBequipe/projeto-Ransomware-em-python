# projeto-ramsonware-em-python

# Simulação e Análise de Ransomware com Python

Projeto prático desenvolvido no bootcamp **Santander Cibersegurança** para compreender o funcionamento técnico de um ransomware baseado em criptografia simétrica utilizando Python.

## 🛠️ Tecnologias e Ferramentas Utilizadas
* **Python 3**: Linguagem de programação utilizada para a criação dos scripts de manipulação de arquivos.
* **Biblioteca `pyaes`**: Módulo para implementação do algoritmo de criptografia AES em Python.
* **Ambiente de Laboratório**: Máquina virtual e ambiente isolado para testes controlados.

## 📂 Componentes do Projeto
* `encrypter.py`: Script responsável por ler um arquivo de teste, aplicar o algoritmo de criptografia simétrica e alterar os dados.
* `decrypter.py`: Script responsável por reverter o processo de criptografia utilizando a chave correta.
* `senhas.txt`: Arquivo de texto utilizado como alvo nos testes de laboratório.

## ⚙️ Funcionamento Técnico

1. **Fase de Criptografia (`encrypter.py`)**:
   * O script localiza o arquivo de texto alvo no diretório.
   * Aplica a chave simétrica gerada pelo algoritmo AES para reescrever os dados em formato criptografado.
2. **Fase de Descriptografia (`decrypter.py`)**:
   * O script utiliza a chave de descriptografia para processar os dados embaralhados.
   * Restaura o arquivo ao seu estado original e legível.

## 📸 Evidências Práticas

*(Insira aqui as capturas de tela do terminal rodando os scripts com sucesso)*

## 🛡️ Medidas de Defesa e Mitigação contra Ransomware

Para conter e prevenir incidentes envolvendo ransomware, adota-se uma estratégia de segurança em camadas:
* **Estratégia de Backup 3-2-1**: Manter 3 cópias dos dados, em 2 mídias diferentes, sendo pelo menos 1 cópia totalmente offline/imutável.
* **Soluções de EDR (Endpoint Detection and Response)**: Ferramentas capazes de identificar comportamentos anômalos, como a tentativa de criptografia em massa de arquivos em curto período.
* **Controle de Acesso e Privilégios**: Aplicação do princípio do menor privilégio para evitar que usuários comuns tenham permissões de escrita em diretórios críticos ou compartilhamentos de rede desnecessários.
