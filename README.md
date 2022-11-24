<h1 align="center">
⛰️ Zenith Inova - Padrões de Commits e Branches
</h1>

<h1 align="center">
  <img src="ZenithLogo.png" width="400px" height="400px">
</h1>

<h1 align="center">
📄 Commits 
</h1>

De acordo com a documentação do **Conventional Commits**, Commits Semânticos são uma convenção simples para ser utilizada nas mensagens de commit. Essa convenção define um conjunto de regras para criar um histórico de commit explícito, o que facilita a criação de ferramentas automatizadas.

Esses commits auxiliarão a equipe da Zenith Inova a entenderem de forma facilitada quais alterações foram realizadas nos trechos de códigos que foram commitados.

Essa identificação ocorre por meio de uma palavra e emoji que identifica se aquele commit realizado se trata de uma alteração de código, atualização de pacotes, documentação, alteração de visual, teste...

## 🦄 Tipo e Descrição

O commit semântico possui os elementos estruturais abaixo (tipos), que informam a intenção do seu commit ao utilizador(a) de seu código.

- `feat`- Commits do tipo feat indicam que seu trecho de código está incluindo um **novo recurso** (se relaciona com o MINOR do versionamento semântico).

- `fix` - Commits do tipo fix indicam que seu trecho de código commitado está **solucionando um problema** (bug fix), (se relaciona com o PATCH do versionamento semântico).

- `docs` - Commits do tipo docs indicam que houveram **mudanças na documentação**, como por exemplo no Readme do seu repositório. (Não inclui alterações em código).

- `test` - Commits do tipo test são utilizados quando são realizadas **alterações em testes**, seja criando, alterando ou excluindo testes unitários. (Não inclui alterações em código)

- `build` - Commits do tipo build são utilizados quando são realizadas modificações em **arquivos de build e dependências**.

- `perf` - Commits do tipo perf servem para identificar quaisquer alterações de código que estejam relacionadas a **performance**.

- `style` - Commits do tipo style indicam que houveram alterações referentes a **formatações de código**, semicolons, trailing spaces, lint... (Não inclui alterações em código).

- `refactor` - Commits do tipo refactor referem-se a mudanças devido a **refatorações que não alterem sua funcionalidade**, como por exemplo, uma alteração no formato como é processada determinada parte da tela, mas que manteve a mesma funcionalidade, ou melhorias de performance devido a um code review. Pode ser uma atualização que não adiciona um recurso nem corrige bugs.

- `chore` - Commits do tipo chore indicam **atualizações de tarefas** de build, configurações de administrador, pacotes... como por exemplo adicionar um pacote no gitignore. (Não inclui alterações em código). Outras atualizações que não alteram os arquivos de teste ou src.

- `ci` - Commits do tipo ci indicam mudanças relacionadas a **integração contínua** (_continuous integration_). Mudanças nos scripts de configuração e arquivos de CI.

- `revert` - Commits do tipo revert revertem um commit feito anteriormente. Deve conter o Id do commit a ser revertido e a descrição da reversão.

- `init` - Commit do tipo initial é apenas o primeiro commit a ser dado no repositório, com informações de README e Licenças, por exemplo. (Não tem alterações de código)

## ☑️ Recomendações

- Adicione um título consistente com o título do conteúdo;
- Recomendamos que na primeira linha deve ter no máximo 4 palavras;
- Para descrever com detalhes, usar a descrição do commit;
- Usar um emoji no início da mensagem de commit representando sobre o commit;
- Um link precisa ser adicionado em sua forma mais autêntica, ou seja: sem encurtadores de link e links afiliados;
- Coloque a primeira letra em maiúsculo e omita o ponto no final da sentença;
- Mantenha em mente de utilizar somente letras minúsculas enquanto utilizar commits tradicionais;
- Se houver corpo do commit, deve ser limitado a 72 caracteres, e as linhas de abertura devem idealmente não ultrapassar 50 caracteres;
- Na mensagem de commit, explique o que você está fazendo e por que você está fazendo.

## 🍧 Complementos de Commits

- **Rodapé:** Geralmente uma informação sobre o revisor e numero de card de trello ou jira 
  Exemplo: Reviewed-by: Elisandro Mello Refs #133
