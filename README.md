# Calculadora-Inversa
Calculadora Inversa: Escolha primeiro a operação e depois os números a serem usados na conta

#include <iostream>

int sub;
int mult;
int divs;
int soma;

using namespace std;
int main() {
  int x;
  int y;
  int z;

  cout << "qual o calculo que desaja fazer?";
  cout << " 1(soma)"; 
  cout << "2(subtração)"; 
  cout << "3(multiplicação)"; 
  cout << "4(divisão)";
  cin >> y;
  
  if (y > 4){
  cout << "ERRO: Não foi encontrada a sua operação ";
    return 0;
  } else if(y < 1){
  cout << "ERRO: Não foi encontrada a sua operação ";
    return 0;
  }

  cout <<"digite o primeiro numero"; 
  cin >> x;

  cout <<"digite o segundo numero" ;
  cin >> z;

  switch(y) {
    case 1: soma = (x + z);
    cout << "o resultado da soma é: " << soma;
    break;
    case 2: sub = x - z;
    cout << "o resultado da subtração é: " << sub;
    break;
    cout << "o resultado da subtração é: " << sub;
    case 3: mult = x * z;
    cout << "o resultado da multiplicação é: " << mult;
    break;
    case 4: divs = x / z;
    cout << "o resultado da divisão é: " << divs;
    break;

  } 
  return 0;
}
