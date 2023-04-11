# Padrões de Commits

Documentação: [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)

De acordo com a documentação do Conventional Commits, **Commits Semânticos** são uma convenção simples que deve ser utilizada nas mensagens de commit. Essa convenção estabelece um conjunto de regras para criar um histórico de commits explícito, o que torna mais fácil a criação de ferramentas automatizadas.

Esses commits ajudarão você e sua equipe a entender de maneira mais simples quais alterações foram realizadas no trecho de código que foi commitado. A identificação das alterações ocorre por meio de uma palavra e um emoji que identificam se aquele commit se trata de uma alteração de código, atualização de pacotes, documentação, mudança visual, teste, entre outros.

Observação: É importante observar que o uso de emoji é opcional na convenção de Commits Semânticos. Embora seja uma prática comum, é possível aderir à convenção sem utilizar emojis nas mensagens de commit.

## 💬 Tipo e Descrição

A convenção de Commits Semânticos utiliza uma série de palavras-chave para descrever os tipos de alterações que foram realizadas no código. Esses tipos ajudam a identificar com clareza o propósito de cada commit. Segue abaixo a descrição de alguns tipos de commits:

- **`feat`**: Commits desse tipo indicam que um **novo recurso** foi adicionado ao código (relacionado ao MINOR do versionamento semântico).
- **`fix`**: Commits desse tipo indicam que um **problema foi solucionado** no código (bug fix), (relacionado ao PATCH do versionamento semântico).
- **`docs`**: Commits desse tipo indicam que houve **mudanças na documentação**, como no arquivo README do repositório. Esses commits não incluem alterações no código.
- **`test`**: Commits desse tipo são utilizados quando são realizadas **alterações em testes**, seja criando, alterando ou excluindo testes unitários. Esses commits não incluem alterações no código.
- **`build`**: Commits desse tipo indicam modificações realizadas em **arquivos de build e dependências**.
- **`perf`**: Commits desse tipo são utilizados para identificar alterações de código que tenham impacto em **performance**.
- **`style`**: Commits desse tipo indicam que houveram **alterações de formatação** no código, como no uso de semicolons, trailing spaces, entre outros. Esses commits não incluem alterações no código.
- **`refactor`**: Commits desse tipo referem-se a mudanças realizadas devido a **refatorações que não alterem a funcionalidade** do código, como melhorias de performance ou alterações em como determinada parte da tela é processada.
- **`chore`**: Commits desse tipo indicam **atualizações de tarefas** de build, configurações de administrador, pacotes, entre outros. Esses commits não incluem alterações no código.
- **`ci`**: Commits desse tipo indicam mudanças relacionadas à **integração contínua** (*continuous integration*).

É importante lembrar que essas palavras-chave são apenas sugestões, e que é possível criar outras palavras-chave de acordo com as necessidades do projeto. Além disso, o uso dessas palavras-chave é opcional, mas pode ajudar a criar um histórico de commit mais claro e consistente.

## 🎯 **Porque utilizar Conventional Commits**

- Criação automatizada de CHANGELOGs.
- Determinar automaticamente alterações no versionamento semântico (com base nos tipos de commits).
- Comunicar a natureza das mudanças para colegas de equipe, o público e outras partes interessadas.
- Disparar processos de build e deploy.
- Facilitar a contribuição de outras pessoas em seus projetos, permitindo que eles explorem um histórico de commits melhor estruturado.

## 🏅 Recomendações

- Adicione um título consistente com o título do conteúdo;
- Recomendamos que na primeira linha deve ter no máximo 4 palavras;
- Para descrever com detalhes, usar a descrição do commit;
- Usar um emoji no início da mensagem de commit representando sobre o commit;
- Um link precisa ser adicionado em sua forma mais autêntica, ou seja: sem encurtadores de link e links afiliados;

## 🍧 Complementos de Commits

- **Rodapé:** Geralmente uma informação sobre o revisor e numero de card de trello ou jira
Exemplo: Reviewed-by: Elisandro Mello Refs #133
- **Corpo** : descrições mais precisas do que está contido no commit, apresentando impactos e os motivos pelos quais foram empregadas as alterações no código, como também instruções essenciais para intervenções futuras.
Exemplo: see the issue for details on typos fixed.
- **Descrições**: uma descrição sucinta da mudança
Exemplo: correct minor typos in code

## 📌 **Padrões de emojis**

| Tipo de Commit | Emojis | Palavra-Chave |
| --- | --- | --- |
| Acessibilidade | ♿ `:wheelchair:` |  |
| Adicionando um teste | ✅ `:white_check_mark:` | test |
| Adicionando uma dependência | ➕ `:heavy_plus_sign:` | build |
| Alterações de revisão de código | 👌🏾 `:ok_hand:` | style |
| Animações e transições | 💫 `:dizzy:` |  |
| Bugfix | 🐛 `:bug:` | fix |
| Comentários | 💡 `:bulb:` | docs |
| Commit inicial | 🎉 `:tada:` | init |
| Configuração | 🔧 `:wrench:` | chore |
| Deploy | 🚀 `:rocket:`  |  |
| Documentação | 📚 `:books:` | docs |
| Em progresso | 🚧 `:construction:` |  |
| Estilização de interface | 💄 `:lipstick:` | feat |
| Infraestrutura | 🧱 `:bricks:` | ci |
| Lista de ideias (tasks) | 🔜 `:soon:` |  |
| Mover/Renomear | 🚛 `:truck:` | chore |
| Novo recurso | ✨ `:sparkles:` | feat |
| Package.json em JS | 📦 `:package:` | build |
| Performance | ⚡ `:zap:` | perf |
| Refatoração | ♻️ `:recycle:` | refactor |
| Removendo um arquivo | 🔥 `:fire:` |  |
| Removendo uma dependência | ➖ `:heavy_minus_sign:` | build |
| Responsividade | 📱 `:iphone:` |  |
| Revertendo mudanças | 💥 `:boom:` | fix |
| Segurança | 🔒 `:lock:` |  |
| SEO | 🔍 `:mag:`  |  |
| Tag de versão | 📑 `:bookmark:` |  |
| Teste de aprovação | ✅ `:heavy_check_mark:` | test |
| Testes | 🧪 `:test_tube:` | test |
| Texto | ✏️ `:pencil:` |  |
| Tipagem | 🏷️ `:label:` |  |
| Tratamento de erros | 🥅 `:goal_net:` |  |

## **🔆 Exemplos**

| Comando Git | Resultado |
| --- | --- |
| git commit -m ":tada: Initial commit" | 🎉 Initial commit |
| git commit -m ":books: docs: Update README" | 📚 Update README documentation |
| git commit -m ":bug: fix: Fix infinite loop on line 50" | 🐛 Fix infinite loop on line 50 |
| git commit -m ":sparkles: feat: Add login page" | ✨ Add login page feature |
| git commit -m ":bricks: ci: Modify Dockerfile" | 🧱 Modify Dockerfile for CI |
| git commit -m ":recycle: refactor: Refactor to arrow functions" | ♻️ Refactor to arrow functions |
| git commit -m ":zap: perf: Improve response time" | ⚡ Improve performance and response time |
| git commit -m ":boom: fix: Revert inefficient changes" | 💥 Revert inefficient changes |
| git commit -m ":lipstick: feat: Style form with CSS" | 💄 Add feature to style form with CSS |
| git commit -m ":test_tube: test: Create new test" | 🧪 Create new test |
| git commit -m ":bulb: docs: Add comments to LoremIpsum( ) function" | 💡 Add comments to LoremIpsum( ) function documentation |
