# Use uma imagem base com a JDK do Java
FROM openjdk:17

# Copie os arquivos Java para dentro do contêiner
COPY . /usr/src/app

# Defina o diretório de trabalho
WORKDIR /usr/src/app

# Compile os arquivos Java
RUN javac *.java

# Execute o programa Java
CMD ["java", "Main"]
