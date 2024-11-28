# Repositório de Workflows Reutilizáveis

Este repositório contém uma coleção de workflows reutilizáveis para GitHub Actions. Estes workflows foram projetados para serem facilmente integrados em diferentes projetos, proporcionando automação e eficiência no desenvolvimento e implantação de software.

## Estrutura do Repositório

- **.github/workflows/**: Contém os arquivos YAML dos workflows reutilizáveis.
- **docs/**: Documentação detalhada sobre cada workflow disponível.
- **examples/**: Exemplos de uso dos workflows em diferentes cenários.

## Como Usar

1. **Clone o repositório**:
    ```sh
    git clone https://github.com/fssou/gh-workflows.git
    ```

2. **Inclua o workflow desejado no seu repositório**:
    No arquivo YAML do seu workflow, utilize a sintaxe `uses` para referenciar o workflow deste repositório. Por exemplo:
    ```yaml
    jobs:
        build:
            uses: fssou/gh-workflows/.github/workflows/[workflow-desejado].yml@[branch/tag]
    ```

3. **Personalize o workflow**:
    Edite o arquivo YAML conforme necessário para atender às necessidades específicas do seu projeto.

## Workflows Disponíveis

- **reusable-deploy-docker-compose-with-ssh.yml**: Workflow para implantação de serviços Docker Compose em um servidor remoto via SSH.

## Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests para adicionar novos workflows ou melhorar os existentes.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
