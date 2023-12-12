# INTRODUÇÃO

Git se trata de um software de versionamento distribuído, no sentido de que vários computadores podem acessar um repositório simultaneamente, de forma que o git irá controlar alterações, exclusões, etc...
O Github, por sua vez, é um servidor que hospeda uma aplicação git, facilitando, assim, a comunicação entre usuários de diversos locais do mundo.

## PRINCIPAIS COMANDOS

<html>
  <table>
    <thead>
      <tr>
        <th>Nome do comando</th>
        <th>Tokens</th>
        <th>Parâmetros</th>
        <th>Descrição</th>
      </tr>
    </thead>
    <tbody align="center">
      <tr>
        <td rowspan="9">config</td>
        <td></td>
        <td></td>
        <td>Exibe todos os tokens do comando "config".</td>
      </tr>
    <tr>
      <td rowspan="5">--global</td>
      <td></td>
      <td>Diz respeito aos parâmetros globais (de usuário).</td>
    </tr>
    <tr>
      <td>user.name ["nome"]</td>
      <td>Exibe o nome de usuário. Se preencher "nome" , configura este par&acirc;metro.</td>
    </tr>
    <tr>
      <td>user.email [nome_email]</td>
      <td>Exibe o email do usuário. Se preencher email, configura este parâmetro.</td>
    </tr>
    <tr>
      <td>init.defaultBranch [nome]</td>
      <td>Exibe o nome do branch padrão. Se preencher nome, configura este parâmetro.</td>
    </tr>
    <tr>
      <td>credential.helper [cache, store]</td>
      <td>Exibe a forma de salvamento das credenciais, se "cache" ou "store". Se quiser configurar, chamar antes da autenticação, e completar com a opção "cache", para guardar temporariamente, ou "store", para guardar permanentemente. </td>
    </tr>
    <tr>
      <td>--system</td>
      <td></td>
      <td>Diz respeito aos parâmetros de sistema (OS, ... ).</td>
    </tr>
    <tr>
      <td>--local</td>
      <td></td>
      <td>Diz respeito aos parâmetros locais (de reposit&oacute;rio).</td>
    </tr>
    <tr>
      <td>[--global, --system, --local] --list [--show-origin]</td>
      <td></td>
      <td>Lista as variáveis gravadas. Se fornecer o escopo (global, system, ou local), lista as variáveis deste escopo. Se --show-origin estiver presente, exibe o caminho em que a variável está guardada.</td>
    </tr>
    <tr>
      <td>clone</td>
      <td></td>
      <td>repo_url [repo-nome] [--branch nome_branch --single-branch]</td>
      <td>Clona o repositório de link "repo_url" para a pasta na qual o comando foi chamado. Use "repo-nome" para renomear localmente a pasta do repositório. Se a opção "--branch nome-branch --single-branch" estiver presente, clona apenas o branch "nome-branch".</td>
    </tr>
    <tr>
      <td rowspan=2>remote</td>
      <td>-v</td>
      <td></td>
      <td>Lista os repositórios remotos ao qual o git está conectado.</td>
    </tr>
    <tr>
      <td>add origin</td>
      <td>repo_url</td>
      <td>Faz o link entre um repositório criado localmente e um repositório do github acessado por "repo_url".</td>
    </tr>
    </tbody>
</table>
</html>

## COMANDOS ÚTEIS NO PROMPT

|Comando|Descrição|
| :---: | :---: |
|```cd "path"```| acessa o diretório especificado por "path"|
|```cd ..```| acessa o diretório pai|
|```mkdir```| cria diretório no caminho ativo|
|```ls [-a]```|Lista arquivos e subdiretórios; se o opcional "-a" estiver presente, exibe todos os itens, inclusive os ocultos|
|```ls -a ~/.ssh```|Chamado na raiz. Lista arquivos de configuração de ssh. Se não existir, não há chaves ssh configuradas.|
