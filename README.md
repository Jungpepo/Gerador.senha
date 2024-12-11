import string as st
import random

# Caracteres para a senha
letras = st.ascii_letters  # Letras maiúsculas e minúsculas
numeros = st.digits        # Números
especial = st.punctuation  # Caracteres especiais

# Combinação de todos os caracteres
algarismos = letras + numeros + especial

# Gerando uma senha de 10 caracteres
senha = ''.join(random.choice(algarismos) for _ in range(10))

# Exibindo a senha
print(senha)
