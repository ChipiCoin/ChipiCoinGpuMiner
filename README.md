# README

[Сообщество](https://t.me/blckbazars)

[Канал жетона](https://t.me/chipicoinru)

Майнер для жетона ChipiCoin. Данный майнер является форком майнера для жетона GRAM. 

Для работы требуется GPU.

- Скачайте содержимое данного репозитория
- Создайте `config.txt` внутри папки с майнером
- Напишите мнемоник в файле `config.txt` в формате

```
SEED=word1 word2
TONAPI_TOKEN=your-token
```

- Активируйте v4r2 кошелек. Отправьте на него средства, а потом отправьте транзакцию самому себе.
- Установите NodeJs [https://nodejs.org](https://nodejs.org/en)
- Запустите майнер открыв `start_tonhub.bat` (для AMD - `start_tonhub_amd.bat`)

### TonApi
Так же вы можете использовать TonApi (tonconsole.com) как провайдер апи. Он дает повышенную стабильность, но не работает без ключа.
На 1 майнер достаточно бесплатного токена.
Для запуска майнера с tonapi используйте `start_tonapi_X.bat` или `start_tonapi_X.sh`(с суффиксом \_amd для компьютеров без CUDA).

### Multi GPU
Можно запустить несколько видеокарт одним скриптом. Пример в файле `start_multi_8.sh` и `start_multi_8.bat`.
Чтобы превратить любой стартовый скрипт в мульти, надо заменить `send_universal` на `send_multigpu`
`--gpu 0` заменить на `--gpu-count X`, где Х кол-во ваших GPU.
Больше ничего менять не нужно, можно запускать.

## EN
[Community](https://t.me/blckbazars)

[Jetton channel](https://t.me/chipicoin)

Miner for ChipiCoin jetton. This miner is a fork of the GRAM jetton miner.

GPU is needed.

- Download the contents of this repository
- Create `config.txt` inside the folder with the miner
- Write the mnemonic in the `config.txt` file in the following format

```
SEED=word1 word2
TONAPI_TOKEN=your-token
```

- Activate v4r2 wallet linked to mnemonic and send some funds to it.
- Install nodejs [https://nodejs.org](https://nodejs.org/en)
- Start miner by opening `start_tonhub.bat` (for AMD - `start_tonhub_amd.bat`)

### TonApi
You can also use TonApi (tonconsole.com) as an api provider. It gives increased stability, but does not work without a token.
A free token is enough for 1 miner.
To start the miner with tonapi use `start_tonapi_X.bat` or `start_tonapi_X.sh` (with suffix \_amd for computers without CUDA).

### Multi GPU
You can start multiple GPU's with one script. Examples are in start_multi_8.sh and start_multi_8.bat.
To turn any start script into a multi script, replace send_universal with send_multigpu --gpu 0 with --gpu-count X, where X is the number of your GPUs.
You don't need to change anything else, it is ready to run.