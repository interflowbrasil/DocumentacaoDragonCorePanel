Recuperar os usuarios criados no painel pelo usuario do API Key:

```sh
curl --location 'https://seudominio.com/core/apiatlas.php' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: PHPSESSID=r02n0da5t6et5fku8kmpifh5o9' \
--data-urlencode 'passapi=SUACHAVE' \
--data-urlencode 'module=userget'
```

Retorno de exemplo: 

```sh
[{"id":87,"byid":1,"categoriaid":1,"limite":1000,"bycredit":0,"login":"lima","senha":"lima","mainid":"NULL","expira":"2025-06-04 15:33:37","lastview":"","status":"Online","valormensal":"","notificado":"nao","whatsapp":"","uuid":""}]
```

---------------------------------------

Recuperar os revendedores criados no painel pelo usuario do API Key:

```sh
curl --location 'https://seudominio.com/core/apiatlas.php' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: PHPSESSID=r02n0da5t6et5fku8kmpifh5o9' \
--data-urlencode 'passapi=SUACHAVE' \
--data-urlencode 'module=revendaget'
```

Retorno de exemplo: 

```sh
[{"id":15,"nome":null,"contato":null,"login":"lima","token":"0","mb":"0","senha":"lima","byid":"1","mainid":"0","accesstoken":null,"valorusuario":null,"valorrevenda":null,"idtelegram":null,"tempo":null,"tokenvenda":"0","acesstokenpaghiper":null,"formadepag":"1","tokenpaghiper":null,"whatsapp":""}]
```

---------------------------------------

Criar teste como administrador:

```sh
curl --location 'https://seudominio.com/core/apiatlas.php' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: PHPSESSID=r02n0da5t6et5fku8kmpifh5o9' \
--data-urlencode 'passapi=SUACHAVE' \
--data-urlencode 'module=criarteste' \
--data-urlencode 'user=USUARIO' \
--data-urlencode 'pass= SENHA' \
--data-urlencode 'testtime= TEMPO EM MINUTOS DO TESTE' \
--data-urlencode 'admincid=ID DA CATEGORIA'
```

Retorno de exemplo: 

```sh
"Sucess: , SERVER ; Error: "
```

---------------------------------------

Criar teste como revendedor:

```sh
curl --location 'https://seudominio.com/core/apiatlas.php' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: PHPSESSID=r02n0da5t6et5fku8kmpifh5o9' \
--data-urlencode 'passapi=SUACHAVE' \
--data-urlencode 'module=criarteste' \
--data-urlencode 'user=USUARIO' \
--data-urlencode 'pass=SENHA' \
--data-urlencode 'testtime= TEMPO EM MINUTOS DO TESTE' \
```

Retorno de exemplo: 

```sh
"Sucess: , SERVER ; Error: "
```

---------------------------------------

Criar Usuario como administrador:

```sh
curl --location 'https://seudominio.com/core/apiatlas.php' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: PHPSESSID=r02n0da5t6et5fku8kmpifh5o9' \
--data-urlencode 'passapi=SUACHAVE' \
--data-urlencode 'module=criaruser' \
--data-urlencode 'user=USUARIO' \
--data-urlencode 'pass=SENHA' \
--data-urlencode 'admincid=ID DA CATEGORIA' \
--data-urlencode 'validadeusuario=Tempo em dias do usuario' \
--data-urlencode 'userlimite=Limite do usuario' \
--data-urlencode 'whatsapp=WHATSAPP DO CLIENTE'
```

Retorno de exemplo: 

```sh
"Sucess: , SERVER ; Error: "
```

---------------------------------------

Criar Usuario como revendedor:

```sh
curl --location 'https://seudominio.com/core/apiatlas.php' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: PHPSESSID=r02n0da5t6et5fku8kmpifh5o9' \
--data-urlencode 'passapi=SUACHAVE' \
--data-urlencode 'module=criaruser' \
--data-urlencode 'user=USUARIO' \
--data-urlencode 'pass=SENHA' \
--data-urlencode 'validadeusuario=Tempo em dias do usuario' \
--data-urlencode 'userlimite=Limite do usuario' \
--data-urlencode 'whatsapp=WHATSAPP DO CLIENTE'
```

