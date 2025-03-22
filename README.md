# CSE108C-Project3
### Compilation command
 g++ -std=c++20 -o seal_oram_benchmark \                 
    benchmark_seal_oram.cpp seal_oram.cpp oram_client.cpp oram_block.cpp oram_bucket.cpp oram_tree.cpp position_map.cpp aes256.cpp  \
    -I./include \
    -I/opt/homebrew/opt/openssl/include \
    -L/opt/homebrew/opt/openssl/lib -lssl -lcrypto \
    -arch arm64
