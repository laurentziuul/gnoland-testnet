# gnoland-testnet
Ordinea în care exec ar fi urmaotoarea : 

Din CMD sau Shell ,deschizi cu admin,dupa fiecare comnda dai enter



wsl --install

După instalare dai restart la PC

Ubuntu pornește automat ,aștepti cateva min ..

Creezi Username din litere mici + parola-repeti parola (parola nu e vizibila)

 Next ,facem Linux upgrade 

sudo apt update && sudo apt upgrade

Acum instalam GO

cd $HOME

Ultima versiune GO

wget https://go.dev/dl/go1.18.3.linux-amd64.tar.gz

Unzip file

sudo tar -xvf go1.18.3.linux-amd64.tar.gz

Mutam fisierul GO in 📁 local
 
sudo mv go /usr/local


Pt a accesa GO din linia de comanda ..

nano ~/.bashrc

Apesi pe tasta săgeata jos până se termină :)) și tastezi 

export GOROOT=/usr/local/go
export GOPATH=$HOME/go
export PATH=$GOPATH/bin:$GOROOT/bin:$PATH

Apasa Ctrl O (O de la Ovidiu) apoi enter pt a salva modificările
Apoi Ctrl X pt a închide configurarea

Restart Ubuntu cu executare ca admin

Verifica  versiunea GO pe care ai instalat-o:

go version

Ar trebui că raspuns sa ai: go version go1.18.3

Mergem mai departe cu:

sudo apt install make

Clonam Gnoland repository:

clone https://github.com/gnolang/gno/


Dupa faza de mai sus ori de cate ori vrei sa interacționezi cu gnoland apesi cd gno
Acum activam gno:

cd gno


Folosim comanda make pt 🏢

make


Cream mnemonic seed phrase din 24 cuv ,salvati-le !


./build/gnokey generate



Acum cream contul initial:

./build/gnokey add account --recover

Pui o parola -repeti parola ,Nu uita parola! :))

Introduci seed phrase 24 cuv 

 vezi adresa pe care ai generat-o ,addr: g1xxxxx

Intra pe https://gno.land/faucet , lipește adresa si obtine testnet tokens pt următoarele misiuni ,🔥
