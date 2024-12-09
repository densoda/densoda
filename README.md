def galvenā_programma():
    kopējā_summa = 0  
    print("Ievadiet precs cenu un daudzumu. Lai beigtu ievadi, ievadiet '0' kā cenu.")
    
    while True:
        try:
            cena = input("Ievadiet preces cenu: ")
            if cena == "0":  
                break
            cena = float(cena)  
            daudzums = int(input("Ievadiet preces daudzumu: "))
        
            starpsumma = cena * daudzums
            kopējā_summa += starpsumma
            
            print(f"Preču kopējā summa: {starpsumma:.2f} €")
        except ValueError:
            print("Lūdzu, ievadiet derīgu cenu un daudzumu!")
    
    print(f"Kopā: {kopējā_summa:.2f} €")
    print("Programma beidzās. Paldies par lietošanu!")
    
galvenā_programma()
