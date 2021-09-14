# o3 cpu   

## 如何做到解耦合，无阻塞？  
  * pipline   
  * 分支预测   
  * 投机执行, 分支数量       
  * pc投机错误恢复机制   
  * fifo/queue   
  * NBDcache   
  * NBDTLB   
  * multi exu     
  * multi issue   
  * wakeup机制   


## resources and match
  - rob
  - ldQ/stQ
  - fetch-buffer
  - physical register
  - issueQ
  - branchTags
  - pipelines

## resources对比
 - embedded cpu
 - sequential scalar cpu
 - sequential superscalar cpu
 - outer-of-order superscalar cpu


## 参数如何确定？   

## 性能如何评估？   

- TMA
- benchmark
  * SpecInt
  * Coremark

## 如何迭代改进？    

## pipeline

每个stage需要考虑
   - exception
   - interrupt
   - branch/branch specutive/ flush / recover
   - hazrd
   - flush

- cache   
  * icache   
  * dcache    
  * cache configure   
  * MSHR   
  * NBDcache   
- pwt  
- tlb    
  * ITLB   
  * NBDTLB    
  * page fault?    
- branch prediction    
  * type  
  * branch history size   
  * the Next-Line Predictor   
     * NLP predictions   
     * NLP updates     
        * BTB updates    
	* RAS updates     
  * the backing predictor     
    * the TAGE predictions    
    * the GShare predictions    
    * the two-bit counter tables   
  * miss resolution    
  * checkpoint    
- inst fetch    
  * exception   
  * inst buffer   
- decode   
- rename   
  * PRF design    
  * data-in-ROB design   
  * the rename map table:map-table, freelist, busy table    
  * dependency: RAR, RAW, WAW, WAR   
- issue   
  * slot resource    -> exu num
  * find vacated slot    
  * update uop status    
  * issue uop    
  * wakeup logic    
- rob   
  * oranization     
  * ROB state   
  * exception state   
  * pc storage   
  * the commit stage   
  * exceptions and flushed    
  * parameterization   
  * causes   
- Arch state     
  * csr  
- registerfile   
  * write/read arbiter   
  * bank number   
  * Dynamic read port scheduling    
  * bypass network   
- exu   
  * exu type : alu/bru/lsu...      
  * exu number ? Is it reasonable ?    
  * exu pipeline    
  * function unit: pipeline ? iterative ?   
  * insn issue & scheduling    
  * register file write/read   
  * commit/writeback issue   
- lsu   
  * LAQ   
  * SAQ   
  * SDQ   
  * dependency: RAR, RAW, WAW, WAR   
  * exception   
- performance counter   
- interrupt    
  * config interrupt    
  * debug interrupt   
  * priority   
  * check  
  * resolution    
- exception    
  * config exception   
  * priority   
  * generate & check
     * frontend exception   
     * lsu exception   
     * rob exception   
  * resolution    
- debug/trace   
  * breakpoint/trigger      
  * step   
  * trace   


