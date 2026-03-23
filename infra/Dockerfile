# Usa a imagem oficial do Nginx baseada no Alpine Linux (leve e segura)
FROM nginx:alpine

# Remove o arquivo de configuração e páginas HTML padrões, por precaução (opcional)
RUN rm -rf /usr/share/nginx/html/*

# Copia nosso index.html para o diretório servido pelo Nginx
COPY src/index.html /usr/share/nginx/html/

# Expõe a porta 80, padrão de web servers
EXPOSE 80

# Comando de execução quando o contêiner inicia
CMD ["nginx", "-g", "daemon off;"]
