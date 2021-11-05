cpu performance
===================

- structural hazards
- data hazards
- control hazards(branch, exceptions)


bubbles analysis
------------------

- commit  bubbles  -> rob
- issue  bubbles   -> issuleQ
- frontEnd bubbles -> fetchBuffer


hazards analysis
-------------------

- decode hazards
- dispatch hazards


resource analysis
-------------------

- state
  * empty
  * full

- fetch buffer
- issueslots
- lsu: ldq/sdq/saq
- rob
- rename stage:phy-register/freelist
- branchTags

- register file ports
- alu ports


top-down summarize
----------------------

- top-down method accomplish
  * events & counters define
  * debug

- top-down hierachy framewaork

- data collection & analysis 
  * benchmarks porting: coremark/spec2006Int

- improve design


the strategies for data hazards
--------------------------------

- interlock
- bypass
- speculate
  * branch prediction


flow
-------

- understand benchmark
- get insn info, draw histogrm & pie chart
- predict performance boltleneck from insn info
- get tma info, draw chart
- analysis performance
- optimize performance


performance data analysis & show
----------------------------------

- benchmarks info scripts 
  * dram histogrm 
  * pie chart
- spec2006 build 
  * tma counter read 
  * info counter read 
  * cnt remap scripts
- perfmance regression
  * flow scripts 
  * data show & chart show


