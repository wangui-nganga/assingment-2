# assingment-2
# Python program to display the Fibonacci sequence
def recur_fibo(n):
   if n <= 1:
       return n
   else:
       return(recur_fibo(n-1) + recur_fibo(n-2))
nterms = 50
# check if the number of terms is valid
if nterms <= 0:
   print("Plese enter a positive integer")
else:
   print("Fibonacci sequence:")
   for i in range(nterms):
       print(recur_fibo(i))
       
# Python Program to find Volume and Surface Area of Sphere

PI = 3.14
radius = float(input('Please Enter the Radius of a Sphere: '))

Volume = (4 / 3) * PI * radius * radius * radius
print("\n The Volume of a Sphere = %.2f" %Volume)



a= float(input("a: "))
b = float(input("b: "))
c = (a*a +b*b)
print("The length of the hypotenuse is", c )

sentence = 'I LOVE AFRICA MOSTLY THE ANIMALS'
vowels = {'A', 'E', 'I', 'O', 'U'}
words = sentence.strip().split(' ')
pig_latin = []
 
for word in words:
    if word[0] in vowels:
        pig_latin.append(word + 'AY')
    else:
        pig_latin.append(word[1:] + word[0] + 'AY')
 
print(' '.join(pig_latin))