- **Corpo** : descrições mais precisas do que está contido no commit, apresentando impactos e os motivos pelos quais foram empregadas as alterações no código, como também instruções essenciais para intervenções futuras. 
  Exemplo: see the issue for details on typos fixed.
- **Descrições**:  uma descrição sucinta da mudança
  Exemplo: correct minor typos in code

## 💈 Padrões de emojis

<table>
  <thead>
    <tr>
      <th>Tipo de commit</th>
      <th>Emojis</th>
      <th>Palavra-chave</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>Acessibilidade</td>
      <td>♿ <code>:wheelchair:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Adicionando um teste</td>
      <td>✅ <code>:white_check_mark:</code></td>
      <td><code>test</code></td>
    </tr>
    <tr>
      <td>Adicionando uma dependência</td>
      <td>➕ <code>:heavy_plus_sign:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Alterações de revisão de código</td>
      <td>👌 <code>:ok_hand:</code></td>
      <td><code>style</code></td>
    </tr>
    <tr>
      <td>Animações e transições</td>
      <td>💫 <code>:dizzy:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Bugfix</td>
      <td>🐛 <code>:bug:</code></td>
      <td><code>fix</code></td>
    </tr>
    <tr>
      <td>Comentários</td>
      <td>💡 <code>:bulb:</code></td>
      <td><code>docs</code></td>
    </tr>
    <tr>
      <td>Commit inicial</td>
      <td>🎉 <code>:tada:</code></td>
      <td><code>init</code></td>
    </tr>
    <tr>
      <td>Configuração</td>
      <td>🔧 <code>:wrench:</code></td>
      <td><code>chore</code></td>
    </tr>
    <tr>
      <td>Deploy</td>
      <td>🚀 <code>:rocket:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Documentação</td>
      <td>📚 <code>:books:</code></td>
      <td><code>docs</code></td>
    </tr>
    <tr>
      <td>Em progresso</td>
      <td>🚧 <code>:construction:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Estilização de interface</td>
      <td>💄 <code>:lipstick:</code></td>
      <td><code>feat</code></td>
    </tr>
    <tr>
      <td>Infraestrutura</td>
      <td>🧱 <code>:bricks:</code></td>
      <td><code>ci</code></td>
    </tr>
    <tr>
      <td>Lista de ideias (tasks)</td>
      <td>🔜 <code> :soon: </code></td>
      <td></td>
    </tr>
    <tr>
      <td>Mover/Renomear</td>
      <td>🚚 <code>:truck:</code></td>
      <td><code>chore</code></td>
    </tr>
    <tr>
      <td>Novo recurso</td>
      <td>✨ <code>:sparkles:</code></td>
      <td><code>feat</code></td>
    </tr>
    <tr>
      <td>Package.json em JS</td>
      <td>📦 <code>:package:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Performance</td>
      <td>⚡ <code>:zap:</code></td>
      <td><code>perf</code></td>
    </tr>
    <tr>
        <td>Refatoração</td>
        <td>♻️ <code>:recycle:</code></td>
        <td><code>refactor</code></td>
    </tr>
    <tr>
      <td>Removendo um arquivo</td>
      <td>🔥 <code>:fire:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Removendo uma dependência</td>
      <td>➖ <code>:heavy_minus_sign:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Responsividade</td>
      <td>📱 <code>:iphone:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Revertendo commit</td>
      <td>🔙 <code>:back:</code></td>
      <td><code>revert</code></td>
    </tr>
    <tr>
      <td>Revertendo mudanças</td>
      <td>💥 <code>:boom:</code></td>
      <td><code>fix</code></td>
    </tr>
    <tr>
      <td>Segurança</td>
      <td>🔒️ <code>:lock:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>SEO</td>
      <td>🔍️ <code>:mag:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Tag de versão</td>
      <td>🔖 <code>:bookmark:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Teste de aprovação</td>
      <td>✔️ <code>:heavy_check_mark:</code></td>
      <td><code>test</code></td>
    </tr>
    <tr>
      <td>Testes</td>
      <td>🧪 <code>:test_tube:</code></td>
      <td><code>test</code></td>
    </tr>
    <tr>
      <td>Texto</td>
      <td>📝 <code>:pencil:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Tipagem</td>
      <td>🏷️ <code>:label:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Tratamento de erros</td>
      <td>🥅 <code>:goal_net:</code></td>
      <td></td>
    </tr>
  </tbody>
