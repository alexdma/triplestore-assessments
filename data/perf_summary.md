# Summary of perforance analyses of RDF Triple Stores

This document provides a summary of the results of performance analyses of RDF triple store. It includes loading time, query response time and memory use from a number of references. We focused on analysis of performance using the LUBM benchmark to be consistent and since it is relevant to the considered scenario.

## Loading time:

### Virtuoso:
- 30 to 37 KT/s for 1GT (virtuoso_lubm)

### AllegroGraph:
- 500KT/s on 1GT (allegro_lubm)
- 30 to 50 hours on GT (bench3)

### Jena:
- 5 to 9 KT/s on 10MT (jena_load_lubm)
- 30 to 70 hours on GT (bench3)

### Oracle:
- 30 to 60 hours on GT (bench3)

### Sesame:
- 30 to 60 hours on GT (bench3)
  
## Query response time

### Virtuoso:
- 2 to 950ms on MT, 7 to 14K on 100MT (virtuoso lubm)
- avg of 16.8 on 100MT (bench1)

### Allegro:
- 7ms to 389K ms on BT (allegro_lubm2)
- Best on BT (bench3)

### Jena:
- 40 to 230K ms on 10MT only on Q1 and Q2 (jena_lubm_perf)
- avg of 35.1 on 100MT (bench1)
- 500 to 1100ms on LUBM 1, 600 to 1443 on LUBM5, 691 to 9481 on LUMB10, 825 to 11796 on LUBM15 ()
- worst on query response on MT (bench3)

### Sesame:
- avg of 164.7 on 100MT (bench1)
- second worst on GT (bench3)   

### Oracle:
- second best on GT (bench3)
   
## Memory usage

### Jena:
- last on GT (bench3)

### Sesame:
- second last on GT (bench3)

### Oracle:
- second on GT (bench3)

### AllegroGraph:
- First on GT (bench3)

## References

@misc{virtuoso_lubm,
title={Virtuoso benchmarking LUBM},
url={http://vos.openlinksw.com/owiki/wiki/VOS/VOSArticleLUBMBenchmark}
}


@misc{allegro_lubm,
title={AllegroGraph overview including performance},
url={https://franz.com/agraph/allegrograph/}
}

@misc{allegro_lubm2,
title={AllegroGraph LUBM results},
url={https://franz.com/agraph/allegrograph/agraph_bench_lubm.lhtml}
}

@misc{jena_load_lubm,
title={Jena Loading Tests},
url={https://jena.apache.org/documentation/sdb/loading_performance.html}
}

@misc{jena_lubm_perf,
title={Jena LUBM perf},
url={https://jena.apache.org/documentation/sdb/query_performance.html}
}

@misc{bench1,
title={Benchmark 1}
url={file:///home/mdaquin/Downloads/2463676.2463718.pdf}
}

@misc{bench2,
title={Benchmark 2},
url={file:///home/mdaquin/Downloads/An_Efficient_Web_Ontology_Storage_Considering_Hierarchical_Knowledge_for_Jena-based_Applications.pdf}
}

@misc{bench3,
title={Benchmark 2},
url={http://www.ijaema.com/gallery/137-december-3030.pdf}
}

@misc{bench4,
title={Benchmark 4},
url={https://www.researchgate.net/profile/Ian_Emmons/publication/220830290_An_Evaluation_of_Triple-Store_Technologies_for_Large_Data_Stores/links/542015090cf2218008d43aa5/An-Evaluation-of-Triple-Store-Technologies-for-Large-Data-Stores.pdf}
}
