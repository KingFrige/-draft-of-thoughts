# o3 cpu   

如何做到解耦合，无阻塞？  
  * pipline   
  * 分支预测   
  * 投机执行    
  * fifo/queue   
  * NBDcache   
  * NBDTLB   
  * multi exu     
  * multi issue   

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
- inst fetch    
  * exception   
  * inst buffer   
- branch prediction    
  * the Next-Line Predictor   
     * NLP predictions   
     * NLP updates     
        * BTB updates    
	* RAS updates     
  * the backing predictor     
    * the TAGE predictions    
    * the GShare predictions    
    * the two-bit counter tables   
- decode   
- rename   
  * PRF design    
  * data-in-ROB design   
  * the rename map table:map-table, freelist, busy table    
  * dependency: RAR, RAW, WAW, WAR   
- issue   
  * slot resource    
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
- core status   
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
- exception    
  * frontend exception   
  * lsu exception   
  * rob exception   
  * config exception   
  * priority   
- debug/trace   
  * breakpoint/trigger      
  * step   
  * trace   



