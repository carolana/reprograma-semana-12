<h1 align="center">
    <br>
    <p align="center">Semana 12 - Introdução ao Banco de Dados<p>
</h1>

## Essa semana nós aprendemos sobre Banco de Dados: 

- Banco de Dados relacional (SQL)
- Banco de Dados não-relacional (NoSQL)
- SGBDs (Sistema de Gerenciamento de Banco de Dados)
- Robo3T
- MongoDB

### Nossa tarefa de casa seria montar foi criar um banco de dados novo (database) e uma coleção com um nome pertinente, de acordo com os dados e tema escolhidos. Vamos ver?

![gif "Will Smith"](img/giphy000.gif)



### Consultar todos os documentos da collection
```
db.getCollection('person').find({})
```

### Inserção de documentos
```
db.person.insertMany([
    {
		"nome": "Liz Lorena da Mata",
		"idade": 68,
		"cpf": "575.974.136-53",
		"rg": "23.091.809-8",
		"data_nasc": "01/06/1953",
		"sexo": "Feminino",
		"signo": "Gêmeos",
		"mae": "Alessandra Stella Vitória",
		"pai": "Vicente Luiz Benício da Mata",
		"email": "lizlorenadamata_@outlook.com.br",
		"senha": "WjU5hDUqZA",
		"cep": "69900-108",
		"endereco": "Rua Piauí",
		"numero": 220,
		"bairro": "Papouco",
		"cidade": "Rio Branco",
		"estado": "AC",
		"telefone_fixo": "(68) 3574-6363",
		"celular": "(68) 99693-4105",
		"altura": "1,53",
		"peso": 73,
		"tipo_sanguineo": "O+",
		"cor": "preto"
	},
	{
		"nome": "Allana Rebeca da Rosa",
		"idade": 40,
		"cpf": "338.779.733-88",
		"rg": "47.702.642-4",
		"data_nasc": "14/08/1981",
		"sexo": "Feminino",
		"signo": "Leão",
		"mae": "Cecília Isabelle Isadora",
		"pai": "Heitor Paulo Breno da Rosa",
		"email": "allanarebecadarosa-96@esplanadaviagens.com.br",
		"senha": "ma8mNR9k6Q",
		"cep": "57073-418",
		"endereco": "1ª Travessa Ministro Lindolfo Collor",
		"numero": 195,
		"bairro": "Cidade Universitária",
		"cidade": "Maceió",
		"estado": "AL",
		"telefone_fixo": "(82) 3854-4213",
		"celular": "(82) 99292-8762",
		"altura": "1,74",
		"peso": 70,
		"tipo_sanguineo": "A+",
		"cor": "vermelho"
	},
	{
		"nome": "Isabel Larissa Nunes",
		"idade": 39,
		"cpf": "513.542.204-80",
		"rg": "47.470.434-8",
		"data_nasc": "04/01/1982",
		"sexo": "Feminino",
		"signo": "Capricórnio",
		"mae": "Milena Benedita Eloá",
		"pai": "Roberto Ruan Mário Nunes",
		"email": "isabellarissanunes_@gruporeis.net",
		"senha": "gZG35fJNhl",
		"cep": "59133-265",
		"endereco": "Rua Francisco Morato",
		"numero": 721,
		"bairro": "Pajuçara",
		"cidade": "Natal",
		"estado": "RN",
		"telefone_fixo": "(84) 3726-8727",
		"celular": "(84) 99136-3389",
		"altura": "1,70",
		"peso": 55,
		"tipo_sanguineo": "AB-",
		"cor": "vermelho"
	},
	{
		"nome": "Iago Erick da Costa",
		"idade": 79,
		"cpf": "670.214.009-69",
		"rg": "30.187.822-5",
		"data_nasc": "04/09/1942",
		"sexo": "Masculino",
		"signo": "Virgem",
		"mae": "Benedita Caroline",
		"pai": "Thales César Bryan da Costa",
		"email": "iagoerickdacosta-92@patrezao.com.br",
		"senha": "aTTdic2nhx",
		"cep": "58057-138",
		"endereco": "Rua Maria Paulino da Silva",
		"numero": 720,
		"bairro": "Mangabeira",
		"cidade": "João Pessoa",
		"estado": "PB",
		"telefone_fixo": "(83) 3825-7264",
		"celular": "(83) 99469-8665",
		"altura": "1,90",
		"peso": 51,
		"tipo_sanguineo": "AB+",
		"cor": "laranja"
	},
	{
		"nome": "Luiz Nathan Lima",
		"idade": 59,
		"cpf": "382.081.746-88",
		"rg": "15.814.994-4",
		"data_nasc": "03/09/1962",
		"sexo": "Masculino",
		"signo": "Virgem",
		"mae": "Isis Mariah",
		"pai": "Renan Edson Lima",
		"email": "lluiznathanlima@bmalaw.com.br",
		"senha": "iKlyNZ463k",
		"cep": "78048-906",
		"endereco": "Avenida dos Florais 875",
		"numero": 442,
		"bairro": "Ribeirão do Lipa",
		"cidade": "Cuiabá",
		"estado": "MT",
		"telefone_fixo": "(65) 2700-2179",
		"celular": "(65) 99258-8777",
		"altura": "1,97",
		"peso": 107,
		"tipo_sanguineo": "AB-",
		"cor": "laranja"
	},
	{
		"nome": "Mateus Kevin de Paula",
		"idade": 24,
		"cpf": "999.876.652-41",
		"rg": "42.114.049-5",
		"data_nasc": "20/05/1997",
		"sexo": "Masculino",
		"signo": "Touro",
		"mae": "Daiane Analu Betina",
		"pai": "Heitor Márcio Cláudio de Paula",
		"email": "mateuskevindepaula-83@hotmnail.com",
		"senha": "6g64Tsj5Ny",
		"cep": "13408-143",
		"endereco": "Rua Edgard Tricanico Delboux",
		"numero": 565,
		"bairro": "Jardim Residencial Javary II",
		"cidade": "Piracicaba",
		"estado": "SP",
		"telefone_fixo": "(19) 3945-0117",
		"celular": "(19) 98293-2559",
		"altura": "1,70",
		"peso": 81,
		"tipo_sanguineo": "AB-",
		"cor": "preto"
	},
	{
		"nome": "Mariana Joana Fernandes",
		"idade": 35,
		"cpf": "566.598.058-77",
		"rg": "49.031.804-6",
		"data_nasc": "05/09/1986",
		"sexo": "Feminino",
		"signo": "Virgem",
		"mae": "Laura Aline",
		"pai": "Daniel Cauê Alexandre Fernandes",
		"email": "marianajoanafernandes..marianajoanafernandes@selfcd.com.br",
		"senha": "xqOcMKUNpL",
		"cep": "68904-016",
		"endereco": "Passagem Jardim",
		"numero": 425,
		"bairro": "Novo Buritizal",
		"cidade": "Macapá",
		"estado": "AP",
		"telefone_fixo": "(96) 3727-2001",
		"celular": "(96) 99994-2216",
		"altura": "1,64",
		"peso": 79,
		"tipo_sanguineo": "A+",
		"cor": "vermelho"
	},
	{
		"nome": "Samuel Erick Brito",
		"idade": 40,
		"cpf": "813.755.072-06",
		"rg": "45.400.456-4",
		"data_nasc": "23/07/1981",
		"sexo": "Masculino",
		"signo": "Leão",
		"mae": "Fabiana Olivia",
		"pai": "Carlos Benedito Brito",
		"email": "samuelerickbrito__samuelerickbrito@dlh.de",
		"senha": "CH6Y3d77KK",
		"cep": "74620-160",
		"endereco": "Rua 11",
		"numero": 644,
		"bairro": "Setor Morais",
		"cidade": "Goiânia",
		"estado": "GO",
		"telefone_fixo": "(62) 3883-8008",
		"celular": "(62) 98135-4628",
		"altura": "1,75",
		"peso": 94,
		"tipo_sanguineo": "A-",
		"cor": "amarelo"
	},
	{
		"nome": "Jaqueline Rosângela Flávia Freitas",
		"idade": 18,
		"cpf": "506.961.599-88",
		"rg": "36.042.884-8",
		"data_nasc": "03/01/2003",
		"sexo": "Feminino",
		"signo": "Capricórnio",
		"mae": "Giovana Teresinha Luiza",
		"pai": "Martin Guilherme Freitas",
		"email": "jaquelinerosangelaflaviafreitas..jaquelinerosangelaflaviafreitas@rjnet.com.br",
		"senha": "M6a22D9c86",
		"cep": "02837-180",
		"endereco": "Rua Joaquim Marques de Oliveira",
		"numero": 942,
		"bairro": "Vila João Batista",
		"cidade": "São Paulo",
		"estado": "SP",
		"telefone_fixo": "(11) 2985-1717",
		"celular": "(11) 99307-3633",
		"altura": "1,50",
		"peso": 76,
		"tipo_sanguineo": "A-",
		"cor": "preto"
	},
	{
		"nome": "Yago Igor Joaquim Costa",
		"idade": 71,
		"cpf": "041.114.758-76",
		"rg": "41.960.292-6",
		"data_nasc": "22/08/1950",
		"sexo": "Masculino",
		"signo": "Leão",
		"mae": "Laís Stefany Daniela",
		"pai": "Henrique Tiago Costa",
		"email": "yyagoigorjoaquimcosta@megamega.com.br",
		"senha": "tYa8MyQBph",
		"cep": "57048-260",
		"endereco": "Avenida Gilberto Soares Pinto",
		"numero": 180,
		"bairro": "Antares",
		"cidade": "Maceió",
		"estado": "AL",
		"telefone_fixo": "(82) 2820-5463",
		"celular": "(82) 99246-3949",
		"altura": "1,83",
		"peso": 66,
		"tipo_sanguineo": "B-",
		"cor": "preto"
    }
])
```

