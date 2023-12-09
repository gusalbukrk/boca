- [BOCA](#boca)
  - [Funcionalidades](#funcionalidades)
    - [Níveis de acesso](#níveis-de-acesso)
      - [System](#system)
      - [Administrador](#administrador)
      - [Juiz](#juiz)
      - [Staff](#staff)
      - [Equipe competidora](#equipe-competidora)
      - [Placar](#placar)

</br>

# BOCA

## Funcionalidades

Tendo em vista a ampla utilização do BOCA, o detalhamento de suas funcionalidades se justifica como um meio de aperfeiçoar a compreensão das demandas específicas desse tipo de sistema.

### Níveis de acesso

O sistema BOCA possui seis níveis de acesso: system, administrador, juiz, staff, equipe competidora e placar. Apenas o system, administrador e equipe competidora são estritamente necessários. Em maratonas de pequeno porte, o administrador geralmente desempenha o papel de juiz e staff e não há a necessidade de disponibilizar o placar para o ambiente externo.

#### System

O BOCA pode gerenciar apenas uma competição por vez. O usuário `system` é o usuário responsável por criar e ativar uma competição. É somente após a competição ser ativada por esse usuário que se torna possível fazer login como o usuário administrador. A barra de navegação da interface do system apresenta os seguintes itens:

1. **Contest**: ativar uma competição nova ou existente e definir alguns parâmetros básicos da competição em andamento.
2. **Options**: trocar de nome de usuário e senha.
3. **Logout**

![](./img/system/contest.png "/system/contest.php")
*/system/contest.php*
</br>

![](./img/system/contest-id.png "/system/contest.php?contest=1")
*/system/contest.php?contest=1*
</br>

![](./img/system/option.png "/system/option.php")
*/system/option.php*
</br>

#### Administrador

O usuário do tipo administrador (que por padrão tem o nome de usuário `admin`) é a autoridade máxima do sistema. Além de possuir privilégios exclusivos, o administrador pode também desempenhar as funções de juiz e staff (podendo inclusive revisar ações de juízes e staff como, por exemplo, retirar tarefas de um staff e retificar correções de um juiz). A barra de navegação da interface do administrador apresenta os seguintes itens:

1. **Runs**: disponibilizar informações gerais de todas as submissões e link para gerenciar individualmente cada submissão.
2. **Score**: acompanhar em tempo-real o placar da competição.
3. **Clarifications**: disponibilizar informações gerais de todas as perguntas e link para gerenciar individualmente cada pergunta.
4. **Users**: adicionar novos usuários e visualizar informações dos usuários já cadastrados inclusive acompanhar se o usuário está atualmente logado no sistema.
5. **Problems**: gerar pacote de problema, adicionar novos problemas e visualizar informações, editar e excluir os problemas já cadastrados.
6. **Languages**: cadastrar, editar e excluir as linguagens permitidas para submissão.
7. **Answers**: cadastrar, editar e excluir as respostas possíveis que um juiz dará para uma submissão (é importante salientar que a equipe competidora não receberá nenhuma outra informação acerca do resultado da submissão além de uma das respostas predefinidas aqui).
8. **Misc**: opções de sistema variadas (limpar cache, atualizar, reverter atualização, etc.).
9. **Tasks**: gerenciar (encarregar-se, deletar, reabrir) as tarefas que foram solicitadas para a staff pelas equipes competidoras.
10. **Site**: visualizar e alterar diversos dados relativos a um site específico.
11. **Contest**: visualizar e alterar os dados gerais da competição ativa.
12. **Logs**: visualizar os registros de ocorrências — é possível alterar a ordem e aplicar filtros.
13. **Reports**: gerar relatórios variados.
14. **Backups**: visualizar os backups realizados pelos usuários.
15. **Options**: alterar informações pessoais.
16. **Logout**

![](./img/admin/run.png "/admin/run.php")
*/admin/run.php*
</br>

![](./img/admin/runedit.png "/admin/runedit.php")
*/admin/runedit.php*
</br>

![](./img/admin/score.png "/admin/score.php")
*/admin/score.php*
</br>

![](./img/admin/clar.png "/admin/clar.php")
*/admin/clar.php*
</br>

![](./img/admin/claredit.png "/admin/claredit.php")
*/admin/claredit.php*
</br>

![](./img/admin/user.png "/admin/user.php")
*/admin/user.php*
</br>

![](./img/admin/problem.png "/admin/problem.php")
*/admin/problem.php*
</br>

![](./img/admin/buildproblem.png "/admin/buildproblem.php")
*/admin/buildproblem.php*
</br>

![](./img/admin/language.png "/admin/language.php")
*/admin/language.php*
</br>

![](./img/admin/answer.png "/admin/answer.php")
*/admin/answer.php*
</br>

![](./img/admin/misc.png "/admin/misc.php")
*/admin/misc.php*
</br>

![](./img/admin/task.png "/admin/task.php")
*/admin/task.php*
</br>

![](./img/admin/site.png "/admin/site.php")
*/admin/site.php*
</br>

![](./img/admin/contest.png "/admin/contest.php")
*/admin/contest.php*
</br>

![](./img/admin/log.png "/admin/log.php")
*/admin/log.php*
</br>

![](./img/admin/report.png "/admin/report.php")
*/admin/report.php*
</br>

![](./img/admin/files.png "/admin/files.php")
*/admin/files.php*
</br>

![](./img/admin/option.png "/admin/option.php")
*/admin/option.php*
</br>

#### Juiz

O usuário do tipo juiz é encarregado de responder perguntas e analisar e corrigir submissões. A barra de navegação da interface do juiz apresenta os seguintes itens:

1. **Runs**: visualizar as submissões realizadas que ainda não foram processadas.
2. **All runs**: visualizar todas as submissões independentemente do status.
3. **Score**: acompanhar em tempo-real o placar da competição.
4. **Clarifications**: visualizar as perguntas enviadas pelas equipes competidoras e respondê-las.
5. **History**: visualizar todas as perguntas e submissões já realizadas e em destaque as que foram processadas pelo juiz atualmente logado.
6. **As Team**: submeter resoluções para fins de teste.
7. **Options**: alterar informações pessoais.
8. **Logout**

![](./img/judge/run.png "/judge/run.php")
*/judge/run.php*
</br>

![](./img/judge/runedit.png "/judge/runedit.php")
*/judge/runedit.php*
</br>

![](./img/judge/allrunlist.png "/judge/allrunlist.php")
*/judge/allrunlist.php*
</br>

![](./img/judge/runview.png "/judge/runview.php")
*/judge/runview.php*
</br>

![](./img/judge/score.png "/judge/score.php")
*/judge/score.php*
</br>

![](./img/judge/clar.png "/judge/clar.php")
*/judge/clar.php*
</br>

![](./img/judge/claredit.png "/judge/claredit.php")
*/judge/claredit.php*
</br>

![](./img/judge/history.png "/judge/history.php")
*/judge/history.php*
</br>

![](./img/judge/team.png "/judge/team.php")
*/judge/team.php*
</br>

![](./img/judge/option.png "/judge/option.php")
*/judge/option.php*
</br>

#### Staff

As funções do pessoal de staff são: fazer as impressões solicitadas pelas equipes competidoras, entregar balões a cada vez que uma equipe submete uma resolução correta e dar assistência com problemas de software e hardware. São tarefas que (diferentemente das competências do administrador e juiz) demandam interação física com as equipes competidoras, no entanto, são geridas também através do BOCA. A barra de navegação da interface da staff apresenta os seguintes itens:

1. **Tasks**: visualizar todas as tarefas e gerenciar (se encarregar, devolver e marcar como completa) as tarefas em aberto.
2. **Score**: acompanhar em tempo-real o placar da competição.
3. **Runs**: visualizar todas as submissões já realizadas.
4. **Logout**

![](./img/staff/task.png "/staff/task.php")
*/staff/task.php*
</br>

![](./img/staff/score.png "/staff/score.php")
*/staff/score.php*
</br>

![](./img/staff/run.png "/staff/run.php")
*/staff/run.php*
</br>

#### Equipe competidora

A barra de navegação da interface da equipe competidora apresenta os seguintes itens:

1. **Problems**: visualizar os problemas da competição.
2. **Runs**: submeter resoluções e visualizar as submissões já realizadas.
3. **Score**: acompanhar em tempo-real o placar da competição.
4. **Clarifications**: enviar perguntas para os organizadores e visualizar as respostas recebidas.
5. **Tasks**: enviar arquivos para impressão ou solicitar assistência presencial.
6. **Backups**: salvar arquivos variados no servidor para que possam ser baixados posteriormente, útil para casos em que é necessário que a equipe competidora troque de máquina.
7. **Options**: alterar informações pessoais.
8. **Logout**

![](./img/team/problem.png "/team/problem.php")
*/team/problem.php*
</br>

![](./img/team/run.png "/team/run.php")
*/team/run.php*
</br>

![](./img/team/score.png "/team/score.php")
*/team/score.php*
</br>

![](./img/team/clar.png "/team/clar.php")
*/team/clar.php*
</br>

![](./img/team/task.png "/team/task.php")
*/team/task.php*
</br>

![](./img/team/files.png "/team/files.php")
*/team/files.php*
</br>

![](./img/team/option.png "/team/option.php")
*/team/option.php*
</br>

#### Placar

O usuário do tipo placar existe para possibilitar a visualização do placar da competição para pessoas que não desempenham nenhum outro papel no sistema. A barra de navegação da interface do placar apresenta os seguintes itens:

1. **Score**
2. **Logout**

![](./img/score/index.png "/score/index.php")
*/score/index.php*
</br>
