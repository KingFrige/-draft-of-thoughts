# o3 cpu micro-Archtecture analysis


## performance


### retired bubbles  

cause：

- 指令数据相关
- 执行资源单元exu有限(div unit, numbers of ALU ...)
- memory bound(Dcache miss, L2Cache miss, DRAM long latency ...)
- rob empty
- branch mispredict


### writeBack bubbles  

cause：

- issue slots data harzd
- memory bound
- instruction type & numbers of exu & type of exu don't match
- issue slots empty


### issue bubbles  

cause：

- issue slots data harzd
- instruction type & numbers of exu & type of exu don't match
- issue slots empty


### fetch bubbles   

cause：

- branch resteers
- machine clear
- branch redirect  
- ICache miss
- ITLB miss


### branch resteers   


### machine clear   


### resource status  
 - fetch buffer  
 - decode width  
 - branch mask  
 - issue slots  
 - exu  
 - physical registers  
 - rob entry  
 - load buffer  
 - store buffer  


### memory  
 - miss  
 - hit  
 - icache/dcache/L2/L3 
 - dram  
 - latency


## power


## reference


