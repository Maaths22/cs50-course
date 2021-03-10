#include <stdio.h>
#include <cs50.h>
#include <string.h>
#include <ctype.h>
#include <stdlib.h>

bool check_key(string s);

int main(int argc, string argv[]){

    if(argc != 2 || !check_key(argv[1])){

        printf("Usage: ./caesar key\n");

        return 1;
    }

    int key = atoi(argv[1]);

    string plaintext = get_string("plaintext: ");

    printf("ciphertext: ");

    int cypher_alpha, letter_ascii;

    for(int i = 0, n = strlen(plaintext); i < n ; i++){

        char c = plaintext[i];

        if(isalpha(c)){

            if(islower(c)){
                cypher_alpha = 0;
                letter_ascii = (int) c;

                cypher_alpha = letter_ascii + key;

                if(letter_ascii + key <= 122){
                    printf("%c", cypher_alpha);
                }else{
                    
                    do{
                            cypher_alpha -= 26;

                    }while(cypher_alpha > 122);
                    
                    printf("%c", cypher_alpha);
                }
            }else{
                cypher_alpha = 0;
                letter_ascii = (int) c;

                cypher_alpha = letter_ascii + key;

                if(letter_ascii + key <= 90){
                    printf("%c", cypher_alpha);
                }else{
                    
                    do{
                            cypher_alpha -= 26;

                    }while(cypher_alpha > 90);
                    
                    printf("%c", cypher_alpha);
                }
            }

        }else{ 
            printf("%c", c);
        }
        
    }   printf("\n");

    return 0;
}

bool check_key(string s){

    for(int i=0, len = strlen(s); i < len; i++)
        if(!isdigit(s[i]))
            return false;

    return true;
}
