### Aluno
#### RF01, RF04, RF05, RF06, RF10
- idAluno
- nome
- cpf
- email
- telefone
- endereco
- rfid
- status
+ contratarPlano()
+ agendarAula()
+ cancelarAgendamento()
+ registrarAcesso()
+ receberNotificacap()

### Plano
#### RF01, RF02, RF04
- idPlano
- nome
- tipo
- valor
- ativo
+ registrar()
+ ativar()
 + desativar()
 + alterarValor()

### Pagamento
#### RF03, RF04, RF09
- idPagamento
- data
- valor
- formaPagamento
- status
+ registrar()
+ confirmar()
+ cancelar()

### Acesso
#### RF05, RF09
- idAcesso
- dataHora
- autorizado
+ registrar()
+ autorizar()
+ negar()

### Aula
#### RF06, RF07, RF09
- idAula
- nome
- horario
- capacidadeMaxima
+ disponibilizarHorario()
+ reservarVaga()
+ liberarVaga()
+ registrarPresenca()

### Agendamento
#### RF06, RF10
- idAgendamento
- dataReserva
- status
+ confirmar()
+ cancelar()

### Presenca
#### RF07
- idPresenca
- data
- presente
+ registrar()

### AvaliacaoFisica
#### RF08, RF10
- idAvaliacao
- data
- peso
- imc
- percentualGordura
- observacoes
- anexo
+ registrar()
+ AtualizarDados()
+ AnexarArquivo()

### Notificacao
#### RF10
- idNotificacao
- tipo
- dataEnvio
- status
- mensagem
+ enviarNotificacao()

### Instrutor
#### RF07, RF08
- idInstrutor
- nome
- especialidade
+ registrarPresenca()
+ registrarAvaliacaoFisica()

### Recepcionista
#### RF01, RF03
- idRecepcionista
- nome
+ cadastrarAluno()
+ receberPagamento()

### Gerente
#### RF02, RF09
- idGerente
- nome
+ gerenciarPlano+ emitirRelatorios()
