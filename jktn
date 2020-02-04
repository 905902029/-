import random


dictionary=("cat","dog","rabbit","bear","sheep")
def hangman(word): 
    wrong = 0
    HP = ["",
              "_______      ",
              "|      |     ",
              "|      |     ",
              "|      |     ",
              "|      |     ",
              "|      0     ",
              "|     /|\    ",
              "|     / \    ",
              "|            "
              ]
    data = list(word)
    board = ["_"] * len(word)
    win = False
    print("単語当てゲームへようこそ!(動物)")
    while wrong < len(HP) - 1:
        print("\n")
        msg = "アルファベットを入力してください! "
        char = input(msg)
        if char in data:
            cind = data.index(char)
            board[cind] = char
            data[cind] = '0'
        else:
            wrong += 1
        print(" ".join(board))
        e = wrong + 1
        print("\n".join(HP[0:e]))
        if "_" not in board:
            print("勝利!")
            print(" ".join(board))
            win = True
            break
    if not win:
        print("\n".join(HP[0:wrong+1]))
        print("あなたは失敗しました。正解は{}".format(word))
sblsy = random.choice(dictionary)
hangman(sblsy)
