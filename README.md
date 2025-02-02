### Date: 14.09.2024
# Ex-7: Des_Algorithm
## Aim:
To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.
## ALGORITHM:

1)AES is based on a design principle known as a substitution–permutation.</br>
2)AES does not use a Feistel network like DES, it uses variant of Rijndael.</br>
3)It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits.</br>
4)AES operates on a 4 × 4 column-major order array of bytes, termed the state</br>

## PROGRAM:
```
//String=Suri
//Hex=53757269

#include <stdio.h>
#include <stdint.h>
#include <string.h>
void simple_des_encrypt(uint64_t *block, uint64_t key);
void simple_des_decrypt(uint64_t *block, uint64_t key);

int main() {
    uint64_t block;
    uint64_t key;
    printf("16-digit Hexadecimal plaintext: ");
    scanf("%lx", &block);
    
    printf("16-digit hexadecimal key: ");
    scanf("%lx", &key);

    printf("\nOriginal Block: %016lX\n", block);
    
    simple_des_encrypt(&block, key);
    printf("Encrypted Block: %016lX\n", block);
    
    simple_des_decrypt(&block, key);
    printf("Decrypted Block: %016lX\n", block);

    return 0;
}

void simple_des_encrypt(uint64_t *block, uint64_t key) {
    *block ^= key;  
}
void simple_des_decrypt(uint64_t *block, uint64_t key) {
    *block ^= key;  
}
```

## OUTPUT:
![sd](https://github.com/user-attachments/assets/b6605328-1f97-47e6-a7d8-3b81f395e87a)


## RESULT:
Thus , to use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption is done successfully.
