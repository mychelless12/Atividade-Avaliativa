# Atividade-Avaliativa
Valendo 2 ponto
01-Alternativa D
02a)
void main() {
  int x=1;
  int y=2;
  String c = 'oiii Mychelle';
  print (x);
  print (y);
  print (c);
}
b)void main() {
  void chamada(){
    for(int i=1;i<=10;i++){
      print(i);
    }
  }
chamada();
}
c)void main() {
int z=50;
cham(z);
}
  void cham(int x){ 
for(int i=1;i<=x;i++){
    print(i);
}
}
d)void main() {
int z=3;
cham(z);
}
  void cham(int x){ 
    int soma=0;
    for(int i=1;i<=x;i++){
    print(i);
  soma=soma+i;
}
    print(soma);
}
e)void main() {
  Cachorro c = new Cachorro("Thor", 3, 5.0);
  c.barulho();
  c.comer(); 
}

class Cachorro{
  String nome;
  int idade;
  double peso;
    Cachorro( String nome , int idade,double peso){
    this.nome=nome;
    this.idade=idade;
    this.peso=peso;
  }
  void barulho() {
    print("Auauau");
  }

  void comer() {
    print("Enche o bucho");
  }
}
#PROVA:
void main() {
  ContaBancaria c1 = new ContaBancaria(345,5432,'Mychelle',2054.67);
  c1.Saque(200);
  c1.Deposito(300);
  c1.Transferencia(100);
  
  } 
 class ContaBancaria{
   int agencia;
   int conta;
   String nome;
   double saldo;
 
   ContaBancaria(int agencia,int conta,String nome,double saldo){
     this.agencia=agencia;
     this.conta=conta;
     this.nome=nome;
     this.saldo=saldo;
   }
 
   void SaldoAtual() => print("Saldo Atual:${this.saldo}");
     
   
   
    void Saque(double dinheiro){
     
     if(saldo<dinheiro){
       print("saldo insuficiente para saque");
     }
     else{
       print("saque concluido");
       this.saldo= this.saldo - dinheiro;
       SaldoAtual();
     }
     
      
    }
   void Deposito( double dinheiro){
     this.saldo = this.saldo + dinheiro;
     SaldoAtual();
     
   }
   void Transferencia(double dinheiro){
     
     if(saldo<dinheiro){
       print("saldo insuficiente para transferencia");
     }
     else{
       print("transferencia concluida");
       this.saldo= this.saldo - dinheiro;
       SaldoAtual();
     }
     
   }
 }
 



