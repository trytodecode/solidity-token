creation of token

created contract to mange token 

 Description

created contract to mange tokens and transaction and it gives insight to learn about transaction
we can set limit of gas and later we can update the limit {our gas limit should always be greater than gas burn }

 Getting Started

 Installing

* we have to open online IDE provided (remix) and then have to perform our execution
* files which is upload in doc format to execute make sure it will in solidity(.sol) format

Executing program

 after writing the code in  the contract section then go to solidity.compiler and compiler the written code  if your compiler is setted to auto compile you dont need to compile manually  afte that you need to go on run and deploy section and then click on deploy your program is ready to run 

* open solidity IDE
* create a file in the format of(.sol)
* write the code of your solidity of token 
* go to compiler section of IDE
* you need to compile  if you compiler is setted to auto compile you dont need to compile your program manually
* and then go to deploy section and deploy  then we observe you contract is ready 


contract MyToken {

    // public variables here
    string public token_name="etherum";
    string public token_ab="eth";
    uint public total_supply=101;
   

    // mapping variable here
     mapping(address => uint) public mapp;
     

    // mint function
     function mint(address _add, uint _u)public {
          total_supply += _u;
          mapp[_add] += _u;

     }

    // burn function
    function burn(address _add, uint _u)public {
      if(mapp[ _add] >= _u){
         total_supply-= _u;
        mapp[ _add] -=_u;
      }
    }

}

 Help

 please mase sure before running the program  your compiler should be set according to version your are adding in your code 
```
click on compile to run code
after that click on deploy to exexute the program
```

 Authors

kumar sanjeev 
https://www.linkedin.com/in/kumar-sanjeev-150965230/




License

This project is licensed under the [MIT LICENSE] License - see the LICENSE.md file for details
