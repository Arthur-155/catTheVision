## 5. Casos de Uso

### 5.1. Enviar Aula
**Ator Principal:** Professor  
**Pré-condição:** Estar cadastrado na plataforma.  

**Fluxo Principal:**  
1. Selecionar “Enviar aula” no topo do hub;  
2. Sistema exibe formulário para envio: nome da aula e tema;  
3. Preencher todos os campos obrigatórios;  
4. Vídeo enviado passa por triagem para aprovação;  
5. Após aprovação, exibe mensagem de sucesso;  
6. Conteúdo é postado e armazenado na plataforma.  

**Fluxo Alternativo:**  
- Caso algum campo obrigatório não seja preenchido, o sistema exibe mensagem de erro e impede o envio;  
- Após publicado, o vídeo recebe avaliações que geram a média de nota do professor.  

---

### 5.2. Cadastro de Login
**Ator Principal:** Usuário  
**Pré-condição:** Possuir e-mail válido para confirmação.  

**Fluxo Principal:**  
1. No menu principal, selecionar a opção de login;  
2. Sistema exibe campos de login e senha, além da opção “Não possui cadastro? Registre-se”;  
3. Ao selecionar “Registrar”, o sistema solicita: Nome Completo, Nome de Usuário, Senha, Confirmar Senha, E-mail, Data de Nascimento e Instituição de Ensino (opcional);  
4. Sistema verifica preenchimento dos campos e envia e-mail de confirmação;  
5. Usuário confirma o cadastro via e-mail e é direcionado para a plataforma;  
6. Sistema salva o cadastro.  

**Fluxo Alternativo:**  
- Usuário pode acessar a tela de cadastro diretamente via link.  

---

### 5.3. Assistir Aula
**Ator Principal:** Usuário (aluno ou não)  
**Pré-condição:** Estar cadastrado na plataforma e ter acesso à internet.  

**Fluxo Principal:**  
1. No menu principal, selecionar a opção “Módulos”;  
2. Sistema exibe lista de módulos disponíveis com título, linguagem abordada e tempo de duração;  
3. Usuário seleciona um módulo;  
4. Sistema mostra a quantidade de aulas do módulo selecionado;  
5. Usuário assiste ao conteúdo;  
6. Ao final, o usuário pode deixar uma avaliação ou comentário sobre a aula.  

**Fluxo Alternativo:**  
- Caso a conexão com a internet falhe durante a reprodução, o sistema exibe mensagem de erro e oferece a opção de tentar novamente;  
- Se o vídeo não estiver mais disponível, exibe mensagem informando a indisponibilidade.  

---

### 5.4. Gerenciar Perfil
**Ator Principal:** Usuário  
**Pré-condição:** Estar logado na plataforma.  

**Fluxo Principal:**  
1. No menu principal, selecionar sua foto de perfil, localizado na direita superior;  
2. O sistema exibe algumas opções;  
3. Clicar em "Meu Perfil";  
4. Sistema exibe as informações cadastradas do usuário: Nome Completo, Nome de Usuário, E-mail, Data de Nascimento e Instituição de Ensino (se informada);  
5. Usuário seleciona “Editar Perfil”;  
6. Sistema exibe campos para edição dos dados (exceto Nome de Usuário, que é fixo);  
7. Usuário realiza as alterações desejadas e confirma;  
8. Sistema valida os dados e salva as alterações;  
9. Mensagem de confirmação é exibida e as novas informações ficam disponíveis.  

**Fluxo Alternativo:**  
- Se algum campo obrigatório não for preenchido corretamente, o sistema exibe mensagem de erro e impede a atualização;  
- Usuário pode optar por cancelar a edição a qualquer momento, retornando para a tela de perfil.  

---

### 5.5. Pesquisar e Filtrar Aulas
**Ator Principal:** Usuário (aluno ou não)  
**Pré-condição:** Estar logado na plataforma e ter acesso à internet.  

**Fluxo Principal:**  
1. No menu principal, selecionar a opção “Módulos”;  
2. Sistema exibe campos de filtro por tema, professor ou avaliação mínima;  
3. Usuário seleciona os filtros desejados e confirma;  
4. Sistema exibe a lista de aulas ou módulos que atendem aos critérios selecionados, com título, linguagem abordada e tempo de duração;  
5. Usuário escolhe uma das aulas para assistir;  
6. Fluxo segue conforme o caso de uso “Assistir Aula”.  

**Fluxo Alternativo:**  
- Se nenhum filtro for aplicado, o sistema lista todas as aulas disponíveis;  
- Se não houver resultados para os filtros aplicados, o sistema exibe mensagem “Nenhum conteúdo encontrado” e oferece a opção de limpar os filtros.  

---

### 5.6. Acessar Mural (Geral e Específico)
**Ator Principal:** Usuário (aluno ou não)  
**Pré-condição:** Estar logado na plataforma.  

**Fluxo Principal:**  
1. No menu principal, selecionar a opção “Mural”;  
2. O sistema exibe a aba Mural Geral contendo temas diversos, incluindo matérias que ainda não possuem módulos disponíveis;  
3. Usuário pode visualizar, comentar ou iniciar um novo tema no Mural Geral;  
4. Ao acessar um módulo específico (ex: Java), o sistema exibe a aba Mural do Módulo;  
5. O Mural do Módulo contém tópicos relacionados ao tema do módulo (ex: abstração em Java);  
6. Usuário pode visualizar, comentar ou iniciar discussões específicas no Mural do Módulo.  

