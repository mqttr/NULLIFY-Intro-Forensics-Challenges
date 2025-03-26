# Flag
hsctf{3337894711750905}

# Guide
1. Continuing From Part 1: You should find the decoded tones being (with arbitrary separations): 6337 8947 1175 0905
2. Based on what the user said in the start of the audio clip, we can infer that this code is related to money, hopefully it is a small leap to assume a credit card number
3. Credit card numbers follow a simple checksum algorithm called "Luhn Algorithm", and as such, this allows us to somewhat correct the inputted value given some more information
4. According to the voice recording, the first value is incorrect
5. We find a website (like https://www.dcode.fr/luhn-algorithm) to help us check multiple possible first values
6. After some trial and error we identify that the credit card number only follows the Luhn Number Checksum when the first value is **3**
7. Replacing the first value (6) with 3 gives us the flag
