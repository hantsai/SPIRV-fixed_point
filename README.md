# SPIRV-fixed_point


#kernel.cl to SPIR-V bit code
clang -cc1 -emit-spirv -triple=spir-unknown-unknown -cl-std=c++ -I /home/chtsai/llvm/llvm-3.6.1.src/tools/master/include/ -x cl xxx.cl -o xxx.spv
#go to spirv_tool/build/tool/
#.spv to human can read
./spirv-dis ~/llvm/llvm-3.6.1.src/tools/master/test/libclcxx/vec/test.spv test.spv.dis
