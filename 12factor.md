# 12 Fatores a serem considerados ([12factor](https://12factor.net/pt_br/))

**I. Base de Código**
Uma base de código com rastreamento utilizando controle de revisão, muitos deploys
**II. Dependências**
Declare e isole as dependências
**III. Configurações**
Armazene as configurações no ambiente
**IV. Serviços de Apoio**
Trate os serviços de apoio, como recursos ligados
**V. Build, release, run**
Separe estritamente os builds e execute em estágios
**VI. Processos**
Execute a aplicação como um ou mais processos que não armazenam estado
**VII. Vínculo de porta**
Exporte serviços por ligação de porta
**VIII. Concorrência**
Dimensione por um modelo de processo
**IX. Descartabilidade**
Maximizar a robustez com inicialização e desligamento rápido
**X. Dev/prod semelhantes**
Mantenha o desenvolvimento, teste, produção o mais semelhante possível
**XI. Logs**
Trate logs como fluxo de eventos
**XII. Processos de Admin**
Executar tarefas de administração/gerenciamento como processos pontuais

# Pontos de atenção com relação a rede

**isso não é verdade...**
1. A rede é confiável.
2. Não há latência.
3. A largura de banda é infinita.
4. A rede é segura.
5. A topologia da rede não muda.
6. Há apenas um administrador.
7. O custo de transporte é zero.
8. A rede é homogênea.

