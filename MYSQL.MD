CREATE USER 'novousuario'@'localhost' IDENTIFIED BY 'password';

GRANT ALL PRIVILEGES ON * . * TO 'novousuario'@'localhost';

FLUSH PRIVILEGES;


ALL PRIVILEGES- como vimos anteriormente, isso daria a um usuário do MySQL todo o acesso a uma determinada base de dados (ou se nenhuma base de dados for selecionada, todo o sistema)
CREATE- permite criar novas tabelas ou bases de dados
DROP- permite deletar tableas ou bases de dados
DELETE- permite deletar linhas das tabelas
INSERT- permite inserir linhas nas tabelas
SELECT- permite utilizar o comando Select para ler bases de dados
UPDATE- permite atualizar linhas das tabelas
GRANT OPTION- permite conceder ou revogar privilégios de outros usuários 


GRANT [tipo de permissão] ON [nome da base de dados].[nome da tabela] TO ‘[nome do usuário]’@'localhost’;


REVOKE [tipo de permissão] ON [nome da base de dados].[nome da tabela] FROM ‘[nome do usuário]’@‘localhost’;


DROP USER ‘demo’@‘localhost’;


quit

mysql -u [nome do usuário]-p
