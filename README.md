<h1>DESAFIO - 4BLUE</h1>

<h2>Bugs encontrados</h2>

<h3>1 - Campos de cadastro sem validação</h3>
<p>
A tela de cadastro não exige o preenchimento de nenhum dos campos, permitindo a criação de uma conta sem o preenchimento de qualquer informação.
</p>

<h4>BDD:</h4>
<p>
Dado que eu esteja na tela de login <br>
E clique em "Não tem uma conta? Criar conta" <br>
E não preencha nenhum campo da tela de cadastro <br>
Quando clicar em "Criar conta" <br>
Então uma tela indicando sucesso na criação da conta será exibida
</p>

<h4>Evidência:</h4>
<p>
<a href="https://drive.google.com/file/d/1_dN_po6ZJpMXKhI6rgCAl-ug2KaGAcpT/view?usp=sharing">Ver evidência</a>
</p>

<h4>Resultado atual:</h4>
<p>
É possível criar uma conta sem preencher nenhuma informação.
</p>

<h4>Resultado esperado:</h4>
<p>
A tela deve exibir uma mensagem informando que o preenchimento dos campos é obrigatório para a criação de uma conta.
</p>

<h4>Severidade:</h4>
<p>Crítica</p>

<h4>Prioridade:</h4>
<p>Alta</p>

<hr>

<h3>2 - Criação de conta sem validação dos requisitos da senha</h3>
<p>
É possível criar uma conta sem preencher o campo de senha ou utilizando senhas que não atendem aos requisitos mínimos, que exigem pelo menos 8 caracteres e um caractere especial.
</p>

<h4>BDD:</h4>
<p>
Dado que eu esteja na tela de login <br>
E clique em "Não tem uma conta? Criar conta" <br>
E preencha os campos nome, telefone e e-mail <br>
E deixe o campo senha em branco ou preencha com "123456" <br>
Quando clicar em "Criar conta" <br>
Então uma tela indicando sucesso na criação da conta será exibida
</p>

<h4>Evidência:</h4>
<p>
<a href="https://drive.google.com/file/d/1kNdYh1LJ3Mqp5gZIN7yScTdMKHtTj4AL/view?usp=sharing">Ver evidência</a>
</p>

<h4>Resultado atual:</h4>
<p>
É possível criar uma conta com senha em branco ou com senha que não atende aos requisitos mínimos.
</p>

<h4>Resultado esperado:</h4>
<p>
O sistema deve exibir uma mensagem informando que a senha deve conter no mínimo 8 caracteres e um caractere especial.
</p>

<h4>Severidade:</h4>
<p>Crítica</p>

<h4>Prioridade:</h4>
<p>Alta</p>

<hr>

<h3>3 - Campo "Confirmar senha" permite senhas diferentes</h3>
<p>
É possível criar uma conta informando valores diferentes nos campos <strong>senha</strong> e <strong>confirmar senha</strong>.
</p>

<h4>BDD:</h4>
<p>
Dado que eu esteja na tela de login <br>
E clique em "Não tem uma conta? Criar conta" <br>
E preencha os campos nome, telefone e e-mail <br>
E preencha o campo senha com "123456" <br>
E preencha o campo confirmar senha com "123" <br>
Quando clicar em "Criar conta" <br>
Então uma tela indicando sucesso na criação da conta será exibida
</p>

<h4>Evidência:</h4>
<p>
<a href="https://drive.google.com/file/d/1pnMeJivzkXYHsNDA46JrvrKITbjH88Hn/view?usp=sharing">Ver evidência</a>
</p>

<h4>Resultado atual:</h4>
<p>
É possível criar uma conta com valores diferentes nos campos senha e confirmar senha.
</p>

<h4>Resultado esperado:</h4>
<p>
O sistema deve exibir uma mensagem informando que os campos senha e confirmar senha devem possuir o mesmo valor.
</p>

<h4>Severidade:</h4>
<p>Alta</p>

<h4>Prioridade:</h4>
<p>Alta</p>

<hr>

