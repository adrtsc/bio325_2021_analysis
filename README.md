# bio325_2021_analysis
Analysis notebooks for BIO325

## Clone the repository
Clone this repository by typing this command in your terminal

    git clone https://github.com/adrtsc/bio325_2021_analysis
    
## Activate your bio325_2021 python environment and install some additional requirements

    conda activate bio325_2021
    cd bio325_2021_analysis
    pip install -r requirements.txt
    
## Start Jupyter lab

    jupyter lab

## Mounting the data share


### On Mac: 
In Finder: Use Command-K

username: BIO325_group1

    Active Share: smb://172.23.115.13/BIO325_group1

Log in using your username & password from above

On Windows: 
Create & run a .bat file containing the following, change the mounting point to be used to 
an unused one:

    @echo off

    set uname=BIO325_group1

    set upass=Password

    set server=172.23.115.13

    set direc=BIO325_group1

    net use J: /delete

    net use J: \\%server%\%direc% %upass% /user:%uname%  /persistent:yes

    REM pausing

    timeout /t 25
