
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
> 1. Running the codes:
>> $ python codes.main.py   
> 2. Input files:
>> all input files are in the path ./data/  
>>>   ├─data      
>>>　　　├─basic      
>>>　　　├─csmar    
>>>　　　│  ├─csmar_finance    
>>>　　　│  └─csmar_trade      
>>>　　　├─para_file     
>>>　　　└─rf     
>>> Download csmar_master.sas7bdat from [WRDS](https://wrds-www.wharton.upenn.edu/) to the local path './data/csmar/csmar_finance/'  
>>> Download csmar_t_mnth.sas7bdat from [WRDS](https://wrds-www.wharton.upenn.edu/) to the local path './data/csmar/csmar_trade/'  
>>> rf.xlsx in path './data/rf/' is the market risk free return
>>> 
>>> './data/para_file/' includes the corresponding parameters files, which can be created by 
>>> running orders: $ python codes.params.XXX.py, where XXX.py are in the path './codes/params/'
>>> For example, running: $ python codes.params.para_construct_portfolio.py to update the file 
>>> 'para_construct_portfolio.csv' in path './data/para_file/'    
>> 3. Output files:    
>> all the results are in the path ./output/

* Tips: 

> 1. How to add predictors 
>
>> ├─codes      
>>　　　├─predictors   
>>　　　　　├─ ep.py  
>>　　　　　└─ market_cap.py 
>>
>> create a predictor_name.py follow the writing styles of examples i.e. ep.py and market_cap.py 
>> see more details in [Read The Docs](https://stock-predictors.readthedocs.io/en/latest/) 
  
* Notes:  
> The frequency of data: monthly.