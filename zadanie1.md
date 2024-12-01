Projekt aplikacji internetowej:
Po uruchomieniu wyświetla adress IP użytkwnika oraz datę i godzinę strefy czasowej.

Podpunkt 3. z instrukcji:
Polecenie do zbudowania kontenera:
```sh
docker build -t zadanie1 .
```

Polecenie do uruchomienia kontenera:
```sh
docker run -d -p 5000:5000 --name server_flask  zadanie1
```

sposób uzyskania informacju wygenerowanych prz starcie kontenera:
```sh
docker logs server_flask
```

sprawdzenie ilości warstw:
```sh
docker history zadanie1
```


Polecenia do części dodatkowej:
1.
```sh
docker buildx build -q -f Dockerfile -t docker.io/jhooman/zad1:server_flask --platform linux/amd64,linux/arm64 --push .
```

Adres repozytorium docker
https://hub.docker.com/r/jhooman/zad1
