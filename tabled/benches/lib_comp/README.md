# Benchmark's result


|                          | cli_table      | comfy_table   | prettytable_rs     | term_table     | tabled           | tabled_color   | tabled_compact     | tabled_iter    |
|--------------------------|----------------|---------------|--------------------|----------------|------------------|----------------|--------------------|----------------|
| test_const_table/1       | 2.5±0.02µs     | 5.0±0.07µs    | **1324.7±17.84ns** | 4.6±0.03µs     | 1642.2±33.51ns   | 1639.9±32.57ns | 1385.8±18.37ns     | 2.5±0.07µs     |
| test_const_table/8       | 49.7±0.74µs    | 54.8±0.42µs   | **23.4±0.69µs**    | 93.8±1.02µs    | 25.4±0.36µs      | 25.3±0.42µs    | 25.2±0.38µs        | 39.2±0.29µs    |
| test_const_table/32      | 664.5±3.82µs   | 698.6±3.41µs  | 335.8±1.45µs       | 1289.8±6.95µs  | **295.2±3.00µs** | 333.1±3.08µs   | 317.1±3.22µs       | 541.6±2.82µs   |
| test_const_table/128     | 9.4±0.12ms     | 11.5±0.08ms   | 5.3±0.03ms         | 17.6±0.35ms    | **4.5±0.02ms**   | 5.0±0.04ms     | **4.5±0.55ms**     | 7.5±0.05ms     |
| test_const_table/512     | 172.5±1.00ms   | 172.0±0.94ms  | 185.0±2.12ms       | 273.0±1.34ms   | 78.2±0.36ms      | 70.7±0.47ms    | **70.2±0.49ms**    | 120.5±0.75ms   |
| test_dynamic_table/1     | 2.2±0.07µs     | 5.4±0.07µs    | **858.6±15.43ns**  | 2.8±0.03µs     | 1420.5±22.66ns   | 1416.0±21.75ns | 1040.5±20.86ns     | 2.2±0.01µs     |
| test_dynamic_table/8     | 42.5±0.65µs    | 47.5±0.28µs   | **15.8±0.26µs**    | 63.9±0.46µs    | 20.7±0.38µs      | 19.2±0.28µs    | 17.5±0.27µs        | 34.7±0.84µs    |
| test_dynamic_table/32    | 538.1±9.81µs   | 703.3±3.28µs  | **225.9±2.63µs**   | 863.3±8.25µs   | 255.7±2.93µs     | 251.2±3.25µs   | 256.8±1.91µs       | 448.9±3.19µs   |
| test_dynamic_table/128   | 8.3±0.04ms     | 10.6±0.05ms   | **3.8±0.06ms**     | 14.1±0.10ms    | 4.0±0.33ms       | 3.9±0.02ms     | 4.0±0.01ms         | 7.1±0.03ms     |
| test_dynamic_table/512   | 140.0±0.80ms   | 160.2±0.86ms  | 149.6±2.07ms       | 245.4±1.04ms   | **62.2±0.35ms**  | 64.3±5.28ms    | 71.9±0.58ms        | 115.4±0.80ms   |
| test_empty_table/1       | 1579.2±13.03ns | 4.6±0.03µs    | **628.4±5.51ns**   | 2.0±0.01µs     | 1140.6±33.58ns   | 1126.3±15.39ns | 731.9±6.03ns       | 1591.7±14.58ns |
| test_empty_table/8       | 23.9±0.33µs    | 44.8±0.23µs   | **8.6±0.06µs**     | 50.0±0.36µs    | 11.2±0.05µs      | 11.3±0.08µs    | 9.4±0.05µs         | 12.6±0.10µs    |
| test_empty_table/32      | 264.5±11.17µs  | 598.1±2.98µs  | **121.7±0.74µs**   | 572.3±6.17µs   | 133.7±0.96µs     | 146.5±0.40µs   | 131.2±0.54µs       | 143.1±0.62µs   |
| test_empty_table/128     | 3.7±0.03ms     | 10.0±0.05ms   | 2.1±0.01ms         | 9.0±0.11ms     | 1963.3±7.43µs    | 1968.8±10.20µs | **1828.5±20.84µs** | 2.1±0.01ms     |
| test_empty_table/512     | 67.5±0.69ms    | 162.3±1.11ms  | 126.8±1.82ms       | 141.6±1.00ms   | 31.5±1.09ms      | 31.5±0.24ms    | **28.7±0.18ms**    | 35.8±0.18ms    |
| test_multiline_table/1   | 7.6±0.21µs     | 11.4±0.09µs   | **2.6±0.04µs**     | 10.5±0.06µs    | 5.2±0.03µs       | 5.6±0.04µs     | *2.2±0.02µs*       | 9.9±0.07µs     |
| test_multiline_table/8   | 157.4±1.81µs   | 213.1±1.42µs  | **60.9±0.37µs**    | 327.3±1.90µs   | 118.7±0.50µs     | 118.6±0.42µs   | *54.9±0.35µs*      | 252.7±1.17µs   |
| test_multiline_table/32  | 2.1±0.01ms     | 2.8±0.02ms    | **823.3±6.33µs**   | 4.3±0.04ms     | 1688.3±8.37µs    | 1627.1±6.26µs  | *793.8±10.24µs*    | 3.5±0.04ms     |
| test_multiline_table/128 | 34.8±0.37ms    | 46.8±0.26ms   | **12.9±0.07ms**    | 71.1±0.33ms    | 25.0±0.13ms      | 25.6±0.19ms    | *11.3±0.09ms*      | 48.2±0.25ms    |
| test_multiline_table/512 | 583.7±3.61ms   | 741.4±21.18ms | **337.1±1.86ms**   | 1022.6±13.76ms | 408.9±10.96ms    | 406.9±27.88ms  | *177.5±1.04ms*     | 759.4±5.55ms   |

* tabled_compact doesn't support multiline strings

## Table Generation

You can generate the table by this command (it relays on `critcmp`).

```bash
cargo run --manifest-path=readme/Cargo.toml
```

#### System

```
Kernel: 5.18.9-arch1-1 
CPU: 11th Gen Intel i7-11850H (16) @ 4.800GHz
```