### Atualização de documentos

```
db.getCollection('person').update(
    {
        "tipo_sanguineo": "O+"
    },
    
    {
        $set: {
            "dataCriacao": ISODATE("2021-08-01T20:03:52:000Z")
          }  
    },
    
    {
        "multi" : true,
        "upsert" : false
    }
);

```
### Exclusão de documentos

```
db.getCollection('person').remove({"estado": "GO" });

```

### Consulta com projeção

```
db.getCollection('person').find({}, {"nome": 1})
```

Para não mostrar determinado atributo (nesse caso não mostraremos o id):

```
db.getCollection('person').find({}, {"nome": 1, "idade": 1, "cor": 1, "_id": 0})
```

### Consulta utilizando combinação entre os seletores

Pesquisando por pessoas que possuem idade menores do que 30 anos OU que são do signo Virgem
```
db.getCollection('person').find(
    {
        $or: [
            {"idade": {$lt: 30}},
            {"signo": /.*Virgem.*/}
        ]
    }
)
```

Pesquisando por registros que tenham necessariamento ambos os atribudos passados:

```
db.getCollection('person').find(
    { 
        "sexo": "Feminino",
        "cor": "vermelho
    }
)
```
### Consulta paginada e ordenada (utilizar skip, limit e sort)

Irá mostrar apenas 5 registros (limit):

```
db.getCollection('person').find({}).limit(5)
```
Vamos pular os 3 primeiros registros (skip):

```
db.getCollection('person').find({}).skip(3)
```
Vamos ordenar o nome das pessoas por ordem alfabética (sort) e idade decrescente:

```
db.getCollection('person').find({}).sort({"nome": 1, "idade": -1})
```