<h3>4 - Campo de telefone permite caracteres e quantidade ilimitada de dígitos</h3>
<p>
O campo de telefone aceita caracteres inválidos e permite o preenchimento com quantidade ilimitada de dígitos.
</p>

<h4>BDD:</h4>
<p>
Dado que eu esteja na tela de login <br>
E clique em "Não tem uma conta? Criar conta" <br>
E preencha o campo telefone com caracteres alfanuméricos ou com quantidade inválida de dígitos <br>
Quando clicar em "Criar conta" <br>
Então uma tela indicando sucesso na criação da conta será exibida
</p>

<h4>Evidência:</h4>
<p>
<a href="https://drive.google.com/file/d/1Y2n1-YCci-0WjW7QDddd-mUN3vmDKib5/view?usp=sharing">Ver evidência</a>
</p>

<h4>Resultado atual:</h4>
<p>
É possível criar uma conta com um telefone inválido.
</p>

<h4>Resultado esperado:</h4>
<p>
O campo de telefone deve aceitar apenas números e limitar o preenchimento a 9 dígitos.
</p>

<h4>Severidade:</h4>
<p>Média</p>

<h4>Prioridade:</h4>
<p>Média</p>

<hr>

<h3>5 - Criação de conta com e-mail já cadastrado</h3>
<p>
É possível criar mais de uma conta utilizando o mesmo e-mail.
</p>

<h4>BDD:</h4>
<p>
Dado que eu esteja na tela de login <br>
E clique em "Não tem uma conta? Criar conta" <br>
E preencha os campos nome, telefone, e-mail e senha <br>
E clique em "Criar conta" <br>
E repita o processo utilizando o mesmo e-mail anteriormente cadastrado <br>
Quando clicar em "Criar conta" pela segunda vez <br>
Então uma tela indicando sucesso na criação da conta será exibida
</p>

<h4>Evidência:</h4>
<p>
<a href="https://drive.google.com/file/d/12BY3itu1jpS_xD4Ef6_7AO7ILVhoJijx/view?usp=sharing">Ver evidência</a>
</p>

<h4>Resultado atual:</h4>
<p>
É possível criar mais de uma conta utilizando o mesmo e-mail.
</p>

<h4>Resultado esperado:</h4>
<p>
O sistema deve exibir uma mensagem informando que já existe uma conta cadastrada com esse e-mail.
</p>

<h4>Severidade:</h4>
<p>Crítica</p>

<h4>Prioridade:</h4>
<p>Alta</p>

<h2>Perguntas e respostas</h2>
<h3>Quais 2 bugs você corrigiria primeiro e por quê?</h3>
<p>O primeiro bug seria o 'Campos de cadastro sem validação' pois é um bug que quebra as regras de negócio. Ele permite com que usuários realizem login e cadastro dentro da plataforma sem identificação alguma. <br><br>
O segundo bug seria o 'Criação de conta sem validação dos requisitos da senha' pois é um bug que afeta a segurança. Permite com que usuários preencham os campos de senha com senhas fracas ou inexistentes fazendo com que os logins sejam extremamente vulneráveis.
</p>
<h3>Melhoria para as telas</h3>
<p>1 - A tela de cadastro apresenta incosistência nos campos, uma melhoria seria deixa-los alinhados com o retangulo do fundo e adicionar espaçamento entre eles.</p>
<a href="https://drive.google.com/file/d/1BR2aBA0hvuVq_5RqOcDGLqRaLozZ51er/view?usp=sharing">Imagem</a> <br> 
<br>
<p>2 - Outra melhoria seria retirar a mensagem 'A senha precisa ter no mínimo 8 caracteres e 1 caractere especial.' da tela de login pois ela deveria pertercer somente a tela de cadastro.</p>
<a href="https://drive.google.com/drive/folders/1ZhgIdz0Ud1xLPQmx0W9Ajx3aBwwcjvRs?usp=sharing">Imagem</a> <br>
<br>
<p>3 - Para usuários que esqueceram a senha, seria interessante disponibilizar uma URL com a opção "Esqueci a senha", redirecionando para a página de recuperação.</p>
