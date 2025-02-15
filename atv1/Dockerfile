# a. Utilize a imagem oficial do “nginx” como base.
FROM nginx:alpine

# b. O diretório de trabalho dentro do container deverá ser o “/app”.
WORKDIR /app

# c. O arquivo “index.html” deverá ser copiado para o diretório de trabalho definido acima.
COPY index.html /app

# d. Utilize uma variável de ambiente chamada “APP_VERSION”, essa variável deverá ter o valor “1.0.0”.
ENV APP_VERSION=1.0.0

# e. Garanta que exista uma instrução para que o serviço do “nginx” execute assim que o container seja iniciado.
CMD ["nginx", "-g", "daemon off;"]

# f. A porta de comunicação na rede, deverá ser a porta “TCP/80”.
EXPOSE 80

# g. Na imagem deverão ser instalados alguns aplicativos, como: “curl, htop e wget”.
RUN apk add --no-cache curl htop wget
