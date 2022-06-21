# Anotações para o Bootcamp
## Comandos básicos do GIT:
		. cd NomeDiretório (change directory): mudar/navegar entre diretórios
		. cd "..": voltar para diretórios anteriores
		. ls: listar pastas
		. mkdir: criar diretórios (PASTAS)
		. del: deletar apenas arquivos dentro de diretórios
		. rmdir: deletar diretórios inteiros
		. echo: joga a string/comando de volta na tela
		. mv: mover arquivos
		. git add NomeArquivo: mover arquivos e dar início ao versionamento
		. git add *: move todos os arquivos para a staged area
		. git add .
		. git commit -m + mensagem: cria a commit e introduz a respectiva mensagem
		. git init: iniciar repositórios do GIT
		. git commit: criação de commits

		
## Objetos do GIT
		. blobs: armazenam metadados dentro do GIT (armazena o sha1 do arquivo e não o nome dele)
		. trees: armazenam blobs (responsável por montar toda a estrutura de onde está determinado arquivo) e podem apontar para blobs ou para outras trees
		. commits: um commit é uma imagem do atual estado do seu repositório. Ou seja, é uma "foto" de como está cada arquivo no momento deste commit. É possível retornar para qualquer commit feito no passado

**O commit está associado a uma hash SHA-1, tal hash possui metadados como autor, data de criação, mensagem e commit pai. Todos esses metadados mais o conteúdo do arquivo formam o SHA-1 do commit, que é imutável. Ou seja, não pode ser alterado. Por isso, qualquer comando utilizado com o propósito de alterar algo relacionado ao commit, irá resultar em um novo SHA-1.**
				
				
				
## Tracked e Untracked
		. Arquivos Untracked são arquivos recém adicionados/criados e que não foram feitas basicamente nenhum tipo de alteração ("arquivos virgens")
		. Passam a se tornar Arquivos Tracked a partir de sua primeira alteração
		. Arquivo Unmodified: arquivo que não sofreu modificações
		. Arquivo Modified: arquivo unmodified que sofreu modificações (o GIT reconhece que o arquivo sofreu modificações no momento em que verifica o seu sha1 - criptografia do arquivo)
		. Arquivo Staged: após o arquivo sofrer qualquer modificação, ele se torna modified, mas quando ele está sofrendo uma série de modificações quer dizer que ele está sendo preparado para ser introduzido ao sistema, neste momento ele se torna um arquivo staged, que está sendo preparado para uma função
		. Após o Staged, o arquivo é adicionado a uma Commit e ele passa a ser novamente um arquivo Unmodified, até que sofra novamente modificações e repita o ciclo.
				
		. Servidor: Remote Repository
		. Ambiente de desenvolvimento: Working Directory - Staging Area - Local Repository
				
		. Working Directory: Corresponde aos arquivos e diretórios visíveis e alteráveis
		. Staging Area: Ao realizar qualquer alteração, seja mudança em arquivos existentes, como inclusão de novos arquivos, antes de gerar uma nova versão, você primeiramente deve adicionar tais alterações para a área de preparo
		
		