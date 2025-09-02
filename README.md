## Construindo a imagem

Dentro da pasta do projeto, execute:

```bash
docker build -t meu-nginx .
```

---

## Executando o container

Rode o Nginx mapeando a porta 8080 do host para a porta 80 do container:

```bash
docker run -d -p 8080:80 --name nginx-container meu-nginx
```

Agora abra no navegador:

```
http://localhost:8080
```

Você verá a página de teste

---

## Parando o container

Para parar:

```bash
docker stop nginx-container
```

Se quiser remover:

```bash
docker rm nginx-container
```

