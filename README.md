# Python-Assign-Q9
import random
import string

# Open the file for writing
with open("random_strings.txt", "w") as file:
    for _ in range(100):
        length = random.randint(10, 15)
        rand_str = ''.join(random.choices(string.ascii_letters + string.digits, k=length))
        file.write(rand_str + "\n")

print("100 random strings written to 'random_strings.txt'.")

