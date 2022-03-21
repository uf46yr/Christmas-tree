from time import sleep
from colorama import *
import ctypes
kernel32 = ctypes.windll.kernel32
kernel32.SetConsoleMode(kernel32.GetStdHandle(-11), 7)

print(Fore.RED + 'Happy New Year!')
schetchik = 10
paket = []
col_list = [Fore.BLUE, Fore.RED, Fore.MAGENTA, Fore.YELLOW, Fore.CYAN]
Hans_Zimmer_time = 0.3

def pos(x, y):
    return '\x1b['+str(y)+';'+str(x)+'H'

def display(txt, dx, dy, color):
    sleep(Hans_Zimmer_time)
    print(color + pos(dx, dy) + txt)

print(' ' * (schetchik + 1) + Fore.YELLOW + '*')
for i in range(1, 11):
    sleep(0.1)
    print(Fore.RESET + ' ' * schetchik + '/', end='')
    print(Fore.GREEN + '0' * i + '0' * (i - 1) + Fore.RESET + '\')
    paket.append(' ' * schetchik + '/'+ '0' * i + '0' * (i - 1) + '\')
    schetchik -= 1
for j in range(2):
    sleep(0.1)
    print(' ' * (i) + '|-|')

rezhim = input("Режим гирлядны (1, 2, 3)> ")
if rezhim == '1':
    while(True):
        for k in range(5):
            Hans_Zimmer_time = 0
            sleep(0.4)
            display(paket[1], 0, 4, col_list[k])
            display(paket[3], 0, 6, col_list[k])
            display(paket[5], 0, 8, col_list[k])
            display(paket[7], 0, 10, col_list[k])
            display(paket[9], 0, 12, col_list[k])
elif rezhim == '2':
    while(True):
        for k in range(5):
            Hans_Zimmer_time = 0
            sleep(0.4)
            display(paket[1], 0, 4, col_list[k-4])
            display(paket[3], 0, 6, col_list[k-3])
            display(paket[5], 0, 8, col_list[k-2])
            display(paket[7], 0, 10, col_list[k-1])
            display(paket[9], 0, 12, col_list[k])
elif rezhim == '3':
    while(True):
        for k in range(5):
            Hans_Zimmer_time = 0.1
            sleep(0.4)
            display(paket[1], 0, 4, col_list[k])
            display(paket[3], 0, 6, col_list[k])
            display(paket[5], 0, 8, col_list[k])
            display(paket[7], 0, 10, col_list[k])
            display(paket[9], 0, 12, col_list[k])