Retorno de exemplo: 

```sh
"Sucess: , SERVER ; Error: "
```

---------------------------------------

Renovar usuario:

```sh
curl --location 'https://seudominio.com/core/apiatlas.php' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: PHPSESSID=r02n0da5t6et5fku8kmpifh5o9' \
--data-urlencode 'passapi=SUACHAVE' \
--data-urlencode 'module=renewuser' \
--data-urlencode 'user=USUARIO'
```

Retorno de exemplo: 

```sh
"Sucess: , SERVER ; Error: "
```

---------------------------------------

Renovar Revendedor:

```sh
curl --location 'https://seudominio.com/core/apiatlas.php' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: PHPSESSID=r02n0da5t6et5fku8kmpifh5o9' \
--data-urlencode 'passapi=SUACHAVE' \
--data-urlencode 'module=renewrev' \
--data-urlencode 'user=USUARIO'
```

Retorno de exemplo: 

```sh
"Revendedor Renovado com sucesso!"
```

---------------------------------------

Limpar Device ID:

```sh
curl --location 'https://seudominio.com/core/apiatlas.php' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: PHPSESSID=r02n0da5t6et5fku8kmpifh5o9' \
--data-urlencode 'passapi=SUACHAVE' \
--data-urlencode 'module=deviceclean' \
--data-urlencode 'user=USUARIO'
```

Retorno de exemplo: 

```sh
"Piu piu limpo"
```

---------------------------------------

Criar Revendedor usando conta administradora:

```sh
curl --location 'https://seudominio.com/core/apiatlas.php' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: PHPSESSID=r02n0da5t6et5fku8kmpifh5o9' \
--data-urlencode 'passapi=SUACHAVE' \
--data-urlencode 'module=createrev' \
--data-urlencode 'user=USUARIO' \
--data-urlencode 'pass=SENHA' \
--data-urlencode 'admincid=ID DA CATEGORIA' \
--data-urlencode 'userlimite=Limite Do revendedor' \
--data-urlencode 'whatsapp=WHATSAPP DO REVENDEDOR'
```

Retorno de exemplo: 

```sh
"Revendedor criado!"
```

---------------------------------------

Criar Revendedor usando conta Revendedora:

```sh
curl --location 'https://seudominio.com/core/apiatlas.php' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: PHPSESSID=r02n0da5t6et5fku8kmpifh5o9' \
--data-urlencode 'passapi=SUACHAVE' \
--data-urlencode 'module=createrev' \
--data-urlencode 'user=USUARIO' \
--data-urlencode 'pass=SENHA' \
--data-urlencode 'userlimite=Limite Do revendedor' \
--data-urlencode 'whatsapp=WHATSAPP DO REVENDEDOR'
```

Retorno de exemplo: 

```sh
"Revendedor criado!"
```

---------------------------------------

Seta o usuario como notificado no banco de dados:

```sh
curl --location 'https://seudominio.com/core/apiatlas.php' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: PHPSESSID=r02n0da5t6et5fku8kmpifh5o9' \
--data-urlencode 'passapi=SUACHAVE' \
--data-urlencode 'module=notificado' \
--data-urlencode 'idpony=ID USUARIO'
```

Retorno de exemplo: 

```sh
true
```
---------------------------------------

Recupera os usuarios onlines:

```sh
curl --location 'https://seudominio.com/core/apiatlas.php' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: PHPSESSID=r02n0da5t6et5fku8kmpifh5o9' \
--data-urlencode 'passapi=SUACHAVE' \
--data-urlencode 'module=onlines'
```

Retorno de exemplo: 

```sh
[{"login":"login","quantidade":"1"}]
```

