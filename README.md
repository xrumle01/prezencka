# Prezencni listina

### Úkol 1
* Naklonujte si obsah tohoto repozitáře.
  ```
  https://github.com/vut-mpc-prg/prezencka.git
  ```
* V pracovním adresáři repozitáře vytvořte prázdný textový soubor a uložte ho pod svým jménem `jmeno_prijmeni.txt`. Nepoužívejte diaktritiku.
* Vytvořte novou revizi.
  ```
    git add jmeno_prijmeni.txt
    git commit
  ```
* Na GitHubu na stránce repozitáře klikněte vpravo nahoře na tlačítko <kbd>Fork</kbd>. Vytvoří se kopie tohoto repozitáře na Vašem účtu:
  `https://github.com/vase_jmeno/prezencka`
* V příkazové řádce přidejte do Gitu adresu Vašeho vzdáleného repozitáře.
  ```
  git remote add vase_jmeno https://github.com/vase_jmeno/prezencka
  ```
* Pošlete změny na Váš vzdálený repozitář.
  ```
  git push vase_jmeno master
  ```
* Na stránkách původního repozitáře nebo na stránkách Vašeho repozitáře se nahoře objeví možnost <kbd>Compare & pull request</kbd>.
  Klikněte na ni, zkontrolujte popisek změny a pull request potvrďte.
* V případě, že autor repozitáře změny přijme, provede jejich začlenění do původního repozitáře.
  Stáhněte si aktuální verzi repozitáře.
  ```
  git pull origin master
  ```
* Ověřte stav repozitáře a zkontrolujte jeho historii.
  ```
  git status
  gitk --all
  git log
  ```


### Úkol 2
V souboru, který jste přidali do repozitáře prezencka, doplňte, jakou máte dnes náladu.

* V repozitáři prezencka vytvořte novou větev.
  ```
  git branch nazev_vetve
  ```
* Přepněte se do nově vytvořené větve.
  ```
  git checkout nazev_vetve
  ```
* V souboru se svým jménem proveďte potřebné změny.
* Vytvořte novou revizi.
* Pošlete změny do svého vzdáleného repozitáře.
  ```
  git push vase_jmeno nazev_vetve
  ```
* Vytvořte pull request.
* Po začlenění Vašich změn:
    * Přepněte se zpět na hlavní větev.
    
      ```
      git checkout master
      ```
    * Stáhněte aktuální verzi repozitáře.
    
      ```
      git pull origin master
      ```
    * Smažte větev, na které jsou změny, které byly začleněny.
    
      ```
      git branch -d nazev_vetve
      ```
