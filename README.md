<h1>CatTheVision</h1>

<h2>1. Visão Geral</h2>

<p><strong>Problema:</strong><br>
Alunos universitários que enfrentam dificuldades de aprendizado.</p>

<p><strong>Solução:</strong><br>
Uma plataforma comunitária que incentiva a ajuda mútua entre alunos, permitindo que tirem dúvidas e contribuam para a formação uns dos outros.</p>

<p><strong>Usuários e Clientes:</strong><br>
Qualquer pessoa interessada em conteúdos acadêmicos, independentemente do curso (engenharia, arquitetura, etc.).</p>

<p><strong>Recursos Principais:</strong></p>
<ul>
  <li>Envio de vídeos da comunidade para a plataforma;</li>
  <li>Visualização e feedback dos conteúdos publicados.</li>
</ul>

<p><strong>Canais:</strong><br>
Web e Mobile</p>

<p><strong>Custo e Receita:</strong><br>
Plataforma comunitária sem foco inicial em monetização. Uso gratuito.</p>

<hr>

<h2>2. Etapa 1</h2>

<p><strong>Nome do Sistema:</strong><br>CatTheVision</p>

<p><strong>Objetivo do Sistema:</strong><br>
Incentivar a troca de conhecimento entre pessoas (alunos ou não), permitindo que dúvidas sejam respondidas e que o processo de aprendizado seja enriquecido.<br>
- Usuários que consomem vídeos recebem conteúdo direcionado.<br>
- Usuários que produzem vídeos desenvolvem habilidades de comunicação e reforçam seu próprio aprendizado.</p>

<p><strong>Usuários Principais:</strong><br>Alunos universitários.</p>

<p><strong>Principais Funcionalidades:</strong></p>
<ul>
  <li>Envio de vídeos para a plataforma;</li>
  <li>Visualização dos vídeos.</li>
</ul>

<p><strong>Problema Resolvido:</strong><br>
Dificuldade de aprendizado em sala de aula.</p>

<p><strong>Recursos Desejados:</strong><br>
Estrutura de feedbacks para avaliação de conteúdos.</p>

<p><strong>Plataformas:</strong><br>
Web e Mobile.</p>

<p><strong>Prazos e Expectativas:</strong><br>
Novembro de 2025.</p>

<hr>

<h2>3. Requisitos Funcionais</h2>
<p>(Funções que o sistema precisa executar)</p>
<ul>
  <li>Cadastro de usuários com dados pessoais e e-mail para confirmação;</li>
  <li>Login e autenticação de usuários registrados;</li>
  <li>Envio de vídeos por usuários autorizados (professores e/ou membros da comunidade);</li>
  <li>Triagem e aprovação de vídeos antes da publicação;</li>
  <li>Visualização de vídeos por qualquer usuário autenticado;</li>
  <li>Sistema de avaliação (nota e/ou comentários) para cada vídeo;</li>
  <li>Listagem de aulas com filtros por tema, professor ou avaliação;</li>
  <li>Armazenamento seguro dos vídeos e metadados (título, descrição, professor, data);</li>
  <li>Notificações por e-mail para confirmação de cadastro e aprovação de vídeos;</li>
  <li>Gestão de perfis (visualização e edição de dados do usuário).</li>
</ul>

<h2>4. Requisitos Não Funcionais</h2>
<p>(Características de qualidade do sistema)</p>
<ul>
  <li><strong>Acessibilidade:</strong> Deve funcionar em navegadores modernos e dispositivos móveis;</li>
  <li><strong>Disponibilidade:</strong> Sistema online 24/7 com tempo de inatividade mínimo;</li>
  <li><strong>Desempenho:</strong> Carregar vídeos e páginas em até 6 segundos em conexão padrão;</li>
  <li><strong>Usabilidade:</strong> Interface simples, intuitiva e responsiva;</li>
  <li><strong>Compatibilidade:</strong> Funcionar nos principais sistemas operacionais (Windows, macOS, Android, iOS);</li>
</ul>

<hr>

<h2>5. Casos de Uso</h2>

<h3>5.1. Enviar Aula</h3>
<p><strong>Ator Principal:</strong> Professor<br>
<strong>Pré-condição:</strong> Estar cadastrado na plataforma.</p>

<p><strong>Fluxo Principal:</strong></p>
<ol>
  <li>Selecionar “Enviar aula” no topo do hub;</li>
  <li>Sistema exibe formulário para envio: nome da aula e tema;</li>
  <li>Preencher todos os campos obrigatórios;</li>
  <li>Vídeo enviado passa por triagem para aprovação;</li>
  <li>Após aprovação, exibe mensagem de sucesso;</li>
  <li>Conteúdo é postado e armazenado na plataforma.</li>
</ol>

<p><strong>Fluxo Alternativo:</strong></p>
<ul>
  <li>Caso algum campo obrigatório não seja preenchido, o sistema exibe mensagem de erro e impede o envio;</li>
  <li>Após publicado, o vídeo recebe avaliações que geram a média de nota do professor.</li>