</table>

## 💻 Exemplos

<table>
  <thead>
    <tr>
      <th>Comando git</th>
      <th>Resultado no GitHub</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>
        <code>git commit -m ":tada: Commit inicial"</code>
      </td>
      <td>🎉 Commit inicial</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":books: docs: Atualizaçao do README"</code>
      </td>
      <td>📚 docs: Atualizaçao do README</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":bug: fix: Loop infinito na linha 50"</code>
      </td>
      <td>🐛 fix: Loop infinito na linha 50</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":sparkles: feat: Pagina de login"</code>
      </td>
      <td>✨ feat: Pagina de login</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":bricks: ci: Modificaçao no Dockerfile"</code>
      </td>
      <td>🧱 ci: Modificaçao no Dockerfile</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":recycle: refactor: Passando para arrow functions"</code>
      </td>
      <td>♻️ refactor: Passando para arrow functions</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":zap: perf: Melhoria no tempo de resposta"</code>
      </td>
      <td>⚡ perf: Melhoria no tempo de resposta</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":boom: fix: Revertendo mudanças ineficientes"</code>
      </td>
      <td>💥 fix: Revertendo mudanças ineficientes</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":lipstick: feat: Estilizaçao CSS do formulario"</code>
      </td>
      <td>💄 feat: Estilizaçao CSS do formulario</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":test_tube: test: Criando novo teste"</code>
      </td>
      <td>🧪 test: Criando novo teste</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":bulb: docs: Comentários sobre a função LoremIpsum( )"</code>
      </td>
      <td>💡 docs: Comentários sobre a função LoremIpsum( )</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":back: revert: Commit 4ea7133 - Voltar para o início da landing page"</code>
      </td>
      <td>🔙 revert: Commit 4ea7133 - Voltar para o início da landing page</td>
    </tr>
  </tbody>
</table>

<h1 align="center">
🎏 Branches 
</h1>

Visando implementar um padrão mais sólido e fácil de gerenciar nossos repositórios na Zenith Inova, resolvemos adotar uma arquitetura de branching. O **Git Flow** é um modelo, uma estratégia, ou ainda, um fluxo de trabalho muito utilizado por equipes de desenvolvimento de software. Ele se destaca por auxiliar na organização do versionamento de códigos.

O objetivo do Git Flow era melhorar as organizações das branches dentro de repositórios e, desta forma, dar mais fluidez ao processo de desenvolvimento de novas funcionalidades, correções de bugs e lançamentos de versões.

O Git Flow é recomendado para projetos que utilizam versionamento semântico ou que precisam oferecer suporte a várias versões de seu software. Se o seu projeto exige entrega contínua, como normalmente ocorre em projetos, este modelo não é recomendado para esse tipo de cenário. Porque geralmente com o Git Flow são geradas branches de longa duração e branches de longa duração atrapalham a entrega contínua.

É importante ressaltar que o Git Flow são diretrizes e não regras, ou seja, você não precisa seguir 100% ao pé da letra o que ele fala, acho legal e até saudável que haja uma adaptação de acordo com a equipe de desenvolvimento. Esse modelo para organizar as nossas branches é bem legal de ser seguido para times de desenvolvimento, pois permite tanto o desenvolvimento "paralelo" de features quanto a correção de bugs críticos encontrados em produção.

## ✍️ Modelo do Git Flow

Em nosso repositório central (origin), temos duas branches que sempre existirão no ciclo de vida de nossas aplicações. 

- `master` - Será sempre nosso código-fonte que está em produção.

- `develop` - Em paralelo a master branch, teremos a branch origin/develop que sempre refletirá todas as novas funcionalidades implementadas para o próximo release. Sempre que tivermos uma versão estável em origin/develop, estamos prontos para realizar um merge em origin/master colocando uma tag com o número do release.

Enquanto as branches origin/master e origin/develop são as principais e sempre estarão presentes, nós usaremos as branches de suporte para implementar novas funcionalidades, corrigir eventuais problemas que surgirem em produção e criar novos releases. Essas branches sempre terão um tempo de vida limitado, pois iremos removê-las assim que não forem mais necessárias. As branches que podemos usar são:

