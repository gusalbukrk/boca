- [Desenvolvimento de um Sistema de Apoio, Classificação e Organização de Competições de Programação](#desenvolvimento-de-um-sistema-de-apoio-classificação-e-organização-de-competições-de-programação)
  - [Funcionalidades](#funcionalidades)
    - [Essenciais](#essenciais)
    - [Não-essenciais](#não-essenciais)
    - [Fora do escopo](#fora-do-escopo)

</br>

# Desenvolvimento de um Sistema de Apoio, Classificação e Organização de Competições de Programação

O sistema a ser desenvolvido será composto por um banco de dados, a API que o gerenciará e dois clientes de front-end: uma aplicação web com o painel de controle do administrador e uma extensão do Visual Studio Code com o ambiente de desenvolvimento e submissão de código para os competidores.

## Funcionalidades

> desambiguação: gerenciamento refere-se à capacidade de performar operações básicas de banco de dados conhecidas como CRUD (create, read, update, delete).

### Essenciais

O MVP (minimum viable product) será composto pelas seguintes funcionalidades:

- sistema de cadastro/login
  - parâmetros: nome, e-mail, senha
- gerenciamento de competições
  - parâmetros: nome, data e hora de início, duração
- gerenciamento de usuários
  - 2 níveis de privilégio em uma competição — administrador e competidor
- gerenciamento de problemas
  - parâmetros: nome, descrição, cor
- gerenciamento de submissões
  - parâmetros: problema, linguagem de programação, código-fonte, horário da submissão
  - notificações devem ser disparadas quando uma solução é submetida e corrigida
- visualização do placar em tempo-real

### Não-essenciais

Após a entrega do MVP, planeja-se a implementação das seguintes funcionalidades priorizadas na seguinte ordem:

- correção automática de submissões
  - durante o cadastramento de um problema, o administrador deve enviar arquivos de teste
  - após a submissão, o sistema deve executar o código-fonte, realizar a comparação com os arquivos de teste e retornar o resultado automaticamente
  - a execução de código-fonte de diferentes linguagens vai demandar a instalação de vários compiladores e interpretadores no servidor e abrir brechas de segurança
- medidas anti-fraude (isolamento de rede e mídia física para competidores)
  - restringir o acesso de rede exclusivamente ao servidor do sistema
  - impedir o uso de dispositivos de armazenamento externo
  - limitar o acesso de arquivos no disco de armazenamento interno
- gerenciamento de esclarecimentos
  - parâmetros: problema, usuário, pergunta, resposta
  - competidores podem enviar dúvidas e o administrador responde (opcionalmente, a resposta pode ser pública); o administrador pode também enviar avisos para todos os competidores
  - notificações devem ser disparadas quando uma pergunta é feita e respondida
- elaboração automática de um relatório após a finalização da competição
  - o relatório deve conter: o placar final, a lista de problemas e seus arquivos de testes, a lista de submissões e seus resultados, a lista de esclarecimentos e suas respostas
- customização do algoritmo de placar
- gerenciamento de entrega de balões
  - notificação deve ser disparada a cada vez que uma submissão é corrigida e o resultado é positivo
  - customização do item a ser usado como indicador visual de problemas
- melhorias diversas
  - ordenação e filtragem de linhas de tabelas
  - bulk import em formulários de cadastramento

### Fora do escopo

As seguintes funcionalidades não estão inclusas atualmente na trilha de desenvolvimento pois agregariam baixo valor ao sistema em comparação com as funcionalidades listadas nas seções anteriores e dificultariam a conclusão do projeto no prazo estabelecido:

- sistema de logs detalhado
- internacionalização (disponibilizar o sistema em múltiplos idiomas)
- múltiplos níveis de acesso para os organizadores (exemplo: juiz, staff, etc.)
