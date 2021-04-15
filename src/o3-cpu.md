# o3 cpu   

- cache   
  * icache   
  * dcache    
  * cache configure   
- virtual memory   
- branch prediction  
- decode   
- rename   
  * PRF design    
  * data-in-ROB design   
  * the rename map table:map-table, freelist, busy table    
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
  - LAQ   
  - SAQ   
  - SDQ   
- performance counter   
- interrupt    
- exception    
- debug/trace   
  * breakpoint/trigger      
  * step   
  * trace  
