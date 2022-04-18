# analytics-engineer-challenge

- Utilização do Script: 
Para que o projeto conecte com o banco de dados, é necessário preencher o arquivo de configuração com o nome banco.ini.


- Analisando a forma de subir o csv para o banco:
Inicialmente iria subir as informações de cada tabela separadamente interando cada linha do csv informando cada coluna no insert, porém para este projeto pensei em  deixar os métodos de forma genérica, sem pensar na estrutura do csv podendo ser reutilizado, então utilizei o comando COPY do POSTGRES (esse comando só é permitido pelo super usuário do banco). 

- Sobre o Jupyter Notebook:
Sempre utilizei a IDE Visual Studio para meus scripts, então foi um  desafio realizar todo o projeto no Jupyter Notebook, porém fiquei feliz ao concluir o projeto só com essa ferramenta. Vou continuar estudando as possibilidades que posso criar com a ferramenta.

- Ferramenta de visualização:
Para este tópico utilizei a ferramenta Grafana, a qual tive meu primeiro contato com este desafio. Foi necessário a criação de uma máquina virtual com o ubuntu server 18.04 LTS para configuração da ferramenta, após a instalação, a conexão com o banco PostgreSQL foi bem tranquila, pois a máquina virtual esta na mesma rede que a minha máquina.



- Em uma futura atualização:
Sei que utilizando somente "VARCHAR" nos tipos dos dados não é a melhor forma de modela-los, mas foi a única maneira que pensei em popular qualquer CSV de forma génerica, como informei nos tópicos anteriores, sem pensar na estrutura do CSV.Para criação das chaves estrangeira, iria utilizar o seguinte comando: ALTER TABLE tabela_filha ADD CONSTRAINT nome_constraint FOREIGN KEY (coluna) REFERENCES tabela-pai(coluna), ao criar as tabelas.
