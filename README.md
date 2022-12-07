# コンテナのビルド

## 手動でビルドする場合

```bash
$ docker buildx bake -f docker-compose.yml
$ docker compose up -d
```

## vscodeのremote containerでビルドする場合

`Open Folder in Container`でルートディレクトリを開く

# cmakeの利用方法

## ビルド

```bash
$ cmake -S . -B build
$ cmake --build build
```

## テストの実行

```bash
$ cd build
$ ctest
Test project /work/build
    Start 1: HelloTest.BasicAssertions
1/1 Test #1: HelloTest.BasicAssertions ........   Passed    0.00 sec

100% tests passed, 0 tests failed out of 1

Total Test time (real) =   0.01 sec
```
