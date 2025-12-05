---- 目录结构 ----
  source/               程序源代码
    ...
  compiler              编译器可执行文件 (ELF 格式, 需要 Linux 下运行)
  in.txt                示例源程序文件
  out.txt               输出的四元式
  debug.txt             输出的二元式、产生式、四元式
  program_ast.json      输出的 JSON 格式的 AST (抽象语法树)
  program.ll            输出的 LLVM IR 中间代码 (未优化)
  program_optimized.ll  输出的优化后的 LLVM IR 中间代码
  program.o             输出的目标代码文件 (ELF 格式)
  program.s             输出的汇编代码
  program               输出的可执行文件 (ELF 格式, 需要 Linux 下运行)

---- 运行说明 ----
本编译器需要在 Linux 下运行, 编译使用的环境为 Ubuntu 22.10.
运行时可加上 -h 参数查看帮助:
$ ./compiler -h
compiler - A demo compiler based on LLVM

---- 编译说明 ----
编译需要 CMake 3.10 或以上版本, LLVM 16.0 (目前还是开发版本).
Ubuntu 下安装 LLVM 的方法可参考 <https://apt.llvm.org/>, 至少需要安装 clang lld llvm-dev 这三个包.


