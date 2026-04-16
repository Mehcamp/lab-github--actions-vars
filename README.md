Por que a Secret aparece no log como "\*\*" e a variável aparece
normalmente?

Resposta:
Porque o GitHub mascara automaticamente valores sensíveis nos logs para evitar vazamento.

O Job deploy_app consegue ler a variável BUILD_VERSION criada no Job
build_app? Por quê?

Resposta:
Não, porque cada job roda em um ambiente isolado (runner diferente), e variáveis não são compartilhadas automaticamente entre jobs.
