# manga API base

Api criada com base numa lista de mangá e suas informações. Possui Login e Cadastro.

# End-Points

POST /login - Login do usuário; (formato de informações JSON, retorna TOKEN)
POST /register - Cadastrar usuário; (formato de informações JSON)

GET /user/id - Pega usuário pelo ID (necessita Bearer TOKEN)

GET /manga - Possibilita somente a leitura de uma lista de mangás para todos os usuários, mesmo que não logados (Não necessita Bearer)

GET/mangaspecial - Possibilita somente a leitura de uma lista de mangás especiais somente para usuários logados (necessita Bearer TOKEN)

POST/userlist - Voce precisa ser dono da lista para escrever/alterar ela, e necessita estar logado para conseguir fazer a leitura (necessita Bearer TOKEN)
