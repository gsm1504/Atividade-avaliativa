# Atividade-avaliativa

# questão 1
Letra D

# questão 2
# letra a)

void main() {
int a = 10;
int b = 20;
String nome = 'Gabriel';
  
print(a);
print(b);
print(nome);
}

# letra b)

void funcao(){
    for(int i = 1; i <=10; i++)
      print(i);
}

void main() {
funcao();
  
}

# letra c)

void funcao(int a){
    for(int i = 1; i <=a; i++)
      print(i);
}

void main() {
funcao(50);
  
}

# letra d)

funcao(int a){
  int contador = 0;
    for(int i = 1; i <=a; i++){
      contador = contador + i;
    }
  print(contador);
}

void main() {
funcao(5);
  
}

# letra e)

void main() {
  cachorro pitbull = cachorro('bob','pitbull','gabriel');
  cachorro pincher = cachorro('fera','pincher','jubileu');
  
  pitbull.latir();
  pincher.latir();
  
  pitbull.apresentacao('bob','pitbull','gabriel');
  pincher.apresentacao('fera','pincher','jubileu');
}

class cachorro{
  String nome;
  String raca;
  String nome_do_dono;
  
  cachorro(String nome,String raca,String nome_do_dono ){
    this.nome = nome;
    this.raca = raca;
    this.nome_do_dono = nome_do_dono;
  }
    
    void latir(){
      print('au au');
    }
  
    void apresentacao(String a, String b, String c){
      print( 'O nome do cachorro é $a e é da raça $b e pertence a $c');
    }
}

# Avaliação qualitativa(valendo 4 pontos)

void main(){
  Criar conta = Criar(123456789,"Gabriel",1000,nome_da_mae:"Bianca");
  void iniciacao(){
    print("Olá cliente");
  }
  
  iniciacao();
  conta.saldotemp();
  
  conta.deposito(500);
  conta.saldotemp();
  
  conta.saque(750);
  conta.saldotemp();
  
  conta.saque(800);
  
    
}

class Criar{
  int n_conta;
  String nome;
  double saldo;
  
  Criar(int a, String b,double c, {String nome_da_mae}){
    this.n_conta = a;
    this.nome=b;
    this.saldo=c;
  }
  
   void saldotemp(){
    print("O saldo atual é : ${this.saldo}");
  }
  
    voidtranferencia(double valor_transferido, int num_conta, int num_receptor){
    this.saldo = this.saldo - valor_transferido;
  }
  
  void deposito(double valor_depositado) => (this.saldo = this.saldo + valor_depositado);
  
 
  
 void saque(int valor_saque){
   if(valor_saque>this.saldo){
     print("Saque inválido");
   }
   else{
    this.saldo = this.saldo -valor_saque;
   }
  }
}

