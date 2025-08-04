# my-docker-compose

Meu repositório pessoal para armazenar o compose para uso em projetos de pesquisas e estudos.

## Serviços disponíveis

- **MLflow**: Plataforma para gerenciamento de experimentos de machine learning. Interface web acessível em `http://localhost:5001`.
- **PostgreSQL**: Banco de dados relacional utilizado como backend do MLflow. Porta padrão: `5432`.
- **MinIO**: Armazenamento de objetos compatível com S3, utilizado para armazenar artefatos do MLflow. API S3: `http://localhost:9003`, Console: `http://localhost:9002`.
- **SonarQube Community**: Ferramenta de análise de qualidade e segurança de código. Interface web em `http://localhost:9000`.

## Como usar

1. Certifique-se de ter o Docker e Docker Compose instalados.
2. Execute os serviços:
   ```sh
   docker compose up -d
   ```
3. Acesse as interfaces web pelos endereços acima.

## Observações

- As credenciais padrão estão definidas para facilitar testes locais. Recomenda-se alterá-las em ambientes de produção.
- Os volumes garantem persistência dos dados dos serviços.
