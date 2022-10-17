# python-global
ATM存取款

def menu():
    print("--------------主菜单-----------------------")
    print("周,wlcome to hemaatn m,make your choice....")
    print("查询余额\t\t\t[1]")
    print("存款  \t\t\t[2]")
    print("取款  \t\t\t[3]")
    print("退出  \t\t\t[4]")
    print("请输入你的选择")

def chaxun():
    print(f"yue{money}\n")

def cunkuan():
    print('cunduoshao\n')
    a=int(input(""))
    global money
    money+=a
    print(f"cun{a}\n")
    print(f"yue{money}\n")

def qukuan():
    a=int(input("quduoshao"))
    global money    #important
    money-=a
    print(f"qu{a}\n")
    print(f"yue{money}\n")

def exeit():
    exit()

money=5000000
name=None
a=0
choice=0
menu()
while(2):
    choice=int(input("choice?"))
    if choice==1:
        chaxun()
    elif  choice == 2:
            cunkuan()
    elif  choice==3:
        qukuan()
    elif  choice==4:
        exeit()