</ul>

<hr>

<h3>5.2. Cadastro de Login</h3>
<p><strong>Ator Principal:</strong> Usuário<br>
<strong>Pré-condição:</strong> Possuir e-mail válido para confirmação.</p>

<p><strong>Fluxo Principal:</strong></p>
<ol>
  <li>No menu principal, selecionar a opção de login;</li>
  <li>Sistema exibe campos de login e senha, além da opção “Não possui cadastro? Registre-se”;</li>
  <li>Ao selecionar “Registrar”, o sistema solicita: Nome Completo, Nome de Usuário, Senha, Confirmar Senha, E-mail, Data de Nascimento e Instituição de Ensino (opcional);</li>
  <li>Sistema verifica preenchimento dos campos e envia e-mail de confirmação;</li>
  <li>Usuário confirma o cadastro via e-mail e é direcionado para a plataforma;</li>
  <li>Sistema salva o cadastro.</li>
</ol>

<p><strong>Fluxo Alternativo:</strong></p>
<ul>
  <li>Usuário pode acessar a tela de cadastro diretamente via link.</li>
</ul>

<hr>

<h3>5.3. Assistir Aula</h3>
<p><strong>Ator Principal:</strong> Usuário (aluno ou não)<br>
<strong>Pré-condição:</strong> Estar cadastrado na plataforma e ter acesso à internet.</p>

<p><strong>Fluxo Principal:</strong></p>
<ol>
  <li>No menu principal, selecionar a opção “Módulos”;</li>
  <li>Sistema exibe lista de módulos disponíveis com título, linguagem abordada e tempo de duração;</li>
  <li>Usuário seleciona um módulo;</li>
  <li>Sistema mostra a quantidade de aulas do módulo selecionado;</li>
  <li>Usuário assiste ao conteúdo;</li>
  <li>Ao final, o usuário pode deixar uma avaliação ou comentário sobre a aula.</li>
</ol>

<p><strong>Fluxo Alternativo:</strong></p>
<ul>
  <li>Caso a conexão com a internet falhe durante a reprodução, o sistema exibe mensagem de erro e oferece a opção de tentar novamente;</li>
  <li>Se o vídeo não estiver mais disponível, exibe mensagem informando a indisponibilidade.</li>
</ul>

<hr>

<h3>5.4. Gerenciar Perfil</h3>
<p><strong>Ator Principal:</strong> Usuário<br>
<strong>Pré-condição:</strong> Estar logado na plataforma.</p>

<p><strong>Fluxo Principal:</strong></p>
<ol>
  <li>No menu principal, selecionar sua foto de perfil, localizado na direita superior;</li>
  <li>O sistema exibe algumas opções;</li>
  <li>Clicando em "Meu Perfil";</li>
  <li>Sistema exibe as informações cadastradas do usuário: Nome Completo, Nome de Usuário, E-mail, Data de Nascimento e Instituição de Ensino (se informada);</li>
  <li>Usuário seleciona “Editar Perfil”;</li>
  <li>Sistema exibe campos para edição dos dados (exceto Nome de Usuário, que é fixo);</li>
  <li>Usuário realiza as alterações desejadas e confirma;</li>
  <li>Sistema valida os dados e salva as alterações;</li>
  <li>Mensagem de confirmação é exibida e as novas informações ficam disponíveis.</li>
</ol>

<p><strong>Fluxo Alternativo:</strong></p>
<ul>
  <li>Se algum campo obrigatório não for preenchido corretamente, o sistema exibe mensagem de erro e impede a atualização;</li>
  <li>Usuário pode optar por cancelar a edição a qualquer momento, retornando para a tela de perfil.</li>
</ul>

<hr>

<h3>5.5. Pesquisar e Filtrar Aulas</h3>
<p><strong>Ator Principal:</strong> Usuário (aluno ou não)<br>
<strong>Pré-condição:</strong> Estar logado na plataforma e ter acesso à internet.</p>

<p><strong>Fluxo Principal:</strong></p>
<ol>
  <li>No menu principal, selecionar a opção “Módulos”;</li>
  <li>Sistema exibe campos de filtro por tema, professor ou avaliação mínima;</li>
  <li>Usuário seleciona os filtros desejados e confirma;</li>
  <li>Sistema exibe a lista de aulas ou módulos que atendem aos critérios selecionados, com título, linguagem abordada e tempo de duração;</li>
  <li>Usuário escolhe uma das aulas para assistir;</li>
  <li>Fluxo segue conforme o caso de uso “Assistir Aula”.</li>
</ol>

<p><strong>Fluxo Alternativo:</strong></p>
<ul>
  <li>Se nenhum filtro for aplicado, o sistema lista todas as aulas disponíveis;</li>
  <li>Se não houver resultados para os filtros aplicados, o sistema exibe mensagem “Nenhum conteúdo encontrado” e oferece a opção de limpar os filtros.</li>
</ul>
