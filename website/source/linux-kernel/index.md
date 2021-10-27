---
title: Linux Kernel Exploitation
---
この章では牛さん🐮と一緒にLinuxのカーネル空間におけるExploit手法、すなわち権限昇格について学びます。WindowsのKernel Exploitでも共通のハードウェアセキュリティ機構や権限昇格の手法に関する説明も含まれています。

- 実行環境とデバッグ方法
  - [Kernel Exploitへの導入](introduction/introduction)
  - [gdbによるカーネルのデバッグ](introduction/debugging)
  - [セキュリティ機構](introduction/security)
  - [コンパイルとexploitの転送](introduction/compile-and-transfer)
- LK01: Holstein
  - [Holsteinモジュールの解析と脆弱性の発火](LK01/welcome-to-holstein)
  - [Holstein v1: Stack Overflowの悪用](LK01/stack_overflow)
  - [Holstein v2: Heap Overflowの悪用](LK01/heap_overflow)
  - [Holstein v3: Use-after-Freeの悪用](LK01/use_after_free)
- カーネル特有の攻撃手法
  - [NULL Pointer Dereference (LK02: Angus)](#)
  - [ユーザー空間のポインタの利用 (LK03: Highland)](#)
  - [Double Fetch (LK0?: Dexter)](#)
  - [Race Conditionとuserfaultfd (LK0?: Hereford)](#)
  - [BPFとJIT (LK0?: Brahman)](#)
- その他の脆弱性
  - [参照カウンタ (LK0?: Simmental)](#)
  - [サイドチャネル攻撃 (LK0?: Charolai)](#)
- UEFIに対する攻撃
  - UEFIアプリケーションの特徴
  - メモリアロケータ
