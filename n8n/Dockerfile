# Use a imagem do n8n
FROM n8nio/n8n:latest

# Defina as variáveis de ambiente, que serão configuradas no Cloud Run
ENV DB_TYPE=postgresdb
ENV N8N_DIAGNOSTICS_ENABLED=false
ENV N8N_PERSONALIZATION_ENABLED=false

# Copie a pasta de backup para o container
COPY ./backup /backup

# Porta para expor o serviço n8n
EXPOSE 5678
