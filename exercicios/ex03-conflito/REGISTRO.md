Eu fiz 2 vezes esse conflito. Na primeira vez eu terminei o conflito e apenas tinha registro de uma das minhas 2 branches que tinham conflitado, então achei melhor refazer para evitar problema.

O conflito ocorreu no arquivo exercicios/ex03-conflito/CONFLITO.md.
A causa foi a divergência entre as branches feat/conflito-lado-a e feat/conflito-lado-b. Ambas foram criadas a partir do mesmo commit da main, mas alteraram a mesma linha (Linha 1) com conteúdos diferentes:

Branch A: Linha 1: Versão modificada pela Branch A (Lógica de Monitoria)
Branch B: Linha 1: Versão modificada pela Branch B (Validação de Dados)

Como a main já havia incorporado a Branch B, ao tentar realizar o merge da Branch A, o Git identificou que a mesma linha possuía duas instruções conflitantes e não soube qual manter automaticamente.

Como decidi qual versão manter?
Para fins de portfólio e para garantir que o trabalho de ambas as "frentes de desenvolvimento" fosse preservado, utilizei a opção "Accept Both Changes" (Aceitar ambas as alterações) no VS Code.

Dessa forma, o arquivo final ficou com as duas mensagens, uma em cada linha, representando a integração das funcionalidades.

Comandos e ações usadas:

1. Identificação do conflito via terminal após o comando git merge feat/conflito-lado-a.
2. VS Code para resolução manual através da interface gráfica.
3. Execução do comando git add exercicios/ex03-conflito/CONFLITO.md para marcar o conflito como resolvido.
4. Finalização com git commit para gerar o commit de merge.
