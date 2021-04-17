# o3 cpu   

无阻塞，分支预测，投机执行，fifo解耦合单元    

- cache   
  * icache   
  * dcache    
  * cache configure   
  * MSHR  
- pwt  
- tlb  
- inst fetch   
  * branch prediction    
  * exception   
  * inst buffer   
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
- exception    
- debug/trace   
  * breakpoint/trigger      
  * step   
  * trace   
