<h1 align="center">
  <img src="assets/ZenithLogo.png" width="400px" height="240">
</h1>

<h1 align="center">
🎏 Padrão de Branches - Zenith Inova 💜
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
