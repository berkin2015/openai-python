def toplama(x, y):
    return x + y

def cikarma(x, y):
    return x - y

def carpma(x, y):
    return x * y

def bolme(x, y):
    if y == 0:
        return "Sıfıra bölme hatası!"
    else:
        return x / y

print("İşlem seçenekleri:")
print("1. Toplama")
print("2. Çıkarma")
print("3. Çarpma")
print("4. Bölme")

secenek = input("Lütfen bir işlem seçin (1/2/3/4): ")

num1 = float(input("Birinci sayıyı girin: "))
num2 = float(input("İkinci sayıyı girin: "))

if secenek == '1':
    print("Sonuç:", toplama(num1, num2))
elif secenek == '2':
    print("Sonuç:", cikarma(num1, num2))
elif secenek == '3':
    print("Sonuç:", carpma(num1, num2))
elif secenek == '4':
    print("Sonuç:", bolme(num1, num2))
else:
    print("Geçersiz giriş!")
