# Gestão Integrada

Sistema web de gestão de colaboradores e controle financeiro, desenvolvido com HTML, CSS e JavaScript, integrado ao Supabase para autenticação, armazenamento e gerenciamento seguro dos dados.

# Módulos

## Colaboradores

* Cadastro e edição de nome, cargo, projeto/setor, salário e status.
* Acompanhamento da folha prevista e dos valores pagos por competência.
* Registro de pagamentos parciais ou integrais, com data e observações.
* Histórico financeiro preservado mesmo após a exclusão de um cadastro.
* Integração automática entre pagamentos e movimentações financeiras.

## Financeiro

* Registro de receitas e despesas, com categoria, data e observação.
* Painel mensal com saldo, entradas, saídas e folha de pagamento.
* Busca e filtros por tipo e categoria.
* Edição e exclusão de movimentações manuais.
* Exportação de movimentações em CSV.
* Backup e restauração de dados por arquivos JSON.

# Integração entre módulos

O pagamento de um colaborador gera automaticamente uma despesa na categoria Salários, vinculada ao respectivo cadastro.

O sistema permite pagamentos parciais ou integrais, acumulando os valores pagos durante cada competência e mantendo o histórico financeiro correspondente.

# Autenticação e segurança

* Autenticação de usuários integrada ao Supabase Auth.
* Acesso ao sistema mediante credenciais autorizadas.
* Banco de dados remoto com PostgreSQL.
* Políticas de segurança RLS (Row Level Security).
* Isolamento dos dados por grupo, impedindo que usuários de um grupo acessem informações financeiras de outro.
* Gerenciamento de sessões e encerramento de acesso.
* Regras de acesso aplicadas diretamente no banco de dados.

# Banco de dados e armazenamento

O sistema utiliza o Supabase como infraestrutura de banco de dados e autenticação.

Os registros de colaboradores e movimentações financeiras são armazenados remotamente, permitindo que as informações sejam acessadas em diferentes dispositivos mediante autenticação.

Também são disponibilizados recursos de exportação e restauração manual por arquivos JSON, facilitando a transferência e a recuperação de informações.

# Tecnologias utilizadas

* HTML5: estrutura da aplicação.
* CSS3: identidade visual e responsividade.
* JavaScript: funcionalidades e integração entre módulos.
* Supabase Auth: autenticação e gerenciamento de usuários.
* PostgreSQL: armazenamento e gerenciamento dos dados.
* Row Level Security (RLS): controle de acesso e isolamento de informações.
* GitHub: versionamento e gerenciamento do código-fonte.

## Publicação

Aplicação web desenvolvida para execução em navegadores modernos, com possibilidade de publicação por meio de hospedagem de arquivos estáticos.

A conexão com o Supabase permite que a aplicação utilize autenticação e banco de dados remoto sem depender exclusivamente do armazenamento local do navegador.

Comercialização e modelo de assinatura

A Gestão Integrada possui uma estrutura de autenticação, banco de dados remoto e separação de informações por grupo.

# Auxílio de Inteligência Artificial

Diferentes modelos e ferramentas de Inteligência Artificial foram utilizados como apoio durante o desenvolvimento, cada um contribuindo para etapas específicas do projeto.

* Claude Code: auxílio na análise do código, correção de bugs, identificação de problemas e ajustes de sintaxe.
* ChatGPT: apoio na concepção, organização e aprimoramento do layout e da experiência de utilização.
* Gemini: estudos e análises de sites existentes, utilizados como referências e inspiração para decisões de design e funcionalidades.
