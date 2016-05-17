Benchmark Report
================


BenchmarkDensify
----------------

                       name | rank | runs |     mean |        sd | timesBaseline
----------------------------|------|------|----------|-----------|--------------
vector densify with densify |    1 |   10 | 0.001449 | 0.0003481 |           1.0
   vector densify with list |    2 |   10 |  0.07557 | 0.0009807 | 52.1627692662
  vector densify with numpy |    3 |   10 |   0.2802 |  0.009282 | 193.379515197
     list densify with list |    4 |   10 |     1.87 |  0.008533 | 1291.06357069

BenchmarkGet
------------

                             name | rank | runs |    mean |        sd | timesBaseline
----------------------------------|------|------|---------|-----------|--------------
  list get with iterable in slice |    1 |   10 | 0.01772 | 0.0003871 |           1.0
vector get with iterable in slice |    2 |   10 | 0.09265 | 0.0003645 | 5.22984521057

BenchmarkInit
-------------

                   name | rank | runs |      mean |        sd | timesBaseline
------------------------|------|------|-----------|-----------|--------------
              list init |    1 |   10 | 2.122e-06 | 1.115e-06 |           1.0
            vector init |    2 |   10 | 6.413e-06 | 5.725e-06 | 3.02247191011
vector init with values |    3 |   10 | 3.099e-05 |  1.36e-05 |  14.606741573
  list init with values |    4 |   10 |  0.004799 |  0.001472 | 2261.85393258

BenchmarkSet
------------

                                      name | rank | runs |     mean |        sd | timesBaseline
-------------------------------------------|------|------|----------|-----------|--------------
vector set with iterables in slice present |    1 |   10 | 0.001995 | 4.278e-05 |           1.0
   list set with iterables in slice absent |    2 |   10 | 0.004164 | 0.0001024 | 2.08773607459
  list set with iterables in slice present |    3 |   10 | 0.004979 | 0.0001566 |  2.4960315563
 vector set with iterables in slice absent |    4 |   10 | 0.006616 | 0.0002026 | 3.31687783887

Each of the above 140 runs were run in random, non-consecutive order by
`benchmark` v0.1.5 (http://jspi.es/benchmark) with Python 2.7.10
Linux-4.2.0-16-generic-x86_64 on 2016-05-17 05:29:44.


Process finished with exit code 0
