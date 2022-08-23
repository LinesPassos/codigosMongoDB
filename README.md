#### Contexto
db = Nome da database usada

cl = Nome da collection usada

k = key hipotetica

v = value hipotetica


# Comandos basicos
### use db
Seleciona a base de dados a ser acessada pelos comandos

# Comandos de QUERY

## Find

### db.cl.find({k : v, k1 : v1...}
Retorna TODOS os valores com pares chave-valor IDENTICOS aos passados nos parametros

### db.cl.findOne({k : v, k1 : v1...})
O mesmo que o find, mas só retorna o primeiro valor encontrado

# Comando de CRUD

## CREATE
**db.cl.insertOne({k : v, k1 : v1...})**
