## Transform VsCode into IDE ##

## Setup clang WSL / Ubuntu / Linux / Debian ##

sudo apt update && sudo apt upgrade

sudo apt install gcc && sudo apt install g++

sudo apt install clang-9

--> This will install clangd as /usr/bin/clangd-9. Make it the default clangd:

sudo update-alternatives --install /usr/bin/clangd clangd /usr/bin/clangd-9 100

## Setup clang VsCode like an IDE ##

touch a.c
code a.c

--> Copy & Paste

    #include<stdio.h>
    int main()
    {
    
        int a = 10, b = 5;
        int c = a + b       // error here
        puts(c);            // error here

        return 69;
    }

--> Search on the VsCode (wsl) extension:

-> Clang

-> Code Runner

-> Path Intellisense

-> Statusbar error

-> Kite ~(optional)~

## Done ##

(c) vioo-bkp 2020-2021
