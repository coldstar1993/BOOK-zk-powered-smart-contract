# BOOK-zk-powered-smart-contract
Writing a book about Smart Contracts powered by Zero Knowledge Proof.
基于这两年的积累，我正在写一系列文章介绍基于零知识证明的智能合约!

### Outline

- [先从一个普通智能合约说起]()
- [走进零知识证明]()
  - 基础认知
    - 基础知识
    - 扩容+隐私
  - 目前大热应用
    - 以太坊
      - Circom+Snarkjs
        - TornadoCash等Dapp
      - ZoKrates
    - StarkNet
      - Cairo
    - Aztec
      - Noir
    - Mina
      - Snarkyjs+zkApp
    - Aleo
      - Leo
- [尝试改造普通合约]()
  - 利用circom+snarkjs
      - 思维转变提点
        - 链上逻辑大前置
          - 转为 "链下(电路+proof)+链上验证"
            - 永远记得：电路即合约！
        - 小粒度的链上存储+借助Merkle Tree实现链下存储
          - 链下扩容
        - zkSnark还得Trusted Setup!
          - 生成Proving Key和Verification Key
          - Growth16两阶段
            - proof体积最小
          - Plonk的第二阶段Setup简单些
        - 生成证明时间很长的
   - 再利用noir改造一遍
     - **TODO**
   - 再利用ZoKrates改造一遍
     - **TODO**
- [深入学习circom电路]()
  - 静态电路！
    - 电路就是一堆约束而已
    - 编译期就得确定一切
    - 电路展开
  - if-else不一样了
    - 所有逻辑分支都执行，只是输出符合条件的分支结果
  - ifelse、while和for循环的坑点
  - 电路组件化以复用
  - 常见社区电路lib
  - Trusted Setup!
  - 分析TornadoCash等Dapp
  - **TODO**
  
- [深入学习Noir电路]()
  - 重新实现TornadoCash
  - **TODO**

- [深入学习Mina的zkApp]()
  - Snarkyjs YYDS!
    - 丝滑-Typescript
    - 丝滑-无须Trusted Setup
    - 麻烦-初始化慢+动态import
    - 麻烦-COOP+COEP启动worker线程
  - 少得可怜的链上存储
    - 麻烦点-链下存储很必要
    - 麻烦点-并发竞争太激烈
    - 麻烦点-证明时的链上状态和验证时不一致
  - zkApp
    - 每次访问都得重新编译电路
      - 最好SPA
  - **TODO**

- [深入学习StarkNet的Cairo]()
  - 了解zkVM
  - Cairo1.0语法好像Rust
  - **TODO**
  
- [深入学习Aleo的Leo]()
  - Aleo的特点
  - Leo语法
  - **TODO**
