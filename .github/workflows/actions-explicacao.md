# 📘 Workflows vs Actions

- **Workflow**: Um arquivo YAML localizado em `.github/workflows/`, que descreve o processo completo de integração/entrega.
- **Action**: Um bloco de execução reutilizável dentro do workflow. Pode ser uma action pronta do marketplace ou personalizada.

### Exemplo:

```yaml
- name: Setup Java
  uses: actions/setup-java@v4
