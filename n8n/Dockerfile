# Use a imagem do n8n
FROM n8nio/n8n:latest

# Defina as variáveis de ambiente padrão
ENV DB_TYPE=postgresdb
ENV N8N_DIAGNOSTICS_ENABLED=false
ENV N8N_PERSONALIZATION_ENABLED=false

# Defina a porta para o Cloud Run (porta padrão configurada pela variável `PORT`)
ENV PORT=8080

# Copie a pasta de backup para o container
COPY ./backup /backup

# Garanta que o n8n escute na porta definida pela variável `PORT`
CMD ["n8n"]

# Expõe a porta usada pelo serviço
EXPOSE 8080
