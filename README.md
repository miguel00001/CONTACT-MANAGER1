# CONTACT-MANAGE
listadecontatos=[]

def recebe_dados_contato():
    telefone=input("digite seu telefone")
    nome=input("digite seu nome")
    criarcontato(telefone,nome)

def criarcontato(telefone,nome):
    dicionario_contato=(telefone,nome)
    listadecontatos(dicionario_contato)
    print("numero adicionado com sucesso")


def removercontato():
   nome=("digite o nome do contato a ser removido")
   for contato in listadecontatos:
      if contato["nome"] ==nome:
         listadecontatos.remove(listadecontatos)
         print("contato excluyido com sucesso")
         return
      print("contato não existente")


def buscarcontatopelonome():
   nome=imput("digite o nome do coontato desejado")
   for  contato in listadecontatos:
      if contato ["nome"] == nome:
         print("contato encontrado")
         print(listadecontatos)
         return
      else:
         print("contato não existente")
         return
import projetosamara

def exibirmenu():
    print("bem-vindo")
    print("1.criar contato")
    print("2.remover contato")
    print("3.buscar contato")
    print("4.sair do sistema")

def opcao_1():
    print("criar contato")
    projetosamara.recebe_dados_contato()


def opcao_2():
    print("remover contato") 
    projetosamara.removercontato()


def opcao_3():
    print("buscar contato")
    projetosamara.buscarcontatopelonome


while True:
    exibirmenu()
    escolha = input("digite o numero da opção desejada:")

    if escolha == "1":
        opcao_1()

    elif escolha == "2":
        opcao_2()

    elif escolha == "3":
        opcao_3

    elif escolha == "4" :
        print("sair")       
        
