Projeto do Curso JSF e PrimeFaces Essencial configurado com o [KumuluzEE](https://github.com/TFaga/KumuluzEE).

Para rodar o projeto basta executar:

```shell
$ mvn package; java -cp target/classes:target/dependency/* com.kumuluz.ee.EeApplication
```

Depois acesse [http://localhost:8080](http://localhost:8080)

## Alterações referentes ao projeto original

O projeto original é esse: https://github.com/algaworks/curso-jsf-primefaces-essencial/tree/master/exportando-tabela-de-dados-para-excel

* Alterar o tipo do projeto de *web* para *jar*
* Inclusão das dependências do KumuluzEE no *pom.xml*
* Mover a pasta *webapp* de *src/main* para *src/main/resources*
* Remover, do arquivo *web.xml*, o mapeamendo do servlet do JSF
* Informar as entidades explicitamente no *persistence.xml*
* Alteração das queries para se adaptarem ao EclipseLink, pois, o KumuluzEE ainda não suporta o Hibernate
