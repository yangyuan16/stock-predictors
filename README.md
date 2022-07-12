
###  Open-assetpricing-china

#### Stock-predictors

* Get the codes:
 
> $ git clone https://github.com/yangyuan16/stock-predictors.git

* View docs:

> documentation is now at [Read The Docs](https://stock-predictors.readthedocs.io/en/latest/) 
> or just click https://stock-predictors.readthedocs.io/en/latest/

* Directory tree:

> ├─codes    
> │  ├─factor_model  
> │  ├─params  
> │  ├─predictors  
> │  ├─utils  
> ├─data  
> │  ├─basic  
> │  ├─csmar  
> │  │  ├─csmar_finance  
> │  │  └─csmar_trade    
> │  ├─para_file   
> │  └─rf  
> └─output  
>　　├─factor_model  
>　　├─portfolio_performance  
>　　├─portfolio_ret  
>　　└─predictors  

* Usage:

> $ python codes.main.py 

* Tips: 

> 1. How to add predictors 
>
>> ├─codes      
>>　　　├─predictors   
>>　　　　　├─ ep.py  
>>　　　　　└─ market_cap.py 
>
>> create a predictor_name.py follow the writing styles of examples i.e. ep.py and market_cap.py 
>> see more details in [Read The Docs](https://stock-predictors.readthedocs.io/en/latest/) 