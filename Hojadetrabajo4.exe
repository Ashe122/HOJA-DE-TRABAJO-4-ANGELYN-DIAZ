//Angelyn Judith Diaz Zeceña

#include <iostream>//Estas son bibliotecas que se utilizan para entrada y salida de datos
#include <cmath>// ypara realizar operaciones de matemáticas

using namespace std;

//Aqui se declaran  funciones
void imprimirResultado(double resultado); // Declaración de la función para imprimir resultados
double realizarOperacion(double num1, double num2, char operador); // Declaración de la función para realizar operaciones matemáticas

int main() {
    int cantidadOperaciones;

    //Aqui se da un mensaje de bienvenida
    cout <<"****** Bienvenida personita ******" << endl;

    // se le pide al usuario la cantidad de operaciones que se irán a realizar
    cout << "Ingresa la cantidad de operaciones que deseas realizar: ";
    cin >> cantidadOperaciones;

    // Aqui se utiliza un Bucle para realizar  las operaciones según la cantidad ingresada
    for (int i = 0; i < cantidadOperaciones; ++i) {
        double num1, num2;
        char operador;

        // Se le pide al usuario los operandos y el operador
        cout << "Ingresa el primer número: ";
        cin >> num1;
        cout << "Ingresa el operador (+, -, *, /, %): ";
        cin >> operador;
        cout << "Ingresa el segundo número: ";
        cin >> num2;

        // Aqui se llama a la función para realizar operaciones matemáticas
        double resultado = realizarOperacion(num1, num2, operador);

        // Se llama a la función para imprimir resultados
        imprimirResultado(resultado);
    }

    return 0;
}

// Aqui se realiza una implementación de la función para imprimir resultados
void imprimirResultado(double resultado) {
    cout << "El resultado es: " << resultado << endl;
}

// Implementación de la función para realizar operaciones matemáticas
double realizarOperacion(double num1, double num2, char operador) {
    switch (operador) {
        case '+':
            return num1 + num2; //Aqui se realiza una suma de numeros
        case '-':
            return num1 - num2; //Aqui se realiza la operacion de restar los numeros
        case '*':
            return num1 * num2; //Aqui se multiplican los numeros
        case '/':
            // Aqui se verifica la división por cero
            if (num2 != 0) {
                return num1 / num2;
            } else {
                cout << "Error: División por cero." << endl;
                return 0;
            }
        case '%':
            //  Se verifica la división por cero
            if (num2 != 0) {
                return fmod(num1, num2);
            } else {
                cout << "Error: División por cero." << endl;
                return 0;
            }
        default:
            cout << "Operador no válido." << endl;
            return 0;
    }
}
//finaliza el programa
