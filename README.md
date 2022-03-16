# Minimal API

Uma API Minimal completa e funcional usando .NET 6, serviços com Autenticação JWT, Identity e Migration.

## Rodando aplicação

 1. Para rodar o projeto é necessário criar uma primeira **Migration**, para isso utilize o seguinte comando.

Comandos para execução:

```
Add-Migration <MIGRATION_NAME>
```

```
Update-Database
```

 2. Com a utilização do pacote NET DevPack, conforme a própria documentação, necessáriamente é preciso gerar uma **Migration** utilizando o próprio **DbContext** do package.

> *Neste projeto é utilizado o pacote [*NET DevPack*](https://github.com/NetDevPack/Security.Identity) Identity que é um conjunto de implementações comuns para ajudá-lo a implementar Identity, Jwt, validação de declarações e outras facilidades*

Comandos para execução:

```
Add-Migration -Context NetDevPackAppDbContext
```

```
Update-Database -Context NetDevPackAppDbContext
```