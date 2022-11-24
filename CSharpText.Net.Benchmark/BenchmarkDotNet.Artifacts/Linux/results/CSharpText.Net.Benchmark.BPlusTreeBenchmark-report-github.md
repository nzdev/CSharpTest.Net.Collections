``` ini

BenchmarkDotNet=v0.13.2, OS=ubuntu 22.04
AMD FX(tm)-8350, 1 CPU, 4 logical and 2 physical cores
.NET SDK=6.0.110
  [Host]   : .NET 6.0.10 (6.0.1022.47701), X64 RyuJIT AVX
  .NET 6.0 : .NET 6.0.10 (6.0.1022.47701), X64 RyuJIT AVX


```
|         Method |      Job |  Runtime |    Mean |   Error |  StdDev |
|--------------- |--------- |--------- |--------:|--------:|--------:|
| TestPerformace | .NET 6.0 | .NET 6.0 | 81.84 s | 1.284 s | 1.138 s |
| TestPerformace | .NET 7.0 | .NET 7.0 |      NA |      NA |      NA |

Benchmarks with issues:
  BPlusTreeBenchmark.TestPerformace: .NET 7.0(Runtime=.NET 7.0)
