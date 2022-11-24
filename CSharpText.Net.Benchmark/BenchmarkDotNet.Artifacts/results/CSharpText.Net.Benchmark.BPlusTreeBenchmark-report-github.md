``` ini

BenchmarkDotNet=v0.13.2, OS=Windows 10 (10.0.19045.2251)
AMD FX(tm)-8350, 1 CPU, 8 logical and 4 physical cores
  [Host]               : .NET Framework 4.8 (4.8.4515.0), X64 RyuJIT VectorSize=128
  .NET 6.0             : .NET 6.0.11 (6.0.1122.52304), X64 RyuJIT AVX
  .NET 7.0             : .NET 7.0.0 (7.0.22.51805), X64 RyuJIT AVX
  .NET Framework 4.6.2 : .NET Framework 4.8 (4.8.4515.0), X64 RyuJIT VectorSize=128
  .NET Framework 4.8   : .NET Framework 4.8 (4.8.4515.0), X64 RyuJIT VectorSize=128


```
|         Method |                  Job |              Runtime |    Mean |    Error |   StdDev | Ratio |
|--------------- |--------------------- |--------------------- |--------:|---------:|---------:|------:|
| TestPerformace |             .NET 6.0 |             .NET 6.0 | 7.220 s | 0.0323 s | 0.0302 s |  0.88 |
| TestPerformace |             .NET 7.0 |             .NET 7.0 | 7.097 s | 0.0375 s | 0.0351 s |  0.87 |
| TestPerformace | .NET Framework 4.6.2 | .NET Framework 4.6.2 | 8.171 s | 0.0740 s | 0.0692 s |  1.00 |
| TestPerformace |   .NET Framework 4.8 |   .NET Framework 4.8 | 8.215 s | 0.0303 s | 0.0283 s |  1.01 |
