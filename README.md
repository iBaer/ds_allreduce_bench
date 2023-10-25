usage:
1. modify run_comm_bench.sh and modify parameters as you need, especially bind_core_list to fit your machine configuration
2. run with the following args:
    run_comm_bench.sh [args]
* --elements: number of elements, default 16384
* --dtype: data type (bf16 or fp32), default bf16
* --count: number of iterations, default 10000
* --ccl: if present use oneccl allreduce, otherwise call deepspeed inference_all_reduce which intend to optimize for inference
