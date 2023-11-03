# Requisitos e Regras de Negócio

## Regras de Negócio

| Indicador | Descrição | Atividades Relacionadas |
| --- | --- | --- |
| RN01 | A "Jardineira" funciona de segunda a sexta-feira, das 7h às 21h55. | - |
| RN02 | A "Jardineira" tem capacidade para transportar de 30 a 40 pessoas por viagem. | - |
| RN03 | A "Jardineira" segue um trajeto pré-definido entre o campus e a estação de metrô Virgílio Távora. | - |
| RN04 | Os usuários devem se cadastrar no sistema com um e-mail válido e uma senha com no mínimo 6 caracteres. | - |
| RN05 | Os usuários devem confirmar o seu cadastro no sistema por meio de um link enviado para o seu e-mail. | - |
| RN06 | Os usuários podem escolher receber notificações push pelo celular, mas devem aceitar as permissões necessárias. | - |
| RN07 | O sistema deve armazenar os seguintes dados pré-definidos que definem o horário das viagens e valem para um dia inteiro: percurso, quantidade de viagens, início das viagens e término das viagens. | - |
| RN08 | A quantidade de viagens deve ser um número inteiro maior ou igual a zero que indique quantas vezes o veículo completou o percurso no dia. | - |
| RN09 | O percurso deve ser uma string que identifica o nome do trajeto seguido pelo veículo, indicando o seu sentido. | - |
| RN10 | O início das viagens e o término das viagens devem ser datas e horas no formato DD/MM/AAAA HH:MM que indiquem quando o veículo iniciou e terminou cada viagem no dia. | - |
| RN11 | O sistema deve validar os dados registrados e armazenados, verificando se eles estão de acordo com os formatos, as unidades e as regras de negócio definidas. Caso contrário, o sistema deve informar o erro e solicitar a correção dos dados. | - |

## Requisitos Funcionais

| Indicador | Descrição | Atividades Relacionadas |
| --- | --- | --- |
| RF01 | O sistema deve permitir que os usuários visualizem o mapa com o trajeto do veículo e a sua posição atual. | Criação da tela de mapa, integração com a API do Google Maps e Directions |
| RF02 | O sistema deve atualizar a posição do veículo em tempo real, em curtos períodos de tempo, usando os dados fornecidos pela API externa. | Integração com a API externa |
| RF03 | O sistema deve mostrar as informações adicionais do veículo, como previsão de chegada. | Criação da tela de informações do veículo |
| RF04 | O sistema deve permitir que os usuários se cadastrem e façam login no sistema, usando um e-mail e uma senha válidos. | Criação da tela de login, validação de e-mail e senha, autenticação com Google ou GitHub |
| RF05 | O sistema deve permitir que os usuários recebam notificações push pelo celular quando o veículo estiver próximo ao seu ponto de embarque ou desembarque. | Criação da tela de notificações push, envio de notificações push |
| RF06 | O sistema deve permitir que os administradores do sistema tenham acesso aos dados de relatórios das viagens e da performance do veículo, como: velocidade média, número de viagens e quilometragem percorrida no mês. | Criação da tela de relatórios, geração de relatórios |

## Requisitos Não Funcionais

| Indicador | Descrição | Atividades Relacionadas |
| --- | --- | --- |
| RNF01 | O sistema deve ser responsivo, adaptando-se ao tamanho da tela do dispositivo usado pelo usuário. | Desenvolvimento do sistema para ser responsivo |
| RNF02 | O sistema deve ser seguro, protegendo os dados dos usuários e do veículo contra acessos não autorizados. | Implementação de medidas de segurança, como criptografia e autenticação |
| RNF03 | O sistema deve ser confiável, garantindo a disponibilidade e a consistência das informações. | - |
| RNF04 | O sistema deve ser fácil de usar, oferecendo uma interface intuitiva e amigável aos usuários. | - |
| RNF05 | O sistema deve ser escalável, podendo suportar um aumento na demanda de usuários, dados e funcionalidades. | Implementação de uma arquitetura escalável |
| RNF06 | O sistema embarcado requer conexão com a internet, seja móvel ou Wi-Fi, para funcionar corretamente, utilizando o módulo GPS Neo-6Mv2 e o Sensor Acelerômetro e Giroscópio MPU-6050. | - |
