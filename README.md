### Linux
O comando "mv" tem a função de mover arquivos. A utilização dele é praticamente igual  a do comando cp. Exemplo:
$ mv MV.txt /home/baixaki/Trabalho/MV.txt  - O arquivo MV.txt foi movido para a pasta /home/baixaki/Trabalho com o mesmo nome.
$ mv MV.txt  VM.txt – O arquivo MV.txt continuou onde estava, porém, agora possui o nome de VM.txt.

sudo apt-get install -f : Para instalar todas as dependencias do pacote

Para renomear arquivos: mv (nome do arquivo atual) (nome do arquivo que deseja)



### Docker
docker ps : mostrar containers ativas
docker ps -a : mostrar todas as containers
docker start (id container): iniciar uma containers
docker stop (id container): parar uma containers

### MongoDB

Para filtrar um range de datas:

db.getCollection('nome da collection').find({ 
    "createdAt": {
        $gte: ISODate("2020-04-06T00:00:00.000-03:00"),
        $lt: ISODate("2020-04-22T23:59:59.999-03:00")
    }
})
