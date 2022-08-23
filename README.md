#### Contexto
*db = Nome da database usada*

*cl = Nome da collection usada*

*k = key hipotetica*

*v = value hipotetica*

*dir = diretorio do arquivo hipotetico*


# Comandos basicos

### show databases
Mostra todas as databases disponiveis.

### use db
Seleciona a database a ser acessada pelos comandos.

### show collections
Mostra todas as collections na database selecionada.

# Comandos de QUERY

## Find

### db.cl.find({k : v, k1 : v1...}
Retorna TODOS os documentos com pares chave-valor IDENTICOS aos passados nos parametros.

### db.cl.findOne({k : v, k1 : v1...})
O mesmo que o find, mas só retorna o primeiro valor encontrado.

# Comandos de CRUD

## CREATE

### db.cl.insertOne({k : v, k1 : v1...})
Insere um documento na collection selecionada no comando.

## DELETE
### db.dropDatabase()
Apaga a database.

### db.cl.drop()
Apaga a colletion.

# Comandos de importação e exportação

## Databases com apenas uma collection

### mongoexport -c *cl* -d *db* -o *dir*

### mongoimport *dir* -d *db* -c *cl*

## Databases com multiplas collections

### mongodump -d *db* -o *dir*
Usado para exportação

### mongorestore *dir*
Usado para importação
