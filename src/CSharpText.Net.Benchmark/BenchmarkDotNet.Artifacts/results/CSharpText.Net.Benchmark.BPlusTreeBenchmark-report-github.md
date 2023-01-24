``` ini

BenchmarkDotNet=v0.13.2, OS=macOS 13.1 (22C65) [Darwin 22.2.0]
Apple M1 Pro, 1 CPU, 10 logical and 10 physical cores
.NET SDK=7.0.102
  [Host]   : .NET 6.0.11 (6.0.1122.52304), Arm64 RyuJIT AdvSIMD
  .NET 6.0 : .NET 6.0.11 (6.0.1122.52304), Arm64 RyuJIT AdvSIMD
  .NET 7.0 : .NET 7.0.2 (7.0.222.60605), Arm64 RyuJIT AdvSIMD


```
|         Method |      Job |  Runtime |    Mean |    Error |   StdDev |
|--------------- |--------- |--------- |--------:|---------:|---------:|
| TestPerformace | .NET 6.0 | .NET 6.0 | 3.470 s | 0.0690 s | 0.1226 s |
| TestPerformace | .NET 7.0 | .NET 7.0 | 2.929 s | 0.0567 s | 0.0653 s |