- `Feature` - Branches de implementação de novas funcionalidades.

- `Release` - Branches criadas para novos releases (entregas) para produção.

- `Hotfix` - Branches criadas para correções de bugs existentes em produção.

<br>
<table>
  <thead>
    <tr>
      <th>Branch</th>
      <th>Criadas a partir de</th>
      <th>Mergidas em</th>
      <th>Convenção</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>
        <code>Feature</code>
      </td>
      <td><code>develop</code></td>
      <td><code>develop</code></td>
      <td>Qualquer nome, exceto <code>master</code>, <code>develop</code>, <code>release-*</code> ou <code>hotfix-*</code></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="4">
        Feature branches são utilizadas para desenvolvimento de novas funcionalidades para um futuro release (entrega). Feature branches geralmente não estarão disponíveis no repositório central (origin) e sim no repositório local do desenvolvedor
      </td>
    </tr>
  </tfoot>
</table>

<br>
<table>
  <thead>
    <tr>
      <th>Branch</th>
      <th>Criadas a partir de</th>
      <th>Mergidas em</th>
      <th>Convenção</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>
        <code>Release</code>
      </td>
      <td><code>develop</code></td>
      <td><code>develop</code> e <code>master</code></td>
      <td><code>release-*</code></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="4">
        Release branches serão nossas pontes entre develop e master, onde iremos corrigir os pequenos detalhes que passaram despercebidos. Essas branches serão a nossa preparação para o próximo release de produção. Para determinar o momento de criação de uma release branch, podemos adotar o seguinte parâmetro: Quando a branch develop estiver preparada para um novo release.<br><br>É proibido adicionar grandes funcionalidades nessa branch, onde só é permitido a correção de erros e pequenos ajustes. Se precisarmos adicionar novas funcionalidades, devemos criar uma feature branch e mergear em develop ao término, onde essa nova funcionalidade precisará esperar o próximo release<br><br>Quando finalizarmos todo o nosso trabalho de correções e ajustes na release branch, precisamos mergear essa branch na master (branch de produção). Como todo commit na master é um novo release por padrão, precisamos criar uma <b>tag</b> para uma futura referência em nosso histórico de versões. Uma tag nada mais é que um número de versão que facilitará nosso controle em produção. Após a criação da tag em master, precisamos mergear nossas modificações feitas na release branch em develop. Assim, teremos todas essas correções já implementadas em futuros releases
      </td>
    </tr>
  </tfoot>
</table>

<br>
<table>
  <thead>
    <tr>
      <th>Branch</th>
      <th>Criadas a partir de</th>
      <th>Mergidas em</th>
      <th>Convenção</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>
        <code>Hotfix</code>
      </td>
      <td><code>master</code></td>
      <td><code>develop</code> e <code>master</code></td>
      <td><code>hotfix-*</code></td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="4">
        Hotfix branches são bem parecidas com Release branches, pois são criadas para serem devolvidas para produção (master), porém são branches criadas sem planejamento, provenientes de bugs encontrados em produção. Basicamente, são criadas quando temos um bug severo em produção e precisa ser corrigido de imediato.<br><br>Ao término da correção do bug, precisamos mergear essas alterações na master, porém precisamos mergear essas novas correções em develop para inclusão em novos releases
      </td>
    </tr>
  </tfoot>
</table>

<br><br>
**ATENÇÃO:** Se existir uma Release Branch na hora de mergear a Hotflix Branch na master, devemos mergear essa Hotfix Branch na atual Release Branch, ao invés de develop. Como ao término do merge da Release Branch na master, temos que mergear a Release Branch em develop, develop receberá essas atualizações. Se por acaso nossa Develop Branch precisar dessas correções imediatamente, podemos mergear a Hotfix Branch diretamente em develop sem problemas.

<div align="center">
  <br/>
  <br/>
  <br/>
    <div>
      <h1>Open Source</h1>
      <sub>Copyright © 2022 - <a href="https://github.com/iuricode">iuricode</sub></a>
    </div>
    <br/>
    <p> 
      <a href="https://github.com/iuricode/padroes-de-commits/blob/main/LICENSE.md">LICENÇA</a>
    </p>
    💖
</div>