**Fluxo Alternativo:**  
- Se não houver tópicos no mural, o sistema exibe a mensagem “Ainda não há discussões neste mural. Seja o primeiro a criar uma!”;  
- Caso o usuário não esteja logado, o sistema exibe mensagem de erro e redireciona para login.  

---

### 5.7. Sistema de Pontos e Ranking de Usuários
**Ator Principal:** Usuário (aluno)  
**Pré-condição:** Estar logado na plataforma.  

**Fluxo Principal:**  
1. Usuário assiste a uma aula até o final;  
2. O sistema concede automaticamente X pontos ao usuário;  
3. Os pontos são acumulados no perfil do usuário;  
4. O sistema gera um ranking dos Top Usuários, baseado na quantidade total de pontos;  
5. O ranking é exibido em uma aba específica chamada Ranking no menu principal.  

**Fluxo Alternativo:**  
- Caso o usuário não conclua a aula, os pontos não são contabilizados;  
- Se houver empate de pontos, o sistema desempata pelo maior número de aulas assistidas.  

---

### 5.8. Ranking de Professores
**Ator Principal:** Usuário (aluno) e Sistema  
**Pré-condição:** Existirem aulas avaliadas por usuários.  

**Fluxo Principal:**  
1. Usuário assiste uma aula e pode avaliá-la ao final;  
2. O sistema registra a avaliação (nota de 1 a 5, por exemplo);  
3. O sistema calcula automaticamente a média das notas de cada professor;  
4. O sistema exibe um Ranking de Professores, ordenando do maior para o menor desempenho médio;  
5. O ranking pode ser acessado por qualquer usuário no menu principal.  

**Fluxo Alternativo:**  
- Se um professor ainda não tiver recebido avaliações, ele não aparece no ranking;  
- Caso dois professores tenham a mesma média, o sistema desempata pelo maior número de avaliações recebidas.  

---

### 5.9. Restringir Acesso às Aulas sem Login
**Ator Principal:** Usuário (não logado)  
**Pré-condição:** Não estar autenticado na plataforma.  

**Fluxo Principal:**  
1. Usuário tenta acessar uma aula ou módulo sem estar logado;  
2. O sistema identifica que não há sessão ativa;  
3. O sistema exibe mensagem: “É necessário estar logado para assistir às aulas.”;  
4. O sistema redireciona o usuário para a tela de Login/Registro.  

**Fluxo Alternativo:**  
- Caso o usuário já esteja logado, o fluxo segue normalmente conforme UC 5.3 – Assistir Aula.  

---

### 5.10. Atribuição de Tags para Usuários Ativos
**Ator Principal:** Sistema  
**Pré-condição:** Usuário logado e ativo na plataforma.  

**Fluxo Principal:**  
1. O sistema acompanha a atividade dos usuários (ex: quantidade de aulas assistidas, participação em murais, avaliações feitas);  
2. Usuários com atividade frequente recebem tags automáticas (ex: “Aluno Focado”, “Aluno Participativo”);  
3. As tags ficam visíveis no perfil do usuário e em suas interações (murais, comentários, rankings).  

**Fluxo Alternativo:**  
- Se o usuário reduzir sua atividade, a tag pode ser removida ou substituída por outra condizente com seu comportamento atual.  

---

### 5.11. Atribuição da Tag de Professor Confiável
**Ator Principal:** Sistema e Administradores  
**Pré-condição:** Usuário já ter enviado pelo menos 3 aulas.  

**Fluxo Principal:**  
1. Quando um usuário envia sua 3ª aula, o sistema concede automaticamente a tag “Professor”;  
2. Usuários com essa tag passam a ter seus vídeos publicados diretamente, sem triagem;  
3. A tag é exibida no perfil do usuário e em suas aulas.  

**Fluxo Alternativo:**  
- Caso um usuário com tag “Professor” publique conteúdo contra os ideais da plataforma, os administradores podem remover a tag e voltar a exigir triagem para novos envios.  

---

### 5.12. Denunciar Aula
**Ator Principal:** Usuário (aluno ou professor)  
**Pré-condição:** Aula publicada na plataforma.  

**Fluxo Principal:**  
1. Usuário acessa uma aula e seleciona a opção “Denunciar Aula”;  
2. O sistema solicita que o usuário escolha ou descreva o motivo da denúncia (ex: conteúdo impróprio, plágio, desrespeito às regras);  
3. O sistema registra a denúncia e envia para análise dos administradores;  
4. Administradores avaliam a denúncia e podem manter ou remover a aula da plataforma.  

**Fluxo Alternativo:**  
- Caso a denúncia seja considerada inválida, o vídeo permanece ativo e o usuário denunciante recebe uma notificação sobre a decisão.  

---

### 5.13. Expandir Temas Além de Programação
**Ator Principal:** Administradores e Professores  
**Pré-condição:** Plataforma em funcionamento.  

**Fluxo Principal:**  
1. Administradores criam novas categorias de módulos (ex: Psicologia, Matemática, Direito, etc.);  
2. Professores podem enviar aulas vinculadas a esses novos temas;  
3. Usuários podem pesquisar, filtrar e acessar conteúdos de qualquer área, não apenas programação.  

**Fluxo Alternativo:**  
- Caso ainda não haja aulas em um tema, o sistema exibe mensagem: “Ainda não há conteúdo disponível nesta categoria. Seja o primeiro a contribuir!”.  
