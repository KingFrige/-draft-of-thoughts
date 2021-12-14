# o3 cpu micro-Archtecture analysis


## performance

- 哪些地方存在性能瓶颈？
- pipeline阻塞：structural hazard, data hazard, control hazard
- 性能瓶颈在vcs/verilator仿真的波形的什么位置？
- 如何使用计数器统计性能瓶颈点？
- TMAM的计数器在流水线的位置？


### retired bubbles  

> 没有指令retired的slots

cause：

- 指令数据相关
- 执行资源单元exu有限(div unit, numbers of ALU ...)
- memory bound(Dcache miss, L2Cache miss, DRAM long latency ...)
- rob empty
- branch mispredict


### writeBack bubbles  

> 没有uops写回到rob的slots

cause：

- issue slots data hazard
- memory bound
- instruction type & numbers of exu & type of exu don't match
- issue slots empty


### issue bubbles  

> 没有uops发射到exu的slots

cause：

- issue slots data hazard
- instruction type & numbers of exu & type of exu don't match
- issue slots empty


### fetch bubbles   

> 没有uops分发到rob/rename阶段的slots

cause：

- branch resteers
- machine clear
- branch redirect  
- ICache miss
- ITLB miss


### branch resteers   

> 由于多个阶段的分支预测器预测不一致导致的pc重定向的cycles


### machine clear   

> csr指令执行造成流水线flush的情况


### resource status  

> 资源不足有可能造成pipeline的阻塞

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

> RISC指令集中，load/store对应的memory系统往往存在memory wall

 - miss  
 - hit  
 - icache/dcache/L2/L3 
 - dram  
 - latency


## power


## reference


