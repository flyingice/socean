# 校验程序代码

用户可以按以下方式校验部署在链上的程序：

1. 从[igneous-labs/stake-pool](https://github.com/igneous-labs/solana-program-library/tree/stake-pool/liquid-deposits)上签出`release/v0.1`代码分支。
2. 在程序目录中运行`cargo build-bpf。`
3. 按照Solana文档中的[步骤](https://docs.solana.com/cli/deploy-a-program#dumping-a-program-to-a-file)检查两个程序二进制文件的哈希值是否匹配。

主网和测试网上的账户地址均为

`5ocnV1qiCgaQR8Jb8xWnVbApfaygJ8tNoZfgPwsgx9kx`
