# sistema_bancário_desafio_dioMe
Um programa simples com funções de depósito, saque e extrato. Valida saldo, limite de saque (R$ 500) e máximo de 3 saques/dia. Feito com funções modularizadas, parâmetros posicionais/nomeados e tratamento básico de erros. Ideal para aprender lógica de programação.

Desafio proposto pela DioMe, com este projeto eu aprendi:
. Estruturação de Código
Aprendeste a dividir o programa em funções especializadas, cada uma com uma responsabilidade única:

menu() para exibir opções

depositar(), sacar() para operações bancárias

exibir_extrato() para mostrar transações

Isso torna o código mais organizado, legível e fácil de manter.

2. Manipulação de Variáveis
Como saldo, extrato e contadores (numero_saques) são atualizados e compartilhados entre funções.

Uso de retorno múltiplo em funções (tuplas) para atualizar várias variáveis de estado.

3. Controle de Fluxo
Loop principal (while True) para manter o sistema em execução até que o usuário decida sair.

Estruturas condicionais (if/elif/else) para tratar diferentes operações.

4. Validação de Dados
Verificação de valores positivos em depósitos e saques.

Regras de negócio:

Limite de saque (R$ 500 por operação).

Número máximo de saques (3 por sessão).

Saldo suficiente para saque.

5. Parâmetros em Funções
Diferença entre parâmetros posicionais e nomeados:

depositar(saldo, valor, extrato, /) → Todos os parâmetros são posicionais.

sacar(*, saldo, valor, extrato...) → Todos os parâmetros devem ser nomeados.

exibir_extrato(saldo, /, *, extrato) → Combinação de ambos.

6. Formatação de Strings
Uso de f-strings para formatar valores monetários (R$ {valor:.2f}).

textwrap.dedent() para melhorar a legibilidade do menu.

7. Experiência do Usuário
Mensagens claras para sucesso ("=== Depósito realizado! ===") e erros ("@@@ Operação falhou! @@@").

8. Boas Práticas
Separação de preocupações: Lógica bancária vs. interface do usuário.

Tratamento básico de erros: Impede operações inválidas.

Clareza no código: Nomes descritivos de variáveis e funções.

9. Lógica de Negócios
Como implementar regras de um sistema real:

Limites, contadores e validações.

Rastreamento de histórico (extrato).

10. Ponto de Entrada do Programa
Uso de if __name__ == "__main__": para garantir que o código só execute quando o arquivo for rodado diretamente (não quando importado como módulo).

Habilidades Desenvolvidas:
✅ Python básico/intermediário: Variáveis, funções, condicionais, loops.
✅ Design de software: Arquitetura simples mas eficiente.
✅ Problemas do mundo real: Como modelar regras de negócio em código.
