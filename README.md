erDiagram
    Voo ||--o{ Assento : Tem
    Passageiro }|o--o{ Reserva : Realiza
    Passageiro }|o--o{ Dependente : Tem
    Reserva {
        data_da_reserva (Chave Primária)
        hora_da_reserva
    }
    Voo {
        identificacao_do_voo (Chave Primária)
        numero_do_aviao
        cidade_de_origem
        cidade_de_destino
        data_do_voo
        hora_do_voo
    }
    Assento {
        identificacao_do_assento (Chave Primária)
        quantidade
    }
    Passageiro {
        CPF (Chave Primária)
        nome
        telefone
        email
        endereco (rua, numero, complemento, bairro, CEP, cidade, estado)
    }
    Dependente {
        nome
        data_de_nascimento
    }
