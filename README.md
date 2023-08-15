### Instruções para iniciar o projeto:

- 1- Criar um projeto JAVA chamado ProjetoNext2023.
- 2- Descompactar o arquivo projetomodelo.zip em uma pasta do sistema de arquivos.
- 3- Localizar, na pasta onde o zip foi descompactado, o diretório SRC.
- 4- Selecionar tal diretório e copiar (CTRL-C).
- 5- Na IDE, selecionar o projeto criado ProjetoNext2023.
- 6- Colar (CTRL-V) o diretório SRC copiado.
- 7- Os passos 3-6 correspondem a uma forma simplificada de colocar as classes de referência em um projeto. Existem outros caminhos, que vão igualmente resultar na estrutura de pacotes e nas classes dentro de um projeto JAVA típico.
- 8- Baixar no diretório do projeto o arquivo PersistenciaObjetos.jar.
- 9- Incluir no projeto a dependência de PersistenciaObjetos.jar. No Eclipse, seguir os seguintes passos:
- a. Selecionar o projeto, clicar no botão direito, que dá acesso ao menu de contexto.
- b. Clicar na opção Properties.
- c. Abre-se uma janela com algumas opções. Clicar em Java Build Path e selecionar a aba Libraries.
- d. No espaço “JARs and class folders on the build path”, selecionar Classpath.
- e. No lado esquerdo, clicar em Add External JARs...
- f. Abre-se uma janela para seleção de arquivos. Selecionar o arquivo PersistenciaObjetos.jar.


# Java Project - Curso Next2023
<div align="center">
   <a href="https://www.cesar.org.br" target="_blank" rel="noreferrer">
      <img  alt="Cesar" height="400px" style="padding-right:10px;" src="https://www.cesar.org.br/image/layout_set_logo?img_id=1086110&t=1683038460804" />
  </a>
</div>

<div align="center"> 
  
![](https://cdn.icon-icons.com/icons2/2699/PNG/512/java_logo_icon_168609.png)

</div>



1. **Classe ContaCorrente, que implementa a interface Serializable**
2. Atributos: número (String), saldo (double), nome do correntista (String)
3. Métodos:
4. Construtor padrão e construtor com todos os atributos.
5. Get para todos os atributos.
6. Set para todos os atributos menos o saldo.
7. void creditar(double valor): saldo = saldo + valor
8. void debitar(double valor): saldo = saldo - valor
9. **Classe ContaPoupanca, que herda de ContaCorrente**
10. Atributos: percentual de bônus (double).
11. Métodos:
12. Construtor padrão e construtor com todos os atributos.
13. Get para todos os atributos.
14. Set para todos os atributos.
15.  @ Override
16. void creditar(double valor): saldo = saldo + valor *(1 + percentual de bônus / 100)
17. **Classe DAOContaCorrente**
18. Atributos: cadastro, do tipo CadastroObjeto.
19. O identificador único de uma conta corrente e de uma conta poupança é o seu número.
20. Métodos:
21. boolean incluir(ContaCorrente conta)
22. boolean alterar(ContaCorrente conta)
23. ContaCorrente buscar(String numero)
24. LIst<ContaCorrente> buscarTodos()
25. Implementar os métodos segundo o código do DAOProduto.

![](https://i.postimg.cc/fyPXmfsL/Diagrama-Conta-Corrente.png)

