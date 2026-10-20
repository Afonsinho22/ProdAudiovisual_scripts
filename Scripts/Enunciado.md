# Sistema de Gestão de um Centro de Produção audiovisual

Um centro de produção audiovisual disponibiliza espaços e equipamentos para realização de sessões de fotografia, gravação de vídeo, produção de áudio e edição multimédia.

Pretende-se desenvolver um sistema que permita gerir os clientes, os espaços existentes, os equipamentos, as reservas e os serviços realizados.

Cada **cliente** possui um identificador, nome, email, telefone e número de identificação fiscal.

O centro possui vários **espaços**, como estúdios de fotografia, salas de gravação, salas de edição e estúdios de áudio. De cada espaço pretende-se guardar um identificador, nome, tipo, capacidade máxima e preço por hora.

O centro possui também vários **equipamentos**, como câmaras, objetivas, microfones, tripés e equipamentos de iluminação. Cada equipamento possui um identificador, designação, tipo, marca e estado.

Um cliente pode efetuar **várias** reservas ao longo do tempo. Cada reserva possui um identificador, data em que foi criada. data de utilização, hora de início, hora de fim e estado.

Cada reserva corresponde a um único espaço. Um espaço pode, naturalmente, estar assocuiado a várias resetvas em datas e horários diferentes.

Durante uma reserva podem também ser utilizados vários equipamentos. O mesmo equipamento pode ser utilizado em diferentes reservas. Para cada equipamento associado a uma reserva é necessário guardar a quantidade utilizada.

O centro disponibiliza ainda diferentes **serviços adicionais**, como assistência técnica, edição de vídeo, tratamento de fotografia e apoio de iluminação. Cada serviço posuui um identificador, designação e preço.

Uma reserva pode incluir vários serviços adicionais e o mesmo serviço pode ser solicitado em várias reservas. Para cada serviço incluído numa reserva pretende-se guardar a quantidade de horas contratada.

Cada reserva pode originar um ou mais **pagamentos**. De cada pagamento pretende-se guardar um identificador, data, valor e método de pagamento.

Os clientes podem utilizar o sistema para consultar espaços, verificar disponibilidade, consultar equipamentos, criar reservas, consultar as suas reservas e cancelar reservas.

Os funcionários poden consultar todas as reservas, confirmar ou rejeitar reservas, registar espaços, registar equipamentos e atualizar o estado dos equipamentos.

Quando um cliente pretende efetuar uma reserva, seleciona o espaço, a data e o horário pretendidos. O sistema verifica a disponiblidade do espaço. Caso não esteja disponível, o cliente é informado e pode escolher outro espaço ou horário.

Se o espaço estiver disponível, o cliente pode selecionar equipamentos e serviços adicionais. A reserva é então registada com o estado **pendente**.

Posteriormente, um funcionário analisa a reserva. Caso possa ser realizada, confirma-a; caso exista algum impedimento, rejeita-a.

Uma reserva confirmada pode posteriormente ser cancelada pelo cliente, desde que ainda não tenha começado. Depois da realização do serviço, a reserva passa para o estado **concluída**.