# torrents

## Descrição

Este repositório contém as especificações do docker-composer para executar cliente torrent baseado na imagem [bishof/torrent](https://hub.docker.com/r/bishof/torrent)

## Executando

```bash
docker-compose up
```

### Para executar em modo daemon

```bash
docker-compose up -d
```

### Interrompendo a execução

```bash
docker-compose down
```

## Informações sobre rede

O client torrent escutará na porta **49184**, se necessário crie uma regra de redirecionamento NAT no seu roteador.

O serviço web do rutorrent estará escudando na porta **8089**, acesse [localhost:8089](http://localhost:8089) no navegador de sua preferência.

Caso deseje alterar as portas altere as respectivas linhas no arquivo **docker-compose.yml**, não altere as portas após os dois pontos **:**.

## Localização dos arquivos

* cfg/.rtorrent.rc = Arquivo de configuração
* data/  = Dados baixados
