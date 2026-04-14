• Por que a Secret aparece no log como ** e a variável aparece
normalmente?
	R: A Secret aparece assim pois ela é feita para senhas e 
	chaves de acesso, possibilitando apenas o dono do 
	repositório acessar e ler suas informações, tendo nível 
	máximo de segurança (criptografado). Já a Variável aparece 
	normalmente por todos que possuem permissão de acesso às 
	configurações do repositório podem vê-la, seu nível de 
	segurança é considerado baixo, então não deve conter dados 
	sensíveis.

• O Job deploy_app consegue ler a variável BUILD_VERSION criada no Job
build_app? Por quê?
	R: Não, pois foi uma variável criada a nível do Job, ou 
	seja, fica disponível para apenas os passos dentro do job 
	que ela foi criada, no caso, Job build_app, ficando 
	invisível para outros jobs.
