# 🧵 FIZZBUZZ - Classic FizzBuzz to run a simple Google Benchmark 

### Installing Google benchmark
$ git clone https://github.com/google/benchmark.git

### Enter the newly cloned directory
$cd benchmark

Use **cmake** to create a build directory to place the build output:

`$ cmake -E make_directory "build"`

Use cmake to generate build system files with and download any dependencies:

`$ cmake -E chdir "build" cmake -DBENCHMARK_DOWNLOAD_DEPENDENCIES=on -DCMAKE_BUILD_TYPE=Release ../`

Finally, build the library:

`$ cmake --build "build" --config Release`

cd ..

## 📁 RUN Benchmarks
`$ g++ -std=c11 -isystem benchmark/include -Lbenchmark/build/src play_game.cpp benchmark_game.cpp -lbenchmark -o benchmark_game lpthread && ./benchmark_game`

### Output

![Benchmark res!](/assets/benchmark_results.png "Benchmark Results")
