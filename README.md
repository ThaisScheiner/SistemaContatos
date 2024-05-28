# Sistema de Cadastro de Contatos Virtual, com C# com ASP.NET MVC + SQLServer

## Projeto de um sistema realizado através de estudo de um curso para Criação de um sistema de contatos 
Usei validação de campos, para que nao possam ser gravados em branco,
nas senhas usei configurações de criptografia, para que no banco a senha do usuário seje preservada,
configurei para que se o usuário esquecer a senha de login, a senha seja enviada para o email, para recuperar a senha,
o usuário também pode alterar a senha,
criei 2 tipos de perfil de usuario, o administrador, onde ele tem acesso total ao sistema e
o usuário padrão que tem acesso restrito ao sistema.
Conectei os dados com o Banco de Dados SQL Server e usei o Entity framework para a comunicação.

## 
Código para funcionar a paginação e a tradução dos componentes de busca

<pre>
  
    $('#table-contatos').DataTable({
        "ordering": true,
        "paging": true,
        "searching": true,
        "oLanguage": {
            "sEmptyTable": "Nenhum registro encontrado na tabela",
            "sInfo": "Mostrar _START_ at&eacute; _END_ de _TOTAL_ registros",
            "sInfoEmpty": "Mostrar 0 at&eacute; 0 de 0 Registros",
            "sInfoFiltered": "(Filtrar de _MAX_ total registros)",
            "sInfoPostFix": "",
            "sInfoThousands": ".",
            "sLengthMenu": "Mostrar _MENU_ registros por pagina",
            "sLoadingRecords": "Carregando...",
            "sProcessing": "Processando...",
            "sZeroRecords": "Nenhum registro encontrado",
            "sSearch": "Pesquisar",
            "oPaginate": {
                "sNext": "Proximo",
                "sPrevious": "Anterior",
                "sFirst": "Primeiro",
                "sLast": "Ultimo"
            },
            "oAria": {
                "sSortAscending": ": Ordenar colunas de forma ascendente",
                "sSortDescending": ": Ordenar colunas de forma descendente"
            }
        }
    });
  
</pre>
