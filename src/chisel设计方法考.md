# chisel   

> chisel - sv - gem5   
> generator vs simulator

## CDE -> parameter-config   

## design-flow   
### systemverilog    
### chisel    
### gem5   

## framework   
### chisel   
  - diplomacy   
  - remapper   
  - sifive-block   
  - rocket-chip    
  - chipyard   
  - dir structure  
  - report info    
  - ci/cd   
### systemverilog    

## modeling -> computing resource   
  - flow    
  - Synchronization of model and design   
  - PPA quantify   
  - Fast convergence : run time / design time / convert to RTL    

## generator / simulator   
  - parameter   
  - Postpone decision -> lazy val
  - basic component: ram/rom/buffer/fifo   
  - instance  
  - connect  
  - class/function   

  - 为什么需要simulator?
  - 如何写一个simulator？   
  - 如何simulator定义灵活的参数呢？   
  
  - 为什么需要generator?
  - 如何写一个generator？   
  - 如何generator定义灵活的参数呢？   
  
  - simulator == generator吗？   
  - 使用chisel写simulator呢？  
  
  > c/c++ - verilog的世界，c/c++用于创建simulator，verilog用于创建参数化的RTL，通常用python/perl辅助创建generator   
 
## IDEA/Editer  
  - IDEA  
  - vim/ctag    
  - verdi  

## doc   
  - scala doc   
  - doxygen

## summary 
  * chisel
    - performance flow   
    - Computing resources   
  * sv
  * gem5
