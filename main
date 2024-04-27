#include <stdio.h>
#include <stdlib.h>
#include <string.h>

typedef struct {
    char nome[50];
    int idade;
} Animal;

void definirAnimal(Animal *animal, const char *nome, int idade) {
    strcpy(animal->nome, nome);
    animal->idade = idade;
}

void obterInfoAnimal(Animal animal) {
    printf("Nome: %s\n", animal.nome);
    printf("Idade: %d anos\n", animal.idade);
}

typedef struct {
    Animal animal;
    char tipoPelagem[20];
} Mamifero;

void definirPelagem(Mamifero *mamifero, const char *tipoPelagem) {
    strcpy(mamifero->tipoPelagem, tipoPelagem);
}

void obterInfoMamifero(Mamifero mamifero) {
    obterInfoAnimal(mamifero.animal);
    printf("Tipo de pelagem: %s\n", mamifero.tipoPelagem);
}

typedef struct {
    Animal animal;
    float envergaduraAsas;
} Ave;

void definirEnvergadura(Ave *ave, float envergaduraAsas) {
    ave->envergaduraAsas = envergaduraAsas;
}

void obterInfoAve(Ave ave) {
    obterInfoAnimal(ave.animal);
    printf("Envergadura das asas: %.2f metros\n", ave.envergaduraAsas);
}

typedef struct {
    Animal animal;
    char corEscama[20];
} Peixe;

void definircorEscama(Peixe *peixe, const char *corEscama) {
    strcpy(peixe->corEscama, corEscama);
}

void obterInfoPeixe(Peixe peixe) {
    obterInfoAnimal(peixe.animal);
    printf("Cor: %s\n", peixe.corEscama);
}

int main() {
  
    Mamifero cachorro;
    printf("Digite o nome do cachorro: ");
    scanf("%s", cachorro.animal.nome);
    printf("Digite a idade do cachorro: ");
    scanf("%d", &cachorro.animal.idade);
    printf("Digite o tipo de pelagem do cachorro: ");
    scanf("%s", cachorro.tipoPelagem);
    
    Ave passaro;
    printf("Digite o nome do passaro: ");
    scanf("%s", passaro.animal.nome);
    printf("Digite a idade do passaro: ");
    scanf("%d", &passaro.animal.idade);
    printf("Digite a envergadura das asas do passaro: ");
    scanf("%f", &passaro.envergaduraAsas);
    
    Peixe peixeIn;
    printf("Nome do peixe: ");
    scanf("%s", peixeIn.animal.nome);
    printf(" Idade do peixe: ");
    scanf("%d", &peixeIn.animal.idade);
    printf("Cor     do peixe: ");
    scanf("%s", peixeIn.corEscama);

    printf("Cachorro:\n");
    obterInfoMamifero(cachorro);

    printf("\nPassaro:\n");
    obterInfoAve(passaro);

    printf("\nPeixe:\n");
    obterInfoPeixe(peixeIn);

    return 0;
}
