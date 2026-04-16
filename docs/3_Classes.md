**Aluno**
RF01, RF04, RF05, RF06, RF10
- idAluno
- nome
- cpf
- email
- telefone
- endereco
- rfid
- status
- estaRegular()
- agendarAula()
- receberNotificacao()
- contratarPlano()
- cancelarAgendamento()
- registrarAcesso()

**Plano**
RF01, RF02, RF04
- idPlano
- nome
- tipo
- valor
- ativo
- ativar()
- desativar()
- alterarValor()

**Pagamento**
RF03, RF04, RF09
- idPagamento
- data
- valor
- formaPagamento
- status
- registrar()
- confirmar()
- cancelar()

**Acesso**
RF05, RF09
- idAcesso
- dataHora
- autorizado
- registrar()
- autorizar()
- negar()

**Aula**
RF06, RF07, RF09
- idAula
- nome
- horario
- capacidadeMaxima

**Agendamento**
RF06, RF10
- idAgendamento
- dataReserva
- status

**Presenca**
RF07
- idPresenca
- data
- presente
- disponibilizarHorario()
- reservarVaga()
- liberarVaga()
- registrarPresenca()

**AvaliacaoFisica**
RF08, RF10
- idAvaliacao
- data
- peso
- imc
- percentualGordura
- observacoes
- anexo
- registrar()
- atualizarDados()
- anexarArquivo()

**Notificacao**
RF10
- idNotificacao
- tipo
- dataEnvio
- status
- mensagem
- tipo: TipoNotificacao
- enviar()
- marcarComoLida()

**Instrutor**
RF07, RF08
- idInstrutor
- nome
- especialidade
- registrarPresenca()
- realizarAvaliacaoFisica()

**Recepcionista**
RF01, RF03
- idRecepcionista
- nome
- cadastrarAluno()
- registrarPagamento()

**Gerente**
RF02, RF09
- idGerente
- nome
- emitirRelatorioInadimplencia()
- emitirRelatorioOcupacao()
- gerenciarPlanos()
- emitirRelatorios()
